# Comparing `tmp/embetter-0.4.0.tar.gz` & `tmp/embetter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/embetter-0.4.0.tar", last modified: Sat Jun 17 12:49:36 2023, max compression
+gzip compressed data, was "dist/embetter-0.4.1.tar", last modified: Fri Jun 30 08:55:01 2023, max compression
```

## Comparing `embetter-0.4.0.tar` & `embetter-0.4.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-17 12:49:36.000000 embetter-0.4.0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4061 2023-06-03 11:05:06.000000 embetter-0.4.0/README.md
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-05-01 13:07:12.000000 embetter-0.4.0/embetter/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.4.0/embetter/base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.4.0/embetter/error.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/external/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/external/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/external/_cohere.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/external/_openai.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/finetune/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/finetune/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5414 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/finetune/_contrastive.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/finetune/_forward.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/grab.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/multi/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/multi/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1758 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/multi/_clip.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/text/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.4.0/embetter/text/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/text/_bpemb.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.4.0/embetter/text/_s2v.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-06-03 11:05:04.000000 embetter-0.4.0/embetter/text/_sbert.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.4.0/embetter/text/_spacy.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2437 2023-06-17 12:37:51.000000 embetter-0.4.0/embetter/utils.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter/vision/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_colorhist.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_loader.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.4.0/embetter/vision/_torchvis.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      878 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1209 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-06-17 12:49:36.000000 embetter-0.4.0/embetter.egg-info/top_level.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-17 12:49:36.000000 embetter-0.4.0/setup.cfg
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2615 2023-06-17 12:26:56.000000 embetter-0.4.0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-17 12:49:36.000000 embetter-0.4.0/tests/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.4.0/tests/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.4.0/tests/test_base.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.4.0/tests/test_default.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.4.0/tests/test_docs.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      452 2023-06-03 11:05:04.000000 embetter-0.4.0/tests/test_finetuners.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3033 2023-06-17 12:37:00.000000 embetter-0.4.0/tests/test_text.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.4.0/tests/test_vision.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-30 08:55:01.000000 embetter-0.4.1/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4061 2023-06-03 11:05:06.000000 embetter-0.4.1/README.md
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-05-01 13:07:12.000000 embetter-0.4.1/embetter/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      326 2022-09-17 15:40:35.000000 embetter-0.4.1/embetter/base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      742 2022-07-16 12:25:08.000000 embetter-0.4.1/embetter/error.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/external/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      256 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/external/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2001 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/external/_cohere.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2356 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/external/_openai.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/finetune/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      401 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/finetune/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5823 2023-06-30 08:54:47.000000 embetter-0.4.1/embetter/finetune/_contrastive.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2851 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/finetune/_forward.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2408 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/grab.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/multi/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      185 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/multi/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1758 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/multi/_clip.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/text/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      730 2023-03-28 13:55:26.000000 embetter-0.4.1/embetter/text/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3794 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/text/_bpemb.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1579 2023-03-28 13:55:22.000000 embetter-0.4.1/embetter/text/_s2v.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3179 2023-06-03 11:05:04.000000 embetter-0.4.1/embetter/text/_sbert.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2767 2023-03-28 13:55:22.000000 embetter-0.4.1/embetter/text/_spacy.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4364 2023-06-30 08:54:47.000000 embetter-0.4.1/embetter/utils.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter/vision/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      361 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1980 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_colorhist.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2205 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_loader.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2056 2023-02-09 16:06:49.000000 embetter-0.4.1/embetter/vision/_torchvis.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5227 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      898 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1209 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       15 2023-06-30 08:55:01.000000 embetter-0.4.1/embetter.egg-info/top_level.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       38 2023-06-30 08:55:01.000000 embetter-0.4.1/setup.cfg
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2615 2023-06-30 08:54:47.000000 embetter-0.4.1/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-30 08:55:01.000000 embetter-0.4.1/tests/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2021-10-31 16:15:20.000000 embetter-0.4.1/tests/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      324 2022-12-05 09:29:24.000000 embetter-0.4.1/tests/test_base.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       64 2022-07-16 12:25:08.000000 embetter-0.4.1/tests/test_default.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      910 2023-02-09 16:06:49.000000 embetter-0.4.1/tests/test_docs.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      694 2023-06-30 08:54:47.000000 embetter-0.4.1/tests/test_finetuners.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3033 2023-06-29 15:07:29.000000 embetter-0.4.1/tests/test_text.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      569 2023-06-30 08:54:47.000000 embetter-0.4.1/tests/test_utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      871 2022-12-05 09:29:24.000000 embetter-0.4.1/tests/test_vision.py
```

### Comparing `embetter-0.4.0/PKG-INFO` & `embetter-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.4.0
+Version: 0.4.1
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
```

### Comparing `embetter-0.4.0/README.md` & `embetter-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/error.py` & `embetter-0.4.1/embetter/error.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/external/_cohere.py` & `embetter-0.4.1/embetter/external/_cohere.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/external/_openai.py` & `embetter-0.4.1/embetter/external/_openai.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/finetune/_contrastive.py` & `embetter-0.4.1/embetter/finetune/_contrastive.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,19 +61,21 @@
 
 
 class ContrastiveNetwork(nn.Module):
     """
     Adapted from network from Figure 1: https://arxiv.org/pdf/1908.10084.pdf.
     """
 
-    def __init__(self, shape_in):
+    def __init__(self, shape_in, hidden_dim):
         super(ContrastiveNetwork, self).__init__()
         shape_out = 2
-        self.emb = nn.Linear(shape_in, shape_in)
-        self.fc = nn.Sequential(nn.Linear(shape_in, shape_out), nn.Sigmoid())
+        self.emb = nn.Linear(shape_in, hidden_dim)
+        # We multiply by three because we concat(u, v, |u - v|)
+        # it's what the paper does https://github.com/koaning/embetter/issues/67
+        self.fc = nn.Sequential(nn.Linear(hidden_dim * 3, shape_out), nn.Sigmoid())
 
     def init_weights(self, m):
         """Initlize the weights"""
         if isinstance(m, nn.Linear):
             torch.nn.init.xavier_uniform_(m.weight)
             m.bias.data.fill_(0.01)
 
@@ -81,28 +83,33 @@
         """Return the learned embedding"""
         return self.emb(input_mat)
 
     def forward(self, input1, input2):
         """Feed forward"""
         emb_1 = self.embed(input1)
         emb_2 = self.embed(input2)
-        return self.fc(torch.abs(emb_1 - emb_2))
+        out = torch.cat((emb_1, emb_2, torch.abs(emb_1 - emb_2)), dim=1)
+        return self.fc(out)
 
 
 class ContrastiveFinetuner(BaseEstimator, TransformerMixin):
     """
     Run a contrastive network to finetune the embeddings towards a class.
 
     Arguments:
+        hidden_dim: the dimension of the new learned representation
         n_neg: number of negative example pairs to sample per positive item
         n_epochs: number of epochs to use for training
         learning_rate: learning rate of the contrastive network
     """
 
-    def __init__(self, n_neg=3, n_epochs=20, learning_rate=0.001) -> None:
+    def __init__(
+        self, hidden_dim=50, n_neg=3, n_epochs=20, learning_rate=0.001
+    ) -> None:
+        self.hidden_dim = hidden_dim
         self.n_neg = n_neg
         self.n_epochs = n_epochs
         self.learning_rate = learning_rate
 
     def fit(self, X, y):
         """Fits the finetuner."""
         return self.partial_fit(X, y, classes=np.unique(y))
@@ -122,15 +129,17 @@
         """Fits the finetuner using the partial_fit API."""
         if not hasattr(self, "_classes"):
             if classes is None:
                 raise ValueError("`classes` must be provided for partial_fit")
             self._classes = classes
         # Create a model if it does not exist yet.
         if not hasattr(self, "_model"):
-            self._model = ContrastiveNetwork(shape_in=X.shape[1])
+            self._model = ContrastiveNetwork(
+                shape_in=X.shape[1], hidden_dim=self.hidden_dim
+            )
             self._optimizer = torch.optim.Adam(
                 self._model.parameters(), lr=self.learning_rate
             )
             self._criterion = nn.CrossEntropyLoss()
 
         X_torch = torch.from_numpy(X).detach().float()
```

### Comparing `embetter-0.4.0/embetter/finetune/_forward.py` & `embetter-0.4.1/embetter/finetune/_forward.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/grab.py` & `embetter-0.4.1/embetter/grab.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/multi/_clip.py` & `embetter-0.4.1/embetter/multi/_clip.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/text/__init__.py` & `embetter-0.4.1/embetter/text/__init__.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/text/_bpemb.py` & `embetter-0.4.1/embetter/text/_bpemb.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/text/_s2v.py` & `embetter-0.4.1/embetter/text/_s2v.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/text/_sbert.py` & `embetter-0.4.1/embetter/text/_sbert.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/text/_spacy.py` & `embetter-0.4.1/embetter/text/_spacy.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/vision/_colorhist.py` & `embetter-0.4.1/embetter/vision/_colorhist.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/vision/_loader.py` & `embetter-0.4.1/embetter/vision/_loader.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter/vision/_torchvis.py` & `embetter-0.4.1/embetter/vision/_torchvis.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/embetter.egg-info/PKG-INFO` & `embetter-0.4.1/embetter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embetter
-Version: 0.4.0
+Version: 0.4.1
 Summary: Just a bunch of useful embeddings to get started quickly.
 Home-page: https://koaning.github.io/embetter/
 Author: Vincent D. Warmerdam
 License: UNKNOWN
 Project-URL: Documentation, https://koaning.github.io/embetter/
 Project-URL: Source Code, https://github.com/koaning/embetter/
 Project-URL: Issue Tracker, https://github.com/koaning/embetter/issues
```

### Comparing `embetter-0.4.0/embetter.egg-info/SOURCES.txt` & `embetter-0.4.1/embetter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,9 @@
 embetter/vision/_torchvis.py
 tests/__init__.py
 tests/test_base.py
 tests/test_default.py
 tests/test_docs.py
 tests/test_finetuners.py
 tests/test_text.py
+tests/test_utils.py
 tests/test_vision.py
```

### Comparing `embetter-0.4.0/embetter.egg-info/requires.txt` & `embetter-0.4.1/embetter.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/setup.py` & `embetter-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 all_packages = base_packages + text_packages + vision_packages + openai_packages
 dev_packages = all_packages + docs_packages + test_packages
 
 
 setup(
     name="embetter",
-    version="0.4.0",
+    version="0.4.1",
     author="Vincent D. Warmerdam",
     packages=find_packages(exclude=["notebooks", "docs"]),
     description="Just a bunch of useful embeddings to get started quickly.",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     license_files=("LICENSE"),
     url="https://koaning.github.io/embetter/",
```

### Comparing `embetter-0.4.0/tests/test_docs.py` & `embetter-0.4.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/tests/test_text.py` & `embetter-0.4.1/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `embetter-0.4.0/tests/test_vision.py` & `embetter-0.4.1/tests/test_vision.py`

 * *Files identical despite different names*

