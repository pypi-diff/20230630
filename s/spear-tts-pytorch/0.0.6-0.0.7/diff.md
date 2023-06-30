# Comparing `tmp/spear-tts-pytorch-0.0.6.tar.gz` & `tmp/spear-tts-pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.6.tar", last modified: Thu Jun 29 20:59:23 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.7.tar", last modified: Fri Jun 30 16:03:46 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.6.tar` & `spear-tts-pytorch-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18624 2023-06-30 16:03:34.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 16:03:46.467204 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-30 16:03:46.000000 spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.6/LICENSE` & `spear-tts-pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.6/PKG-INFO` & `spear-tts-pytorch-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.6/README.md` & `spear-tts-pytorch-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,20 @@
 
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
 
 ## Todo
 
-- [ ] add eos logic + generate, and hook up end-to-end generation in soundstorm
+- [x] add eos logic + generate, and hook up end-to-end generation in soundstorm
+- [x] add first pretraining speech-to-speech with the reconstruction of 60% deleted tokens
+
 - [ ] add total flexiblity of which layers of encoder / decoder to freeze during training
-- [ ] add first pretraining speech-to-speech with the reconstruction of 60% deleted tokens
+- [ ] add step for training on small speech -> text corpus and generating pseudo-labelled dataset + finetuning
+- [ ] add final step of finetuning on text -> speech + pseudolabelled dataset
 - [ ] add dropouts for this project, as low-resource
 
 ## Citations
 
 ```bibtex
 @misc{kharitonov2023speak,
     title   = {Speak, Read and Prompt: High-Fidelity Text-to-Speech with Minimal Supervision},
```

#### html2text {}

```diff
@@ -1,15 +1,17 @@
 [./spear-tts.png] ## Spear-TTS - Pytorch (wip) Implementation of Spear-TTS -
 multi-speaker text-to-speech attention network, in Pytorch The text-to-semantic
 module built here will be used for SoundStorm for conditioning. ## Appreciation
 - Stability and ð¤_Huggingface for their generous sponsorships to work on and
-open source cutting edge artificial intelligence research ## Todo - [ ] add eos
-logic + generate, and hook up end-to-end generation in soundstorm - [ ] add
-total flexiblity of which layers of encoder / decoder to freeze during training
-- [ ] add first pretraining speech-to-speech with the reconstruction of 60%
-deleted tokens - [ ] add dropouts for this project, as low-resource ##
-Citations ```bibtex @misc{kharitonov2023speak, title = {Speak, Read and Prompt:
-High-Fidelity Text-to-Speech with Minimal Supervision}, author = {Eugene
-Kharitonov and Damien Vincent and ZalÃ¡n Borsos and RaphaÃ«l Marinier and
-Sertan Girgin and Olivier Pietquin and Matt Sharifi and Marco Tagliasacchi and
-Neil Zeghidour}, year = {2023}, eprint = {2302.03540}, archivePrefix = {arXiv},
-primaryClass = {cs.SD} } ```
+open source cutting edge artificial intelligence research ## Todo - [x] add eos
+logic + generate, and hook up end-to-end generation in soundstorm - [x] add
+first pretraining speech-to-speech with the reconstruction of 60% deleted
+tokens - [ ] add total flexiblity of which layers of encoder / decoder to
+freeze during training - [ ] add step for training on small speech -> text
+corpus and generating pseudo-labelled dataset + finetuning - [ ] add final step
+of finetuning on text -> speech + pseudolabelled dataset - [ ] add dropouts for
+this project, as low-resource ## Citations ```bibtex @misc{kharitonov2023speak,
+title = {Speak, Read and Prompt: High-Fidelity Text-to-Speech with Minimal
+Supervision}, author = {Eugene Kharitonov and Damien Vincent and ZalÃ¡n Borsos
+and RaphaÃ«l Marinier and Sertan Girgin and Olivier Pietquin and Matt Sharifi
+and Marco Tagliasacchi and Neil Zeghidour}, year = {2023}, eprint =
+{2302.03540}, archivePrefix = {arXiv}, primaryClass = {cs.SD} } ```
```

### Comparing `spear-tts-pytorch-0.0.6/setup.py` & `spear-tts-pytorch-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
```

### Comparing `spear-tts-pytorch-0.0.6/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.7/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,26 +291,31 @@
 # class
 
 SpeechOrTextLiteral = Union[
     Literal['speech'],
     Literal['text']
 ]
 
+SemanticModelType = Union[
+    FairseqVQWav2Vec,
+    HubertWithKmeans
+]
+
 class TextToSemantic(Module):
     @beartype
     def __init__(
         self,
         dim,
         *,
         num_text_token_ids,
         source_depth,
         target_depth,
         tokenizer_encode: Optional[Callable] = None,
         use_openai_tokenizer = False,
-        wav2vec: Optional[Union[FairseqVQWav2Vec, HubertWithKmeans]] = None,
+        wav2vec: Optional[SemanticModelType] = None,
         num_semantic_token_ids = None,
         dim_head = 64,
         heads = 8,
         semantic_pad_id = -1,
         text_pad_id = 0,
         autoset_semantic_eos_id = True,
         autoset_text_eos_id = True,
@@ -575,14 +580,78 @@
         logits = target_to_logit(target_emb)
 
         if not return_loss:
             return logits
 
         assert not empty(target)
 
+        logits = rearrange(logits[:, :-1], 'b n c -> b c n')
+
         loss = F.cross_entropy(
-            rearrange(logits[:, :-1], 'b n c -> b c n'),
+            logits,
             target,
             ignore_index = target_pad_id
         )
 
         return loss
+
+# pretraining modules
+
+def get_mask_subset_prob(mask, prob, min_mask = 0):
+    batch, seq, device = *mask.shape, mask.device
+    num_to_mask = (mask.sum(dim = -1, keepdim = True) * prob).clamp(min = min_mask)
+    logits = torch.rand((batch, seq), device = device)
+    logits = logits.masked_fill(~mask, -1)
+
+    randperm = logits.argsort(dim = -1).float()
+
+    num_padding = (~mask).sum(dim = -1, keepdim = True)
+    randperm -= num_padding
+
+    subset_mask = randperm < num_to_mask
+    subset_mask.masked_fill_(~mask, False)
+    return subset_mask
+
+class SpeechSpeechPretrainWrapper(nn.Module):
+    @beartype
+    def __init__(
+        self,
+        model: TextToSemantic,
+        wav2vec: Optional[SemanticModelType] = None,
+        deletion_prob: float = 0.6
+    ):
+        super().__init__()
+
+        self.model = model
+        self.wav2vec = default(wav2vec, model.wav2vec)
+        assert exists(self.wav2vec)
+
+        self.deletion_prob = deletion_prob
+
+    def forward(
+        self,
+        x
+    ):
+        is_raw_audio = x.dtype == torch.float
+
+        if is_raw_audio:
+            with torch.no_grad():
+                self.wav2vec.eval()
+                x = self.wav2vec(x, flatten = False)
+
+        batch = x.shape[0]
+
+        mask = torch.ones_like(x, dtype = torch.bool, device = self.model.device)
+
+        delete_mask = get_mask_subset_prob(mask, self.deletion_prob)
+
+        source = rearrange(x[~delete_mask], '(b n) -> b n', b = batch)
+        target = rearrange(x[delete_mask], '(b n) -> b n', b = batch)
+
+        loss = self.model(
+            source, target,
+            source_type = 'speech',
+            target_type = 'speech',
+            return_loss = True
+        )
+
+        return loss
```

### Comparing `spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.7/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

