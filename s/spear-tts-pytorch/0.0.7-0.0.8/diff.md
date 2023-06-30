# Comparing `tmp/spear-tts-pytorch-0.0.7.tar.gz` & `tmp/spear-tts-pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.7.tar", last modified: Fri Jun 30 16:03:46 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.8.tar", last modified: Fri Jun 30 17:13:52 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.7.tar` & `spear-tts-pytorch-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.911023 spear-tts-pytorch-0.0.8/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-06-30 17:13:43.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 17:13:52.915023 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 17:13:52.000000 spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.7/LICENSE` & `spear-tts-pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.7/PKG-INFO` & `spear-tts-pytorch-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.7/README.md` & `spear-tts-pytorch-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
 
 ## Todo
 
 - [x] add eos logic + generate, and hook up end-to-end generation in soundstorm
 - [x] add first pretraining speech-to-speech with the reconstruction of 60% deleted tokens
+- [x] add dropouts for this project, as low-resource
 
 - [ ] add total flexiblity of which layers of encoder / decoder to freeze during training
 - [ ] add step for training on small speech -> text corpus and generating pseudo-labelled dataset + finetuning
 - [ ] add final step of finetuning on text -> speech + pseudolabelled dataset
-- [ ] add dropouts for this project, as low-resource
 
 ## Citations
 
 ```bibtex
 @misc{kharitonov2023speak,
     title   = {Speak, Read and Prompt: High-Fidelity Text-to-Speech with Minimal Supervision}, 
     author  = {Eugene Kharitonov and Damien Vincent and Zalán Borsos and Raphaël Marinier and Sertan Girgin and Olivier Pietquin and Matt Sharifi and Marco Tagliasacchi and Neil Zeghidour},
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 [./spear-tts.png] ## Spear-TTS - Pytorch (wip) Implementation of Spear-TTS -
 multi-speaker text-to-speech attention network, in Pytorch The text-to-semantic
 module built here will be used for SoundStorm for conditioning. ## Appreciation
 - Stability and ð¤_Huggingface for their generous sponsorships to work on and
 open source cutting edge artificial intelligence research ## Todo - [x] add eos
 logic + generate, and hook up end-to-end generation in soundstorm - [x] add
 first pretraining speech-to-speech with the reconstruction of 60% deleted
-tokens - [ ] add total flexiblity of which layers of encoder / decoder to
-freeze during training - [ ] add step for training on small speech -> text
-corpus and generating pseudo-labelled dataset + finetuning - [ ] add final step
-of finetuning on text -> speech + pseudolabelled dataset - [ ] add dropouts for
-this project, as low-resource ## Citations ```bibtex @misc{kharitonov2023speak,
-title = {Speak, Read and Prompt: High-Fidelity Text-to-Speech with Minimal
-Supervision}, author = {Eugene Kharitonov and Damien Vincent and ZalÃ¡n Borsos
-and RaphaÃ«l Marinier and Sertan Girgin and Olivier Pietquin and Matt Sharifi
-and Marco Tagliasacchi and Neil Zeghidour}, year = {2023}, eprint =
-{2302.03540}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ```
+tokens - [x] add dropouts for this project, as low-resource - [ ] add total
+flexiblity of which layers of encoder / decoder to freeze during training - [ ]
+add step for training on small speech -> text corpus and generating pseudo-
+labelled dataset + finetuning - [ ] add final step of finetuning on text -
+> speech + pseudolabelled dataset ## Citations ```bibtex @misc
+{kharitonov2023speak, title = {Speak, Read and Prompt: High-Fidelity Text-to-
+Speech with Minimal Supervision}, author = {Eugene Kharitonov and Damien
+Vincent and ZalÃ¡n Borsos and RaphaÃ«l Marinier and Sertan Girgin and Olivier
+Pietquin and Matt Sharifi and Marco Tagliasacchi and Neil Zeghidour}, year =
+{2023}, eprint = {2302.03540}, archivePrefix = {arXiv}, primaryClass = {cs.SD}
+} ```
```

### Comparing `spear-tts-pytorch-0.0.7/setup.py` & `spear-tts-pytorch-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
```

### Comparing `spear-tts-pytorch-0.0.7/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.8/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,42 +157,45 @@
 # feedforward
 
 class GEGLU(nn.Module):
     def forward(self, x):
         x, gate = x.chunk(2, dim = -1)
         return F.gelu(gate) * x
 
-def FeedForward(dim, mult = 4):
+def FeedForward(dim, mult = 4, dropout = 0.):
     dim_inner = int(dim * mult * 2 / 3)
     return nn.Sequential(
         RMSNorm(dim),
         nn.Linear(dim, dim_inner * 2),
         GEGLU(),
+        nn.Dropout(dropout),
         nn.Linear(dim_inner, dim)
     )
 
 # attention
 
 class Attention(nn.Module):
     def __init__(
         self,
         dim,
         *,
         dim_head = 64,
         heads = 8,
-        causal = False
+        causal = False,
+        dropout = 0.
     ):
         super().__init__()
         self.heads = heads
         self.scale = dim_head ** -0.5
         dim_inner = heads * dim_head
 
         self.causal = causal
 
         self.norm = RMSNorm(dim)
+        self.attn_dropout = nn.Dropout(dropout)
 
         self.to_q = nn.Linear(dim, dim_inner, bias = False)
         self.to_kv = nn.Linear(dim, dim_inner * 2, bias = False)
         self.to_out = nn.Linear(dim_inner, dim, bias = False)
 
     def forward(
         self,
@@ -222,14 +225,15 @@
 
         if self.causal:
             i, j = sim.shape[-2:]
             causal_mask = torch.ones((i, j), device = x.device, dtype = torch.bool).triu(j - i + 1)
             sim = sim.masked_fill(causal_mask, -torch.finfo(sim.dtype).max)
 
         attn = sim.softmax(dim = -1)
+        attn = self.attn_dropout(attn)
 
         out = einsum('b h i j, b h j d -> b h i d', attn, v)
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # transformer
@@ -239,32 +243,34 @@
         self,
         *,
         dim,
         depth,
         dim_head = 64,
         heads = 8,
         causal = False,
+        attn_dropout = 0.,
         ff_mult = 4,
+        ff_dropout = 0.,
         cross_attend = False
     ):
         super().__init__()
 
         self.rel_pos_bias = RelativePositionBias(
             scale = dim_head ** 0.5,
             causal = causal,
             heads = heads
         )
 
         self.layers = nn.ModuleList([])
 
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                Attention(dim = dim, causal = causal, dim_head = dim_head, heads = heads),
-                Attention(dim = dim, dim_head = dim_head, heads = heads) if cross_attend else None,
-                FeedForward(dim = dim, mult = ff_mult)
+                Attention(dim = dim, causal = causal, dim_head = dim_head, heads = heads, dropout = attn_dropout),
+                Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout) if cross_attend else None,
+                FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
         self.final_norm = RMSNorm(dim)
 
     def forward(
         self,
         x,
@@ -311,14 +317,16 @@
         target_depth,
         tokenizer_encode: Optional[Callable] = None,
         use_openai_tokenizer = False,
         wav2vec: Optional[SemanticModelType] = None,
         num_semantic_token_ids = None,
         dim_head = 64,
         heads = 8,
+        attn_dropout = 0.,
+        ff_dropout = 0.,
         semantic_pad_id = -1,
         text_pad_id = 0,
         autoset_semantic_eos_id = True,
         autoset_text_eos_id = True,
     ):
         super().__init__()
         self.dim = dim
@@ -392,22 +400,26 @@
         # source and target attention layers
 
         self.source_transformer = Transformer(
             dim = dim,
             dim_head = dim_head,
             heads = heads,
             depth = source_depth,
+            attn_dropout = attn_dropout,
+            ff_dropout = ff_dropout,
             causal = False
         )
 
         self.target_transformer = Transformer(
             dim = dim,
             dim_head = dim_head,
             heads = heads,
             depth = source_depth,
+            attn_dropout = attn_dropout,
+            ff_dropout = ff_dropout,
             causal = True,
             cross_attend = True
         )
 
     def load(self, path, strict = True):
         path = Path(path)
         assert path.exists()
```

### Comparing `spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.8/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

