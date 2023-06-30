# Comparing `tmp/product_key_memory-0.2.7.tar.gz` & `tmp/product_key_memory-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "product_key_memory-0.2.7.tar", last modified: Wed Jun 28 22:43:09 2023, max compression
+gzip compressed data, was "product_key_memory-0.2.8.tar", last modified: Fri Jun 30 21:49:37 2023, max compression
```

## Comparing `product_key_memory-0.2.7.tar` & `product_key_memory-0.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:43:09.504057 product_key_memory-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-28 22:42:57.000000 product_key_memory-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-28 22:43:09.504057 product_key_memory-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-28 22:42:57.000000 product_key_memory-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:43:09.504057 product_key_memory-0.2.7/product_key_memory/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-28 22:42:57.000000 product_key_memory-0.2.7/product_key_memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-06-28 22:42:57.000000 product_key_memory-0.2.7/product_key_memory/product_key_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 22:43:09.504057 product_key_memory-0.2.7/product_key_memory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-28 22:43:09.000000 product_key_memory-0.2.7/product_key_memory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-28 22:43:09.000000 product_key_memory-0.2.7/product_key_memory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 22:43:09.000000 product_key_memory-0.2.7/product_key_memory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 22:43:09.000000 product_key_memory-0.2.7/product_key_memory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-28 22:43:09.000000 product_key_memory-0.2.7/product_key_memory.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 22:43:09.504057 product_key_memory-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-28 22:42:57.000000 product_key_memory-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/product_key_memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/product_key_memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/product_key_memory/product_key_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/product_key_memory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 21:49:37.000000 product_key_memory-0.2.8/product_key_memory.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 21:49:37.983594 product_key_memory-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-30 21:49:28.000000 product_key_memory-0.2.8/setup.py
```

### Comparing `product_key_memory-0.2.7/LICENSE` & `product_key_memory-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `product_key_memory-0.2.7/PKG-INFO` & `product_key_memory-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product_key_memory
-Version: 0.2.7
+Version: 0.2.8
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.7/README.md` & `product_key_memory-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 ## Appreciation
 
 Special thanks go to <a href="https://github.com/AranKomat">Aran</a> for encouraging me to look into this, and to <a href="https://github.com/madisonmay">Madison May</a> for his <a href="https://www.pragmatic.ml/large-memory-layers-with-product-keys/">educational blog post</a>, which helped me understand this better.
 
 ## Todo
 
 - [x] offer stochasticity with annealed gumbel noise. seen dramatic effects in vector-quantization setting
+- [x] offer a way for smaller value dimensions + concat and linear combination of heads (like multi-head attention)
 
 - [ ] get caught up on latest literature on product key memories, if any
-- [ ] offer a way for smaller value dimensions + concat and linear combination of heads (like multi-head attention)
 - [ ] instead of additive scores, try multiplicative using coordinate descent routing
 
 ## Citations
 
 ```bibtex
 @misc{lample2019large,
     title   = {Large Memory Layers with Product Keys},
```

#### html2text {}

```diff
@@ -19,18 +19,18 @@
 import Adam from product_key_memory import fetch_optimizer_parameters
 parameters = fetch_optimizer_parameters(model) # automatically creates array of
 parameter settings with learning rate set at 1e-2 for pkm values optim = Adam
 (parameters, lr=1e-3) ``` ## Appreciation Special thanks go to Aran for
 encouraging me to look into this, and to Madison_May for his educational_blog
 post, which helped me understand this better. ## Todo - [x] offer stochasticity
 with annealed gumbel noise. seen dramatic effects in vector-quantization
-setting - [ ] get caught up on latest literature on product key memories, if
-any - [ ] offer a way for smaller value dimensions + concat and linear
-combination of heads (like multi-head attention) - [ ] instead of additive
-scores, try multiplicative using coordinate descent routing ## Citations
-```bibtex @misc{lample2019large, title = {Large Memory Layers with Product
-Keys}, author = {Guillaume Lample and Alexandre Sablayrolles and Marc'Aurelio
-Ranzato and Ludovic Denoyer and HervÃ© JÃ©gou}, year = {2019}, eprint =
-{1907.05242}, archivePrefix = {arXiv} } ``` ```bibtex @misc{liu2020evolving,
-title = {Evolving Normalization-Activation Layers}, author = {Hanxiao Liu and
-Andrew Brock and Karen Simonyan and Quoc V. Le}, year = {2020}, eprint =
-{2004.02967}, archivePrefix = {arXiv} } ```
+setting - [x] offer a way for smaller value dimensions + concat and linear
+combination of heads (like multi-head attention) - [ ] get caught up on latest
+literature on product key memories, if any - [ ] instead of additive scores,
+try multiplicative using coordinate descent routing ## Citations ```bibtex
+@misc{lample2019large, title = {Large Memory Layers with Product Keys}, author
+= {Guillaume Lample and Alexandre Sablayrolles and Marc'Aurelio Ranzato and
+Ludovic Denoyer and HervÃ© JÃ©gou}, year = {2019}, eprint = {1907.05242},
+archivePrefix = {arXiv} } ``` ```bibtex @misc{liu2020evolving, title =
+{Evolving Normalization-Activation Layers}, author = {Hanxiao Liu and Andrew
+Brock and Karen Simonyan and Quoc V. Le}, year = {2020}, eprint = {2004.02967},
+archivePrefix = {arXiv} } ```
```

### Comparing `product_key_memory-0.2.7/product_key_memory/product_key_memory.py` & `product_key_memory-0.2.8/product_key_memory/product_key_memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import math
 import torch
 from torch import nn, einsum
 
 from einops import rearrange
+from einops.layers.torch import Rearrange, Reduce
 
 from colt5_attention import topk as coor_descent_topk
 
 # helper functions
 
 def exists(val):
     return val is not None
@@ -79,15 +80,16 @@
         dim_head = 128,
         input_dropout = 0.,
         query_dropout = 0.,
         value_dropout = 0.,
         attn_dropout = 0.,
         use_layernorm = True,
         pre_layernorm = False,
-        differentiable_topk = False
+        differentiable_topk = False,
+        concat_values_and_combine = False
     ):
         super().__init__()
         self.topk = topk
         self.heads = heads
         self.num_keys = num_keys
 
         dim_query = dim_head * heads * 2
@@ -102,18 +104,40 @@
         self.use_layernorm = use_layernorm
 
         if use_layernorm:
             self.norm = nn.LayerNorm(dim_head)
         else:
             self.norm = MaskedBatchNorm1D(nn.BatchNorm1d(dim_head))
 
+        # keys
+
         self.keys = nn.Parameter(torch.zeros(heads, num_keys, 2, dim_head))
-        self.values = nn.EmbeddingBag(num_keys ** 2, dim, mode = 'sum')
         init_(self.keys)
-        init_(self.values.weight)
+
+        # values
+
+        self.concat_values_and_combine = concat_values_and_combine
+
+        if concat_values_and_combine:
+            values = nn.Embedding(num_keys ** 2, dim_head)
+
+            self.values = nn.Sequential(
+                values,
+                Reduce('b (h k) d -> b h d', 'sum', h = heads),
+                Rearrange('b n d -> b (n d)'),
+                nn.Linear(dim_head * heads, dim, bias = False)
+            )
+        else:
+            values = nn.EmbeddingBag(num_keys ** 2, dim, mode = 'sum')
+            self.values = values
+
+
+        init_(values.weight)
+
+        # dropouts
 
         self.input_dropout = nn.Dropout(input_dropout)
         self.query_dropout = nn.Dropout(query_dropout)
         self.value_dropout = nn.Dropout(value_dropout)
         self.attn_dropout = nn.Dropout(attn_dropout)
 
         # use a differentiable topk, based on coordinate descent
@@ -188,11 +212,14 @@
         attn = final_topk.softmax(dim=-1)
         attn = self.attn_dropout(attn)
 
         value_indices, attn = map(lambda t: rearrange(t, 'b t h k -> (b t) (h k)'), (value_indices, attn))
 
         # aggregate
 
-        out = self.values(value_indices, per_sample_weights=attn)
-        out = self.value_dropout(out)
+        if self.concat_values_and_combine:
+            out = self.values(value_indices)
+        else:
+            out = self.values(value_indices, per_sample_weights = attn)
 
+        out = self.value_dropout(out)
         return rearrange(out, '(b t) d -> b t d', b = b)
```

### Comparing `product_key_memory-0.2.7/product_key_memory.egg-info/PKG-INFO` & `product_key_memory-0.2.8/product_key_memory.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: product-key-memory
-Version: 0.2.7
+Version: 0.2.8
 Summary: Product Key Memory
 Home-page: https://github.com/lucidrains/product-key-memory
 Author: Aran Komatsuzaki, Phil Wang
 Author-email: aran1234321@gmail.com, lucidrains@gmail.com
 License: MIT
 Keywords: transformers,artificial intelligence
 Classifier: Development Status :: 4 - Beta
```

### Comparing `product_key_memory-0.2.7/setup.py` & `product_key_memory-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'product_key_memory',
     packages = find_packages(),
-    version = '0.2.7',
+    version = '0.2.8',
     license = 'MIT',
     description = 'Product Key Memory',
     long_description_content_type = 'text/markdown',
     author = 'Aran Komatsuzaki, Phil Wang',
     author_email = 'aran1234321@gmail.com, lucidrains@gmail.com',
     url = 'https://github.com/lucidrains/product-key-memory',
     keywords = [
```

