# Comparing `tmp/yoyodyne-0.2.1.tar.gz` & `tmp/yoyodyne-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yoyodyne-0.2.1.tar", last modified: Mon Dec  5 14:55:31 2022, max compression
+gzip compressed data, was "yoyodyne-0.2.3.tar", last modified: Fri Jun 30 17:21:28 2023, max compression
```

## Comparing `yoyodyne-0.2.1.tar` & `yoyodyne-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2022-12-05 14:55:31.752532 yoyodyne-0.2.1/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    10814 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/LICENSE.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6333 2022-12-05 14:55:31.749534 yoyodyne-0.2.1/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     5629 2022-12-05 14:49:05.000000 yoyodyne-0.2.1/README.md
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       38 2022-12-05 14:55:31.753532 yoyodyne-0.2.1/setup.cfg
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     2072 2022-12-05 14:36:05.000000 yoyodyne-0.2.1/setup.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2022-12-05 14:55:31.298370 yoyodyne-0.2.1/yoyodyne/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6451 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/collators.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    21599 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/datasets.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3860 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/evaluators.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2022-12-05 14:55:31.723262 yoyodyne-0.2.1/yoyodyne/models/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1587 2022-12-05 14:34:34.000000 yoyodyne-0.2.1/yoyodyne/models/__init__.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     3465 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/attention.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     9489 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/base.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    16156 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/expert.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1825 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/generation_probability.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    19769 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/lstm.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    18948 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/pointer_generator.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     2139 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/positional_encoding.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    24772 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/models/transducer.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    14080 2022-12-05 14:34:34.000000 yoyodyne-0.2.1/yoyodyne/models/transformer.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     7659 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/predict.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     1751 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/schedulers.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      155 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/special.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)    15243 2022-12-05 14:34:34.000000 yoyodyne-0.2.1/yoyodyne/train.py
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      929 2022-12-05 14:34:35.000000 yoyodyne-0.2.1/yoyodyne/util.py
-drwxrwxrwx   0 kbg       (1000) kbg       (1000)        0 2022-12-05 14:55:31.431444 yoyodyne-0.2.1/yoyodyne.egg-info/
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)     6333 2022-12-05 14:55:30.000000 yoyodyne-0.2.1/yoyodyne.egg-info/PKG-INFO
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      719 2022-12-05 14:55:31.000000 yoyodyne-0.2.1/yoyodyne.egg-info/SOURCES.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        1 2022-12-05 14:55:30.000000 yoyodyne-0.2.1/yoyodyne.egg-info/dependency_links.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)       96 2022-12-05 14:55:30.000000 yoyodyne-0.2.1/yoyodyne.egg-info/entry_points.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)      105 2022-12-05 14:55:30.000000 yoyodyne-0.2.1/yoyodyne.egg-info/requires.txt
--rwxrwxrwx   0 kbg       (1000) kbg       (1000)        9 2022-12-05 14:55:30.000000 yoyodyne-0.2.1/yoyodyne.egg-info/top_level.txt
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-06-30 17:21:28.530934 yoyodyne-0.2.3/
+-rw-r--r--   0 kbg        (501) staff       (20)    10814 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/LICENSE.txt
+-rw-r--r--   0 kbg        (501) staff       (20)    10736 2023-06-30 17:21:28.530782 yoyodyne-0.2.3/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)     9976 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/README.md
+-rw-r--r--   0 kbg        (501) staff       (20)     1277 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/pyproject.toml
+-rw-r--r--   0 kbg        (501) staff       (20)       38 2023-06-30 17:21:28.530966 yoyodyne-0.2.3/setup.cfg
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-06-30 17:21:28.528509 yoyodyne-0.2.3/yoyodyne/
+-rw-r--r--   0 kbg        (501) staff       (20)      289 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/__init__.py
+-rw-r--r--   0 kbg        (501) staff       (20)     3495 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/batches.py
+-rw-r--r--   0 kbg        (501) staff       (20)     6175 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/collators.py
+-rw-r--r--   0 kbg        (501) staff       (20)     8394 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/yoyodyne/dataconfig.py
+-rw-r--r--   0 kbg        (501) staff       (20)    11930 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/datasets.py
+-rw-r--r--   0 kbg        (501) staff       (20)      737 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/yoyodyne/defaults.py
+-rw-r--r--   0 kbg        (501) staff       (20)     3906 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/evaluators.py
+-rw-r--r--   0 kbg        (501) staff       (20)     4281 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/indexes.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-06-30 17:21:28.530620 yoyodyne-0.2.3/yoyodyne/models/
+-rw-r--r--   0 kbg        (501) staff       (20)     2505 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/models/__init__.py
+-rw-r--r--   0 kbg        (501) staff       (20)     3305 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/models/attention.py
+-rw-r--r--   0 kbg        (501) staff       (20)    15032 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/yoyodyne/models/base.py
+-rw-r--r--   0 kbg        (501) staff       (20)    17071 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/models/expert.py
+-rw-r--r--   0 kbg        (501) staff       (20)     1931 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/models/generation_probability.py
+-rw-r--r--   0 kbg        (501) staff       (20)    18831 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/models/lstm.py
+-rw-r--r--   0 kbg        (501) staff       (20)    21816 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/models/pointer_generator.py
+-rw-r--r--   0 kbg        (501) staff       (20)     2277 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/models/positional_encoding.py
+-rw-r--r--   0 kbg        (501) staff       (20)    24209 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/models/transducer.py
+-rw-r--r--   0 kbg        (501) staff       (20)    13107 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/models/transformer.py
+-rw-r--r--   0 kbg        (501) staff       (20)     6137 2023-06-28 17:23:07.000000 yoyodyne-0.2.3/yoyodyne/predict.py
+-rw-r--r--   0 kbg        (501) staff       (20)     4566 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/schedulers.py
+-rw-r--r--   0 kbg        (501) staff       (20)      169 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/special.py
+-rw-r--r--   0 kbg        (501) staff       (20)    14313 2023-06-30 17:20:26.000000 yoyodyne-0.2.3/yoyodyne/train.py
+-rw-r--r--   0 kbg        (501) staff       (20)      599 2023-05-09 13:12:52.000000 yoyodyne-0.2.3/yoyodyne/util.py
+drwxr-xr-x   0 kbg        (501) staff       (20)        0 2023-06-30 17:21:28.529240 yoyodyne-0.2.3/yoyodyne.egg-info/
+-rw-r--r--   0 kbg        (501) staff       (20)    10736 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/PKG-INFO
+-rw-r--r--   0 kbg        (501) staff       (20)      809 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/SOURCES.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        1 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/dependency_links.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       96 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/entry_points.txt
+-rw-r--r--   0 kbg        (501) staff       (20)       82 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/requires.txt
+-rw-r--r--   0 kbg        (501) staff       (20)        9 2023-06-30 17:21:28.000000 yoyodyne-0.2.3/yoyodyne.egg-info/top_level.txt
```

### Comparing `yoyodyne-0.2.1/LICENSE.txt` & `yoyodyne-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yoyodyne-0.2.1/yoyodyne/evaluators.py` & `yoyodyne-0.2.3/yoyodyne/evaluators.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,113 +7,107 @@
 class Error(Exception):
     pass
 
 
 class Evaluator:
     """Evaluates predictions."""
 
-    device: torch.device
-
-    def __init__(self, device):
-        """Initizalizes the evaluator.
-
-        Args:
-            device (torch.device).
-        """
-        self.device = device
-
     def val_accuracy(
         self,
-        preds: torch.Tensor,
+        predictions: torch.Tensor,
         golds: torch.Tensor,
         end_idx: int,
         pad_idx: int,
     ) -> float:
         """Computes the exact word match accuracy.
 
         Args:
-            preds (torch.Tensor): B x vocab_size x seq_len.
+            predictions (torch.Tensor): B x vocab_size x seq_len.
             golds (torch.Tensor): B x seq_len x 1.
             end_idx (int): end of sequence index.
             pad_idx (int): padding index.
 
         Returns:
             float: exact accuracy.
         """
-        if preds.size(0) != golds.size(0):
+        if predictions.size(0) != golds.size(0):
             raise Error(
-                "Preds batch size ({preds.size(0)}) and golds batch size "
-                "({golds.size(0)} do not match"
+                "Preds batch size ({predictions.size(0)}) and "
+                "golds batch size ({golds.size(0)} do not match"
             )
-        # -> B x seq_len x vocab_size.
-        preds = preds.transpose(1, 2)
-        # Gets the max val at each dim2 in preds.
-        vals, preds = torch.max(preds, dim=2)
-        # Finalizes the preds.
-        preds = self.finalize_preds(preds, end_idx, pad_idx, self.device)
-        return self.get_accuracy(preds, golds, pad_idx)
+        # Gets the max val at each dim2 in predictions.
+        vals, predictions = torch.max(predictions, dim=2)
+        # Finalizes the predictions.
+        predictions = self.finalize_predictions(predictions, end_idx, pad_idx)
+        return self.accuracy(predictions, golds, pad_idx)
 
     @staticmethod
-    def get_accuracy(
-        preds: torch.Tensor,
+    def accuracy(
+        predictions: torch.Tensor,
         golds: torch.Tensor,
         pad_idx: int,
     ) -> float:
-        if preds.size(1) > golds.size(1):
-            preds = preds[:, : golds.size(1)]
-        elif preds.size(1) < golds.size(1):
-            num_pads = (0, golds.size(1) - preds.size(1))
-            preds = functional.pad(preds, num_pads, "constant", pad_idx)
+        if predictions.size(1) > golds.size(1):
+            predictions = predictions[:, : golds.size(1)]
+        elif predictions.size(1) < golds.size(1):
+            num_pads = (0, golds.size(1) - predictions.size(1))
+            predictions = functional.pad(
+                predictions, num_pads, "constant", pad_idx
+            )
         # Gets the count of exactly matching tensors in the batch.
-        # -> B x max_seq_len
-        corr_count = torch.where((preds == golds).all(dim=1))[0].size()[0]
+        # -> B x max_seq_len.
+        corr_count = torch.where(
+            (predictions.to(golds.device) == golds).all(dim=1)
+        )[0].size()[0]
         # Gets the batch size (total_count).
-        total_count = preds.size(0)
+        total_count = predictions.size(0)
         return corr_count / total_count
 
     @staticmethod
-    def finalize_preds(
-        preds: torch.Tensor,
+    def finalize_predictions(
+        predictions: torch.Tensor,
         end_idx: int,
         pad_idx: int,
-        device: torch.device,
     ) -> torch.Tensor:
         """Finalizes predictions.
 
         Cuts off tensors at the first end_idx, and replaces the rest of the
         predictions with pad_idx, as these are erroneously decoded while the
         rest of the batch is finishing decoding.
 
         Args:
-            preds (torch.Tensor): prediction tensor.
+            predictions (torch.Tensor): prediction tensor.
             end_idx (int).
             pad_idx (int).
-            device (torch.device).
 
         Returns:
             torch.Tensor: finalized predictions.
         """
         # Not necessary if batch size is 1.
-        if preds.size(0) == 1:
-            return preds
-        for i, x in enumerate(preds):
+        if predictions.size(0) == 1:
+            return predictions
+        for i, x in enumerate(predictions):
             assert len(x.size()) == 1
             # Gets first instance of EOS.
             EOS = (x == end_idx).nonzero(as_tuple=False)
             if len(EOS) > 0 and EOS[0].item() < len(x):
                 # If an EOS was decoded and it is not the last one in the
                 # sequence.
                 EOS = EOS[0]
             else:
-                # Leaves preds[i] alone.
+                # Leaves predictions[i] alone.
                 continue
             # Hack in case the first prediction is EOS. In this case,
             # torch.split will result in an error, so we change these 0's to
             # 1's, which will make the entire sequence EOS as intended.
             EOS[EOS == 0] = 1
-            chars, *extras = torch.split(x, EOS)
+            chars, *_ = torch.split(x, EOS)
             # Replaces everything after with PAD, to replace erroneous decoding
             # While waiting on the entire batch to finish.
-            pads = torch.ones(len(x) - len(chars), device=device) * pad_idx
+            pads = (
+                torch.ones(len(x) - len(chars), device=chars.device) * pad_idx
+            )
             pads[0] = end_idx
-            preds[i] = torch.cat((chars, pads))
-        return preds
+            # Making an in-place udpate to an inference tensor.
+            with torch.inference_mode():
+                predictions[i] = torch.cat((chars, pads))
+        return predictions
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/__init__.py` & `yoyodyne-0.2.3/yoyodyne/models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,94 @@
 """Model classes and lookup function."""
 
-import pytorch_lightning as pl
+import argparse
 
 from .. import util
-from .lstm import LSTMEncoderDecoder, LSTMEncoderDecoderAttention
+from .base import BaseEncoderDecoder
+from .lstm import AttentiveLSTMEncoderDecoder, LSTMEncoderDecoder
 from .pointer_generator import (
     PointerGeneratorLSTMEncoderDecoderFeatures,
     PointerGeneratorLSTMEncoderDecoderNoFeatures,
 )
 from .transducer import TransducerFeatures, TransducerNoFeatures
 from .transformer import (
     FeatureInvariantTransformerEncoderDecoder,
     TransformerEncoderDecoder,
 )
 
 
-def get_model_cls(
-    arch: str, attn: str, include_features: bool
-) -> pl.LightningModule:
+def get_model_cls(arch: str, has_features: bool) -> BaseEncoderDecoder:
     """Model factory.
 
     Args:
         arch (str).
-        attn (str).
-        include_features (bool).
+        has_features (bool).
 
     Raises:
         NotImplementedError.
 
     Returns:
-        pl.LightningModule.
+        BaseEncoderDecoder.
     """
     model_fac = {
+        "attentive_lstm": AttentiveLSTMEncoderDecoder,
+        "lstm": LSTMEncoderDecoder,
+        "transducer": TransducerFeatures
+        if has_features
+        else TransducerNoFeatures,
+        "transformer": TransformerEncoderDecoder,
         # fmt: off
         "feature_invariant_transformer":
             FeatureInvariantTransformerEncoderDecoder,
         "pointer_generator_lstm":
             PointerGeneratorLSTMEncoderDecoderFeatures
-            if include_features
+            if has_features
             else PointerGeneratorLSTMEncoderDecoderNoFeatures,
         # fmt: on
-        "transducer": TransducerFeatures
-        if include_features
-        else TransducerNoFeatures,
-        "transformer": TransformerEncoderDecoder,
-        "lstm": LSTMEncoderDecoderAttention if attn else LSTMEncoderDecoder,
     }
-    if arch in ["lstm", "pointer_generator_lstm", "transformer"]:
-        util.log_info(f"Attention: {attn}")
     try:
-        kls = model_fac[arch]
-        return kls
+        model_cls = model_fac[arch]
+        util.log_info(f"Model: {model_cls.__name__}")
+        return model_cls
     except KeyError:
         raise NotImplementedError(f"Architecture {arch} not found")
+
+
+def get_model_cls_from_argparse_args(
+    args: argparse.Namespace,
+) -> BaseEncoderDecoder:
+    """Creates a model from CLI arguments.
+
+    Args:
+        args (argparse.Namespace).
+
+    Raises:
+        NotImplementedError.
+
+    Returns:
+        BaseEncoderDecoder.
+    """
+    return get_model_cls(args.arch, args.features_col != 0)
+
+
+def add_argparse_args(parser: argparse.ArgumentParser) -> None:
+    """Adds model options to an argument parser.
+
+    We only add the ones needed to look up the model class itself, with
+    more specific arguments specified in ../train.py.
+
+    Args:
+        parser (argparse.ArgumentParser).
+    """
+    parser.add_argument(
+        "--arch",
+        choices=[
+            "attentive_lstm",
+            "feature_invariant_transformer",
+            "lstm",
+            "pointer_generator_lstm",
+            "transducer",
+            "transformer",
+        ],
+        default="attentive_lstm",
+        help="Model architecture to use",
+    )
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/attention.py` & `yoyodyne-0.2.3/yoyodyne/models/attention.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Attention module class."""
 
+import math
 from typing import Tuple
 
 import torch
 from torch import nn
 
 
 class Attention(nn.Module):
@@ -12,34 +13,29 @@
     After:
         Luong, M.-T., Pham, H., and Manning, C. D. 2015. Effective
         approaches to attention-based neural machine translation. In
         Proceedings of the 2015 Conference on Empirical Methods in
         Natural Language Processing, pages 1412-1421.
     """
 
-    encoder_outputs_size: int
     hidden_size: int
     M: nn.Linear
     V: nn.Linear
 
     def __init__(self, encoder_outputs_size, hidden_size):
         """Initializes the attention module.
 
         Args:
             encoder_outputs_size (int).
             hidden_size (int).
         """
-        super(Attention, self).__init__()
-        self.encoder_outputs_size = encoder_outputs_size
-        self.hidden_size = hidden_size
+        super().__init__()
         # MLP to run over encoder_outputs.
-        self.M = nn.Linear(
-            self.encoder_outputs_size + self.hidden_size, self.hidden_size
-        )
-        self.V = nn.Linear(self.hidden_size, 1)
+        self.M = nn.Linear(encoder_outputs_size + hidden_size, hidden_size)
+        self.V = nn.Linear(hidden_size, 1)
 
     def forward(
         self,
         hidden: torch.Tensor,
         encoder_outputs: torch.Tensor,
         mask: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
@@ -59,20 +55,20 @@
         """
         # Gets last hidden layer.
         hidden = hidden[:, -1, :].unsqueeze(1)
         # Repeats hidden to be copied for each encoder output of shape
         # B  x seq_len x decoder_dim.
         hidden = hidden.repeat(1, encoder_outputs.size(1), 1)
         # Gets the scores of each time step in the output.
-        attn_scores = self.score(hidden, encoder_outputs)
+        attention_scores = self.score(hidden, encoder_outputs)
         # Masks the scores with -inf at each padded character so that softmax
         # computes a 0 towards the distribution for that cell.
-        attn_scores.data.masked_fill_(mask, -float("inf"))
+        attention_scores.data.masked_fill_(mask, -math.inf)
         # -> B x 1 x seq_len
-        weights = nn.functional.softmax(attn_scores, dim=1).unsqueeze(1)
+        weights = nn.functional.softmax(attention_scores, dim=1).unsqueeze(1)
         # -> B x 1 x decoder_dim
         weighted = torch.bmm(weights, encoder_outputs)
         return weighted, weights
 
     def score(
         self, hidden: torch.Tensor, encoder_outputs: torch.Tensor
     ) -> torch.Tensor:
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/expert.py` & `yoyodyne-0.2.3/yoyodyne/models/expert.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 prediction y, it returns optimal cost-to-go for all valid edit actions.
 
 Also includes ActionVocabulary class for compatibility with maxwell dictionary.
 Class stores valid edit actions for given dataset.
 """
 
 import abc
+import argparse
 import dataclasses
 from typing import Any, Dict, Iterable, Iterator, List, Sequence, Set, Tuple
 
 import numpy
 from maxwell import actions, sed
 from torch.utils import data
 
-from . import util
+from .. import defaults, util
 
 
 class Error(Exception):
     pass
 
 
 class ActionVocabulary:
@@ -215,15 +216,15 @@
 
 class Expert(abc.ABC):
     actions: ActionVocabulary
     aligner: sed.StochasticEditDistance
     oracle_factor: int
     roll_in: int
 
-    def __init__(self, actions, aligner, oracle_factor=1):
+    def __init__(self, actions, aligner, oracle_factor=defaults.ORACLE_FACTOR):
         """Oracle scores possible edit actions between prediction and target.
 
         Args:
             actions (ActionVocabulary): vocabulary of possible edit actions.
             aligner (StochasticEditDistance): an alignment object to score
                 edits between source and target strings.
             oracle_factor (int): a scaling factor for scheduling predictions
@@ -390,16 +391,16 @@
             Prefix(prediction, target, i)
             for i in numpy.where(prediction_row == prediction_row.min())[0]
         ]
 
 
 def get_expert(
     train_data: data.Dataset,
-    epochs: int = 10,
-    oracle_factor: int = 1,
+    epochs: int = defaults.ORACLE_EM_EPOCHS,
+    oracle_factor: int = defaults.ORACLE_FACTOR,
     sed_params_path: str = None,
 ) -> Expert:
     """Generates expert object for training transducer.
 
     Args:
         data (data.Dataset): dataset for generating expert vocabulary.
         epochs (int): number of EM epochs.
@@ -426,19 +427,19 @@
             actions (ActionVocabulary): Vocabulary object
                 to encode actions for expert.
         Returns:
             Iterator[Tuple[List[int], List[int]]]: Iterator that
                 yields list version of source and target entries
                 in dataset.
         """
-        for source, *_, target in data:
+        for item in data:
             # Dataset encodes BOW and EOW symbols for source. EOW
             # for target. Removes these for SED training.
-            source = source.tolist()[1:-1]
-            target = target.tolist()[:-1]
+            source = item.source.tolist()[1:-1]
+            target = item.target.tolist()[:-1]
             actions.encode_actions(target)
             yield source, target
 
     def _encode_action_vocabulary(
         data: data.Dataset, actions: ActionVocabulary
     ) -> None:
         """Encodes action vocabulary for expert oracle.
@@ -446,17 +447,17 @@
         For instantiating SED objects from file.
 
         Args:
             data (data.Dataset): Dataset to iterate over.
             actions (ActionVocabulary): Vocabulary object
                 to encode actions for expert.
         """
-        for _, *_, target in data:
+        for item in data:
             # Ignores last symbol since EOW.
-            target = target.tolist()[:-1]
+            target = item.target.tolist()[:-1]
             actions.encode_actions(target)
 
     if sed_params_path:
         sed_params = sed.ParamDict.read_params(sed_params_path)
         sed_aligner = sed.StochasticEditDistance(sed_params)
         actions = ActionVocabulary()
         # Loads vocabulary into action vocabulary.
@@ -465,7 +466,36 @@
         actions = ActionVocabulary()
         sed_aligner = sed.StochasticEditDistance.fit_from_data(
             _generate_data_and_encode_vocabulary(train_data, actions),
             epochs=epochs,
         )
     util.log_info(f"Action vocabulary: {actions}")
     return Expert(actions, sed_aligner, oracle_factor=oracle_factor)
+
+
+def add_argparse_args(parser: argparse.ArgumentParser) -> None:
+    """Adds expert configuration options to the argument parser.
+
+    These are only needed at training time.
+
+    Args:
+        parser (argparse.ArgumentParser).
+    """
+    parser.add_argument(
+        "--oracle_em_epochs",
+        type=int,
+        default=defaults.ORACLE_EM_EPOCHS,
+        help="Number of EM epochs "
+        "(transducer architecture only). Default: %(default)s.",
+    )
+    parser.add_argument(
+        "--oracle_factor",
+        type=int,
+        default=defaults.ORACLE_FACTOR,
+        help="Roll-in schedule parameter "
+        "(transducer architecture only). Default: %(default)s.",
+    )
+    parser.add_argument(
+        "--sed_path",
+        type=str,
+        help="Path to input SED parameters (transducer architecture only)",
+    )
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/generation_probability.py` & `yoyodyne-0.2.3/yoyodyne/models/generation_probability.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,53 @@
 
 
 class GenerationProbability(nn.Module):
     """Calculates the generation probability for a pointer generator."""
 
     stdev = 1 / math.sqrt(100)
 
-    W_attn: nn.Linear
+    W_attention: nn.Linear
     W_hs: nn.Linear
     W_inp: nn.Linear
     bias: nn.Parameter
 
-    def __init__(self, embedding_size: int, hidden_size: int, attn_size: int):
+    def __init__(
+        self, embedding_size: int, hidden_size: int, attention_size: int
+    ):
         """Initializes the generation probability operator.
 
         Args:
             embedding_size (int): embedding dimensions.
             hidden_size (int): decoder hidden state dimensions.
-            attn_size (int): dimensions of combined encoder attentions.
+            attention_size (int): dimensions of combined encoder attentions.
         """
         super().__init__()
-        self.W_attn = nn.Linear(attn_size, 1, bias=False)
+        self.W_attention = nn.Linear(attention_size, 1, bias=False)
         self.W_hs = nn.Linear(hidden_size, 1, bias=False)
         self.W_inp = nn.Linear(embedding_size, 1, bias=False)
         self.bias = nn.Parameter(torch.Tensor(1))
         self.bias.data.uniform_(-self.stdev, self.stdev)
 
     def forward(
-        self, h_attn: torch.Tensor, dec_hs: torch.Tensor, inp: torch.Tensor
+        self,
+        h_attention: torch.Tensor,
+        decoder_hs: torch.Tensor,
+        inp: torch.Tensor,
     ) -> torch.Tensor:
         """Computes Wh * ATTN_t + Ws * HIDDEN_t + Wy * Y_{t-1} + b.
 
         Args:
-            h_attn (torch.Tensor): combined context vector over source and
-                features of shape B x 1 x attn_size.
-            dec_hs (torch.Tensor): decoder hidden state of shape
+            h_attention (torch.Tensor): combined context vector over source and
+                features of shape B x 1 x attention_size.
+            decoder_hs (torch.Tensor): decoder hidden state of shape
                 B x 1 x hidden_size.
             inp (torch.Tensor): decoder input of shape B x 1 x embedding_size.
 
         Returns:
             (torch.Tensor): generation probability of shape B.
         """
         # -> B x 1 x 1.
-        p_gen = self.W_attn(h_attn) + self.W_hs(dec_hs)
-        p_gen += self.W_inp(inp) + self.bias.expand(h_attn.size(0), 1, -1)
+        p_gen = self.W_attention(h_attention) + self.W_hs(decoder_hs)
+        p_gen += self.W_inp(inp) + self.bias.expand(h_attention.size(0), 1, -1)
         # -> B.
         p_gen = torch.sigmoid(p_gen.squeeze(1))
         return p_gen
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/lstm.py` & `yoyodyne-0.2.3/yoyodyne/models/lstm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,168 +1,84 @@
 """LSTM model classes."""
 
+import argparse
 import heapq
 from typing import List, Optional, Tuple, Union
 
 import torch
 from torch import nn
 
-from .. import evaluators
 from . import attention, base
-
-
-class Error(Exception):
-    pass
+from .. import batches, defaults
 
 
 class LSTMEncoderDecoder(base.BaseEncoderDecoder):
     """LSTM encoder-decoder without attention.
 
     We achieve this by concatenating the last (non-padding) hidden state of
     the encoder to the decoder hidden state."""
 
-    vocab_size: int
-    enc_layers: int
-    dec_layers: int
-    pad_idx: int
-    optim_name: str
-    beta1: float
-    beta2: float
-    warmup_steps: int
-    lr: int
-    evaluator: evaluators.Evaluator
-    scheduler: str
-    start_idx: int
-    end_idx: int
-    embedding_size: int
+    # Model arguments.
     bidirectional: bool
-    num_directions: int
-    dropout: float
-    dropout_layer: nn.Dropout
-    hidden_size: int
-    output_size: int
+    # Constructed inside __init__.
     source_embeddings: nn.Embedding
     target_embeddings: nn.Embedding
     encoder: nn.LSTM
     h0: nn.Parameter
     c0: nn.Parameter
-    max_decode_len: int
     decoder: nn.LSTM
     classifier: nn.Linear
     log_softmax: nn.LogSoftmax
-    label_smoothing: Optional[float]
-    beam_width: Optional[int]
 
     def __init__(
         self,
-        vocab_size,
-        embedding_size,
-        hidden_size,
-        output_size,
-        pad_idx,
-        start_idx,
-        end_idx,
-        optim,
-        beta1,
-        beta2,
-        warmup_steps,
-        lr,
-        scheduler,
-        evaluator,
-        max_decode_len,
-        dropout=0.1,
-        enc_layers=2,
-        dec_layers=2,
-        bidirectional=True,
-        label_smoothing=None,
-        beam_width=None,
+        *args,
+        bidirectional=defaults.BIDIRECTIONAL,
         **kwargs,
     ):
         """Initializes the encoder-decoder without attention.
 
         Args:
-            vocab_size (int).
-            embedding_size (int).
-            hidden_size (int).
-            output_size (int).
-            pad_idx (int).
-            start_idx (int).
-            end_idx (int).
-            optim (str).
-            beta1 (float).
-            beta2 (float).
-            warmup_steps (int).
-            lr (float).
-            evaluator (evaluators.Evaluator).
-            scheduler (str).
-            max_decode_len (int).
-            dropout (float, optional).
-            enc_layers (int, optional).
-            dec_layers (int, optional).
-            bidirectional (bool, optional).
-            label_smoothing (float, optional).
-            beam_width (int, optional) defaults to None; if True, then beam
-                search is used for decoding. This should only be used at test
-                time.
-            **kwargs: ignored.
+            *args: passed to superclass.
+            bidirectional (bool).
+            **kwargs: passed to superclass.
         """
-        super().__init__()
-        self.vocab_size = vocab_size
-        self.enc_layers = enc_layers
-        self.dec_layers = dec_layers
-        self.pad_idx = pad_idx
-        self.optim_name = optim
-        self.beta1 = beta1
-        self.beta2 = beta2
-        self.warmup_steps = warmup_steps
-        self.lr = lr
-        self.evaluator = evaluator
-        self.scheduler = scheduler
-        self.start_idx = start_idx
-        self.end_idx = end_idx
-        self.embedding_size = embedding_size
+        super().__init__(*args, **kwargs)
         self.bidirectional = bidirectional
-        self.num_directions = 2 if self.bidirectional else 1
-        self.dropout = dropout
-        self.dropout_layer = nn.Dropout(p=self.dropout, inplace=False)
-        self.hidden_size = hidden_size
-        self.output_size = output_size
         self.source_embeddings = self.init_embeddings(
             self.vocab_size, self.embedding_size, self.pad_idx
         )
         self.target_embeddings = self.init_embeddings(
             self.output_size, self.embedding_size, self.pad_idx
         )
         self.encoder = nn.LSTM(
             self.embedding_size,
             self.hidden_size,
-            num_layers=enc_layers,
-            dropout=dropout,
+            num_layers=self.encoder_layers,
+            dropout=self.dropout,
             batch_first=True,
             bidirectional=self.bidirectional,
         )
-        enc_size = self.hidden_size * self.num_directions
+        encoder_size = self.hidden_size * self.num_directions
         # Initial hidden state whose parameters are shared across all examples.
         self.h0 = nn.Parameter(torch.rand(self.hidden_size))
         self.c0 = nn.Parameter(torch.rand(self.hidden_size))
-        self.max_decode_len = max_decode_len
         self.decoder = nn.LSTM(
-            enc_size + self.embedding_size,
+            encoder_size + self.embedding_size,
             self.hidden_size,
             dropout=self.dropout,
-            num_layers=self.dec_layers,
+            num_layers=self.decoder_layers,
             batch_first=True,
         )
-        self.classifier = nn.Linear(self.hidden_size, output_size)
+        self.classifier = nn.Linear(self.hidden_size, self.output_size)
         self.log_softmax = nn.LogSoftmax(dim=2)
-        self.label_smoothing = label_smoothing
-        self.beam_width = beam_width
-        self.loss_func = self.get_loss_func("mean")
-        # Saves hyperparameters for PL checkpointing.
-        self.save_hyperparameters()
+
+    @property
+    def num_directions(self):
+        return 2 if self.bidirectional else 1
 
     def init_embeddings(
         self, num_embeddings: int, embedding_size: int, pad_idx: int
     ) -> nn.Embedding:
         """Initializes the embedding layer.
 
         Args:
@@ -174,33 +90,31 @@
             nn.Embedding: embedding layer.
         """
         return self._normal_embedding_initialization(
             num_embeddings, embedding_size, pad_idx
         )
 
     def encode(
-        self, source: torch.Tensor, mask: torch.Tensor
+        self, source: batches.PaddedTensor
     ) -> Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
-        """Encodes a batch of inputs.
+        """Encodes the input.
 
         Args:
-            source (torch.Tensor): input symbols of shape B x seq_len x 1
-            mask (torch.Tensor): mask for the input symbols of shape
-                B x seq_len x 1
+            source (batches.PaddedTensor): source padded tensors and mask
+                for source, of shape B x seq_len x 1.
 
         Returns:
             Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
                 encoded timesteps, and the LSTM h0 and c0 cells.
         """
-        embedded = self.source_embeddings(source)
+        embedded = self.source_embeddings(source.padded)
         embedded = self.dropout_layer(embedded)
         # Packs embedded source symbols into a PackedSequence.
-        lens = (mask == 0).sum(dim=1).to("cpu")
         packed = nn.utils.rnn.pack_padded_sequence(
-            embedded, lens, batch_first=True, enforce_sorted=False
+            embedded, source.lengths(), batch_first=True, enforce_sorted=False
         )
         # -> B x seq_len x encoder_dim, (h0, c0).
         packed_outs, (H, C) = self.encoder(packed)
         encoded, _ = nn.utils.rnn.pad_packed_sequence(
             packed_outs,
             batch_first=True,
             padding_value=self.pad_idx,
@@ -208,232 +122,249 @@
         )
         return encoded, (H, C)
 
     def decode_step(
         self,
         symbol: torch.Tensor,
         last_hiddens: torch.Tensor,
-        enc_out: torch.Tensor,
-        enc_mask: torch.Tensor,
+        encoder_out: torch.Tensor,
+        encoder_mask: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Decodes one step.
 
         Args:
             symbol (torch.Tensor): previously decoded symbol of shape B x 1.
             last_hiddens (torch.Tensor): last hidden states from the decoder
                 of shape (1 x B x decoder_dim, 1 x B x decoder_dim).
-            enc_out (torch.Tensor): encoded input sequence of shape
+            encoder_out (torch.Tensor): encoded input sequence of shape
                 B x seq_len x encoder_dim.
-            enc_mask (torch.Tensor): mask for the encoded input batch of shape
-                B x seq_len.
+            encoder_mask (torch.Tensor): mask for the encoded input batch of
+                shape B x seq_len.
 
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: tuple of scores and hiddens.
         """
         embedded = self.target_embeddings(symbol)
         embedded = self.dropout_layer(embedded)
         # -> 1 x B x decoder_dim.
         last_h0, last_c0 = last_hiddens
         # Get the index of the last unmasked tensor.
         # -> B.
-        last_enc_out_idxs = (~enc_mask).sum(dim=1) - 1
+        last_encoder_out_idxs = (~encoder_mask).sum(dim=1) - 1
         # -> B x 1 x 1.
-        last_enc_out_idxs = last_enc_out_idxs.view([enc_out.size(0)] + [1, 1])
+        last_encoder_out_idxs = last_encoder_out_idxs.view(
+            [encoder_out.size(0)] + [1, 1]
+        )
         # -> 1 x 1 x encoder_dim. This indexes the last non-padded dimension.
-        last_enc_out_idxs = last_enc_out_idxs.expand(
-            [-1, -1, enc_out.size(-1)]
+        last_encoder_out_idxs = last_encoder_out_idxs.expand(
+            [-1, -1, encoder_out.size(-1)]
         )
         # -> B x 1 x encoder_dim.
-        last_enc_out = torch.gather(enc_out, 1, last_enc_out_idxs)
+        last_encoder_out = torch.gather(encoder_out, 1, last_encoder_out_idxs)
         # The input to decoder LSTM is the embedding concatenated to the
         # weighted, encoded, inputs.
         output, hiddens = self.decoder(
-            torch.cat((embedded, last_enc_out), 2), (last_h0, last_c0)
+            torch.cat((embedded, last_encoder_out), 2), (last_h0, last_c0)
         )
         output = self.dropout_layer(output)
         # Classifies into output vocab.
         # -> B x 1 x output_size.
         output = self.classifier(output)
         # Computes log_softmax scores for NLLLoss.
         output = self.log_softmax(output)
         return output, hiddens
 
     def init_hiddens(
-        self, batch_size: int
+        self, batch_size: int, num_layers: int
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Initializes the hidden state to pass to the LSTM.
 
         Note that we learn the initial state h0 as a parameter of the model.
 
         Args:
             batch_size (int).
+            num_layers (int).
 
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: hidden cells for LSTM
                 initialization.
         """
         return (
-            self.h0.repeat(self.enc_layers, batch_size, 1),
-            self.c0.repeat(self.enc_layers, batch_size, 1),
+            self.h0.repeat(num_layers, batch_size, 1),
+            self.c0.repeat(num_layers, batch_size, 1),
         )
 
     def decode(
         self,
         batch_size: int,
-        enc_mask: torch.Tensor,
-        enc_out: torch.Tensor,
+        encoder_mask: torch.Tensor,
+        encoder_out: torch.Tensor,
+        teacher_forcing: bool,
         target: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         """Decodes a sequence given the encoded input.
 
-        This initializes an <EOS> tensor, and decodes using teacher forcing
-        when training, or else greedily.
+        Decodes until all sequences in a batch have reached [EOS] up to
+        a specified length depending on the `target` args.
 
         Args:
             batch_size (int).
-            enc_mask (torch.Tensor): mask for the batch of encoded inputs.
-            enc_out (torch.Tensor): batch of encoded inputs.
-            target (torch.Tensor, optional): target symbols. If None, then we
-                decode greedily with 'student forcing'.
+            encoder_mask (torch.Tensor): mask for the batch of encoded
+                input symbols.
+            encoder_out (torch.Tensor): batch of encoded input symbols.
+            teacher_forcing (bool): Whether or not to decode
+                with teacher forcing.
+            target (torch.Tensor, optional): target symbols;  we
+                decode up to `len(target)` symbols. If it is None, then we
+                decode up to `self.max_target_length` symbols.
 
         Returns:
-            preds (torch.Tensor): tensor of predictions of shape
-                (sequence_length, batch_size, output_size)
+            predictions (torch.Tensor): tensor of predictions of shape
+                seq_len x batch_size x output_size.
         """
         # Initializes hidden states for decoder LSTM.
-        decoder_hiddens = self.init_hiddens(batch_size)
+        decoder_hiddens = self.init_hiddens(batch_size, self.decoder_layers)
         # Feed in the first decoder input, as a start tag.
         # -> B x 1.
         decoder_input = (
-            torch.LongTensor([self.start_idx])
-            .to(self.device)
+            torch.tensor(
+                [self.start_idx], device=self.device, dtype=torch.long
+            )
             .repeat(batch_size)
             .unsqueeze(1)
         )
-        preds = []
+        predictions = []
         num_steps = (
-            target.size(1) if target is not None else self.max_decode_len
+            target.size(1) if target is not None else self.max_target_length
         )
         # Tracks when each sequence has decoded an EOS.
-        finished = torch.zeros(batch_size).to(self.device)
+        finished = torch.zeros(batch_size, device=self.device)
         for t in range(num_steps):
             # pred: B x 1 x output_size.
             output, decoder_hiddens = self.decode_step(
-                decoder_input, decoder_hiddens, enc_out, enc_mask
+                decoder_input, decoder_hiddens, encoder_out, encoder_mask
             )
-            preds.append(output.squeeze(1))
-            # If we have a target (training) then the next input is the gold
-            # symbol for this step (i.e., teacher forcing).
-            if target is not None:
+            predictions.append(output.squeeze(1))
+            # In teacher forcing mode the next input is the gold symbol
+            # for this step.
+            if teacher_forcing:
+                assert (
+                    target is not None
+                ), "Teacher forcing requested but no target provided"
                 decoder_input = target[:, t].unsqueeze(1)
-            # Otherwise, it must be inference time and we pass the top pred to
-            # the next next timestep (i.e., student forcing, greedy decoding).
+            # Otherwise we pass the top pred to the next timestep
+            # (i.e., student forcing, greedy decoding).
             else:
                 decoder_input = self._get_predicted(output)
                 # Updates to track which sequences have decoded an EOS.
                 finished = torch.logical_or(
                     finished, (decoder_input == self.end_idx)
                 )
                 # Breaks when all batches predicted an EOS symbol.
+                # If we have a target (and are thus computing loss),
+                # we only break when we have decoded at least the the
+                # same number of steps as the target length.
                 if finished.all():
-                    break
-        preds = torch.stack(preds)
-        return preds
+                    if target is None or decoder_input.size(-1) >= target.size(
+                        -1
+                    ):
+                        break
+        predictions = torch.stack(predictions)
+        return predictions
 
     def beam_decode(
         self,
         batch_size: int,
-        enc_mask: torch.Tensor,
-        enc_out: torch.Tensor,
+        encoder_mask: torch.Tensor,
+        encoder_out: torch.Tensor,
         beam_width: int,
         n: int = 1,
         return_confidences: bool = False,
     ) -> Union[Tuple[List, List], List]:
         """Beam search with beam_width.
 
         Note that we assume batch size is 1.
 
         Args:
             batch_size (int).
-            enc_mask (torch.Tensor).
-            enc_out (torch.Tensor): encoded inputs.
+            encoder_mask (torch.Tensor).
+            encoder_out (torch.Tensor): encoded inputs.
             beam_width (int): size of the beam.
             n (int): number of hypotheses to return.
             return_confidences (bool, optional): additionally return the
                 likelihood of each hypothesis.
 
         Returns:
             Union[Tuple[List, List], List]: _description_
         """
         # TODO: only implemented for batch size of 1. Implement batch mode.
         if batch_size != 1:
             raise NotImplementedError(
                 "Beam search is not implemented for batch_size > 1"
             )
         # Initializes hidden states for decoder LSTM.
-        decoder_hiddens = self.init_hiddens(enc_out.size(0))
+        decoder_hiddens = self.init_hiddens(
+            encoder_out.size(0), self.decoder_layers
+        )
         # log likelihood, last decoded idx, all likelihoods,  hiddens tensor.
         histories = [[0.0, [self.start_idx], [0.0], decoder_hiddens]]
-        for t in range(self.max_decode_len):
-            # Flat [List] that stores the heap of the top beam_width elements
-            # from all beam_width * output_size possibilities
+        for t in range(self.max_target_length):
+            # List that stores the heap of the top beam_width elements from all
+            # beam_width x output_size possibilities
             likelihoods = []
             hypotheses = []
             # First accumulates all beam_width softmaxes.
             for (
                 beam_likelihood,
                 beam_idxs,
                 char_likelihoods,
                 decoder_hiddens,
             ) in histories:
-                # Doesn ot keep decoding a path that has hit EOS.
+                # Does not keep decoding a path that has hit EOS.
                 if len(beam_idxs) > 1 and beam_idxs[-1] == self.end_idx:
                     fields = [
                         beam_likelihood,
                         beam_idxs,
                         char_likelihoods,
                         decoder_hiddens,
                     ]
                     # TODO: Beam search with beam_width.
                     # TODO: Replace heapq with torch.max or similar?
                     heapq.heappush(hypotheses, fields)
                     continue
                 # Feeds in the first decoder input, as a start tag.
                 # -> batch_size x 1
-                decoder_input = (
-                    torch.LongTensor([beam_idxs[-1]])
-                    .to(self.device)
-                    .unsqueeze(1)
-                )
-                preds, decoder_hiddens = self.decode_step(
-                    decoder_input, decoder_hiddens, enc_out, enc_mask
+                decoder_input = torch.tensor(
+                    [beam_idxs[-1]], device=self.device, dtype=torch.long
+                ).unsqueeze(1)
+                predictions, decoder_hiddens = self.decode_step(
+                    decoder_input, decoder_hiddens, encoder_out, encoder_mask
                 )
                 likelihoods.append(
                     (
-                        preds,
+                        predictions,
                         beam_likelihood,
                         beam_idxs,
                         char_likelihoods,
                         decoder_hiddens,
                     )
                 )
             # Constrains the next step to beamsize.
             for (
-                preds,
+                predictions,
                 beam_likelihood,
                 beam_idxs,
                 char_likelihoods,
                 decoder_hiddens,
             ) in likelihoods:
-                # Preds is B x seq_len x outputs.
-                # This is 1 x 1 x outputs since we fixed batch size to 1.
+                # This is 1 x 1 x output_size since we fixed batch size to 1.
                 # We squeeze off the fist 2 dimensions to get a tensor of
                 # output_size.
-                preds = preds.squeeze(0).squeeze(0)
-                for j, prob in enumerate(preds):
+                predictions = predictions.squeeze(0).squeeze(0)
+                for j, prob in enumerate(predictions):
                     if return_confidences:
                         cl = char_likelihoods + [prob]
                     else:
                         cl = char_likelihoods
                     if len(hypotheses) < beam_width:
                         fields = [
                             beam_likelihood + prob,
@@ -453,92 +384,117 @@
             # Takes the top beam hypotheses from the heap.
             histories = heapq.nlargest(beam_width, hypotheses)
             # If the top n hypotheses are full sequences, break.
             if all([h[1][-1] == self.end_idx for h in histories]):
                 break
         # Returns the top-n hypotheses.
         histories = heapq.nlargest(n, hypotheses)
-        preds = torch.tensor([h[1] for h in histories])
+        predictions = torch.tensor([h[1] for h in histories], self.device)
         # Converts shape to that of `decode`: seq_len x B x output_size.
-        preds = preds.unsqueeze(0).transpose(0, 2)
+        predictions = predictions.unsqueeze(0).transpose(0, 2)
         if return_confidences:
-            return (preds, torch.tensor([h[2] for h in histories]))
+            return (predictions, torch.tensor([h[2] for h in histories]))
         else:
-            return preds
+            return predictions
 
-    def forward(self, batch: base.Batch) -> torch.Tensor:
+    def forward(
+        self,
+        batch: batches.PaddedBatch,
+    ) -> torch.Tensor:
         """Runs the encoder-decoder model.
 
         Args:
-            batch (base.Batch): batch of the input, input mask, output, and
-                output mask.
+            batch (batches.PaddedBatch).
 
         Returns:
-            preds (torch.Tensor): tensor of predictions of shape
-                (sequence_length, batch_size, output_size).
+            predictions (torch.Tensor): tensor of predictions of shape
+                (seq_len, batch_size, output_size).
         """
-        if len(batch) == 4:
-            source, source_mask, target, target_mask = batch
-        elif len(batch) == 2:
-            source, source_mask = batch
-            target = None
-        else:
-            raise Error(f"Batch of {len(batch)} elements is invalid")
-        batch_size = source.size(0)
-        enc_out, _ = self.encode(source, source_mask)
+        encoder_out, _ = self.encode(batch.source)
         if self.beam_width is not None and self.beam_width > 1:
-            preds = self.beam_decode(
-                batch_size, source_mask, enc_out, beam_width=self.beam_width
+            predictions = self.beam_decode(
+                len(batch),
+                batch.source.mask,
+                encoder_out,
+                beam_width=self.beam_width,
             )
         else:
-            preds = self.decode(batch_size, source_mask, enc_out, target)
-        # -> B x output_size x seq_len.
-        preds = preds.transpose(0, 1).transpose(1, 2)
-        return preds
+            predictions = self.decode(
+                len(batch),
+                batch.source.mask,
+                encoder_out,
+                self.teacher_forcing if self.training else False,
+                batch.target.padded if batch.target else None,
+            )
+        # -> B x seq_len x output_size.
+        predictions = predictions.transpose(0, 1)
+        return predictions
+
+    @staticmethod
+    def add_argparse_args(parser: argparse.ArgumentParser) -> None:
+        """Adds LSTM configuration options to the argument parser.
+
+        Args:
+            parser (argparse.ArgumentParser).
+        """
+        parser.add_argument(
+            "--bidirectional",
+            action="store_true",
+            default=defaults.BIDIRECTIONAL,
+            help="Uses a bidirectional encoder "
+            "(LSTM-backed architectures only. Default: %(default)s.",
+        )
+        parser.add_argument(
+            "--no_bidirectional",
+            action="store_false",
+            dest="bidirectional",
+        )
 
 
-class LSTMEncoderDecoderAttention(LSTMEncoderDecoder):
+class AttentiveLSTMEncoderDecoder(LSTMEncoderDecoder):
     """LSTM encoder-decoder with attention."""
 
     attention: attention.Attention
 
     def __init__(self, *args, **kwargs):
         """Initializes the encoder-decoder with attention."""
         super().__init__(*args, **kwargs)
-        enc_size = self.hidden_size * self.num_directions
-        self.attention = attention.Attention(enc_size, self.hidden_size)
+        encoder_size = self.hidden_size * self.num_directions
+        self.attention = attention.Attention(encoder_size, self.hidden_size)
 
     def decode_step(
         self,
         symbol: torch.Tensor,
         last_hiddens: Tuple[torch.Tensor, torch.Tensor],
-        enc_out: torch.Tensor,
-        enc_mask: torch.Tensor,
+        encoder_out: torch.Tensor,
+        encoder_mask: torch.Tensor,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Decodes one step.
 
         Args:
             symbol (torch.Tensor): previously decoded symbol of shape B x 1.
             last_hiddens (Tuple[torch.Tensor, torch.Tensor]): last hidden
                 states from the decoder of shape
                 (1 x B x decoder_dim, 1 x B x decoder_dim).
-            enc_out (torch.Tensor): encoded input sequence of shape
+            encoder_out (torch.Tensor): encoded input sequence of shape
                 B x seq_len x encoder_dim.
-            enc_mask (torch.Tensor): mask for the encoded input batch of
+            encoder_mask (torch.Tensor): mask for the encoded input batch of
                 shape B x seq_len.
 
         Returns:
             Tuple[torch.Tensor, torch.Tensor]: softmax scores over all outputs,
                 and the previous hidden states from the decoder LSTM.
         """
         embedded = self.target_embeddings(symbol)
         embedded = self.dropout_layer(embedded)
         # -> 1 x B x decoder_dim.
         last_h0, last_c0 = last_hiddens
-        context, _ = self.attention(last_h0.transpose(0, 1), enc_out, enc_mask)
+        context, _ = self.attention(
+            last_h0.transpose(0, 1), encoder_out, encoder_mask
+        )
         output, hiddens = self.decoder(
             torch.cat((embedded, context), 2), (last_h0, last_c0)
         )
         output = self.dropout_layer(output)
         # Classifies into output vocab.
         # -> B x 1 x output_size
         output = self.classifier(output)
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/pointer_generator.py` & `yoyodyne-0.2.3/yoyodyne/models/pointer_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Pointer-generator model classes."""
 
 from typing import Optional, Tuple
 
 import torch
 from torch import nn
 
-from . import attention, base, lstm, generation_probability
+from . import attention, generation_probability, lstm
+from .. import batches
 
 
 class Error(Exception):
     pass
 
 
 class PointerGeneratorLSTMEncoderDecoderNoFeatures(lstm.LSTMEncoderDecoder):
@@ -18,69 +19,81 @@
     After:
         See, A., Liu, P. J., and Manning, C. D. 2017. Get to the point:
         summarization with pointer-generator networks. In Proceedings of the
         55th Annual Meeting of the Association for Computational Linguistics
         (Volume 1: Long Papers), pages 1073-1083.
     """
 
+    # Constructed inside __init__.
     source_attention: attention.Attention
     geneneration_probability: generation_probability.GenerationProbability
 
     def __init__(self, *args, **kwargs):
         """Initializes the pointer-generator model with an LSTM backend."""
         super().__init__(*args, **kwargs)
+        self._check_layer_sizes()
         # We use the inherited defaults for the source embeddings/encoder.
-        enc_size = self.hidden_size * self.num_directions
-        self.source_attention = attention.Attention(enc_size, self.hidden_size)
+        encoder_size = self.hidden_size * self.num_directions
+        self.source_attention = attention.Attention(
+            encoder_size, self.hidden_size
+        )
         # Overrides classifier to take larger input.
         self.classifier = nn.Linear(3 * self.hidden_size, self.output_size)
         self.generation_probability = (
-            generation_probability.GenerationProbability(
-                self.embedding_size, self.hidden_size, enc_size
+            generation_probability.GenerationProbability(  # noqa: E501
+                self.embedding_size, self.hidden_size, encoder_size
             )
         )
 
+    def _check_layer_sizes(self):
+        """Checks that encoder and decoder layers are the same number.
+
+        Raises:
+            Error.
+        """
+        if self.encoder_layers != self.decoder_layers:
+            msg = "encoder_layers needs to be the same as decoder_layers."
+            msg += f" {self.encoder_layers} != {self.decoder_layers}."
+            raise Error(msg)
+
     def encode(
         self,
-        source: torch.Tensor,
-        source_mask: torch.Tensor,
+        source: batches.PaddedTensor,
         encoder: torch.nn.LSTM,
     ) -> torch.Tensor:
         """Encodes the input.
 
         Args:
-            source (torch.Tensor).
-            source_mask (torch.Tensor).
+            source (batches.PaddedTensor).
             encoder (torch.nn.LSTM).
 
         Returns:
             torch.Tensor: sequence of encoded symbols.
         """
-        embedded = self.source_embeddings(source)
+        embedded = self.source_embeddings(source.padded)
         embedded = self.dropout_layer(embedded)
-        lens = (source_mask == 0).sum(dim=1).to("cpu")
         packed = nn.utils.rnn.pack_padded_sequence(
-            embedded, lens, batch_first=True, enforce_sorted=False
+            embedded, source.lengths(), batch_first=True, enforce_sorted=False
         )
         # -> B x seq_len x encoder_dim,
         # (D*layers x B x hidden_size, D*layers x B x hidden_size)
-        packed_outs, (H, C) = self.encoder(packed)
+        packed_outs, (H, C) = encoder(packed)
         encoded, _ = torch.nn.utils.rnn.pad_packed_sequence(
             packed_outs,
             batch_first=True,
             padding_value=self.pad_idx,
             total_length=None,
         )
         # Sums over directions, keeping layers.
         # -> num_layers x B x hidden_size.
         H = H.view(
-            self.enc_layers, self.num_directions, H.size(1), H.size(2)
+            self.encoder_layers, self.num_directions, H.size(1), H.size(2)
         ).sum(axis=1)
         C = C.view(
-            self.enc_layers, self.num_directions, C.size(1), C.size(2)
+            self.encoder_layers, self.num_directions, C.size(1), C.size(2)
         ).sum(axis=1)
         return encoded, (H, C)
 
     def decode_step(
         self,
         symbol: torch.Tensor,
         last_hiddens: Tuple[torch.Tensor, torch.Tensor],
@@ -102,243 +115,270 @@
         Returns:
             Tuple[torch.Tensor, torch.Tensor].
         """
         embedded = self.target_embeddings(symbol)
         embedded = self.dropout_layer(embedded)
         # -> 1 x B x decoder_dim.
         last_h, last_c = last_hiddens
-        source_context, source_attn_weights = self.source_attention(
+        source_context, source_attention_weights = self.source_attention(
             last_h.transpose(0, 1), source_enc, source_mask
         )
         _, (h, c) = self.decoder(
             torch.cat((embedded, source_context), 2), (last_h, last_c)
         )
-        hidden = h.transpose(0, 1)
+        # -> B x 1 x hidden_size
+        hidden = h[-1, :, :].unsqueeze(1)
         output_probs = self.classifier(
             torch.cat([hidden, source_context], dim=2)
         )
         # Ordinary softmax, log will be taken at the end.
         output_probs = nn.functional.softmax(output_probs, dim=2)
         # -> B x 1 x output_size.
-        attn_probs = torch.zeros(
-            symbol.size(0), self.output_size, device=self.device
+        ptr_probs = torch.zeros(
+            symbol.size(0),
+            self.output_size,
+            device=self.device,
+            dtype=source_attention_weights.dtype,
         ).unsqueeze(1)
         # Gets the attentions to the source in terms of the output generations.
         # These are the "pointer" distribution.
         # -> B x 1 x output_size.
-        attn_probs.scatter_add_(
-            2, source_indices.unsqueeze(1), source_attn_weights
+        ptr_probs.scatter_add_(
+            2, source_indices.unsqueeze(1), source_attention_weights
         )
         # Probability of generating (from output_probs).
         gen_probs = self.generation_probability(
             source_context, hidden, embedded
         ).unsqueeze(2)
         gen_scores = gen_probs * output_probs
-        ptr_scores = (1 - gen_probs) * attn_probs
+        ptr_scores = (1 - gen_probs) * ptr_probs
         scores = gen_scores + ptr_scores
         # Puts scores in log space.
         scores = torch.log(scores)
         return scores, (h, c)
 
     def decode(
         self,
         batch_size: int,
         decoder_hiddens: torch.Tensor,
         source_indices: torch.Tensor,
         source_enc: torch.Tensor,
         source_mask: torch.Tensor,
+        teacher_forcing: bool,
         target: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
-        """Decodes a sequence.
+        """Decodes a sequence given the encoded input.
+
+        Decodes until all sequences in a batch have reached [EOS] up to
+        a specified length depending on the `target` args.
 
         Args:
             batch_size (int).
-            decoder_hiddens (torch.Tensor).
-            source_indices (torch.Tensor).
-            source_enc (torch.Tensor).
-            source_mask (torch.Tensor).
-            target (torch.Tensor, optional).
+            decoder_hiddens (torch.Tensor): .
+            source_indices (torch.Tensor): Indices of the input for calculating
+                pointer weights.
+            source_enc (torch.Tensor): batch of encoded input symbols.
+            source_mask (torch.Tensor): mask for the batch of encoded input
+                symbols.
+            feature_enc (torch.Tensor): batch of encoded feaure symbols.
+            teacher_forcing (bool): Whether or not to decode
+                with teacher forcing.
+            target (torch.Tensor, optional): target symbols;  we
+                decode up to `len(target)` symbols. If it is None, then we
+                decode up to `self.max_target_length` symbols.
 
         Returns:
-            torch.Tensor
+            torch.Tensor.
         """
         # Feeds in the first decoder input, as a start tag.
         # -> B x 1
         decoder_input = (
-            torch.LongTensor([self.start_idx])
-            .to(self.device)
+            torch.tensor(
+                [self.start_idx], device=self.device, dtype=torch.long
+            )
             .repeat(batch_size)
             .unsqueeze(1)
         )
-        preds = []
+        predictions = []
         num_steps = (
-            target.size(1) if target is not None else self.max_decode_len
+            target.size(1) if target is not None else self.max_target_length
         )
         # Tracks when each sequence has decoded an EOS.
-        finished = torch.zeros(batch_size).to(self.device)
+        finished = torch.zeros(batch_size, device=self.device)
         for t in range(num_steps):
             # pred: B x 1 x output_size.
             output, decoder_hiddens = self.decode_step(
                 decoder_input,
                 decoder_hiddens,
                 source_indices,
                 source_enc,
                 source_mask,
             )
-            preds.append(output.squeeze(1))
-            # If we have a target (training) then the next input is the gold
-            # symbol for this step (teacher forcing).
-            if target is not None:
+            predictions.append(output.squeeze(1))
+            # In teacher forcing mode the next input is the gold symbol
+            # for this step.
+            if teacher_forcing:
+                assert (
+                    target is not None
+                ), "Teacher forcing requested but no target provided"
                 decoder_input = target[:, t].unsqueeze(1)
-            # Otherwise, it must be inference time and we pass the top pred
-            # to the next next timestep (student forcing; greedy decoding).
+            # Otherwise we pass the top pred to the next timestep
+            # (i.e., student forcing, greedy decoding).
             else:
                 decoder_input = self._get_predicted(output)
                 # Tracks which sequences have decoded an EOS.
                 finished = torch.logical_or(
                     finished, (decoder_input == self.end_idx)
                 )
-                # Breaks when all batches predicted an END symbol.
+                # Breaks when all batches predicted an EOS symbol.
+                # If we have a target (and are thus computing loss),
+                # we only break when we have decoded at least the the
+                # same number of steps as the target length.
                 if finished.all():
-                    break
-        preds = torch.stack(preds)
-        return preds
+                    if target is None or decoder_input.size(-1) >= target.size(
+                        -1
+                    ):
+                        break
+        predictions = torch.stack(predictions)
+        return predictions
 
-    def forward(self, batch: base.Batch) -> torch.Tensor:
+    def forward(
+        self,
+        batch: batches.PaddedBatch,
+    ) -> torch.Tensor:
         """Runs the encoder-decoder.
 
         Args:
-            batch (base.Batch): tuple of tensors in the batch.
+            batch (batches.PaddedBatch).
 
         Returns:
             torch.Tensor.
         """
-        # Training mode with targets.
-        if len(batch) == 4:
-            (source, source_mask, target, target_mask) = batch
-        # No targets given at inference.
-        elif len(batch) == 2:
-            source, source_mask = batch
-            target = None
-        else:
-            raise Error(f"Batch of {len(batch)} elements is invalid")
-        batch_size = source.size(0)
         source_encoded, (h_source, c_source) = self.encode(
-            source, source_mask, self.encoder
+            batch.source, self.encoder
         )
         if self.beam_width is not None and self.beam_width > 1:
-            # preds = self.beam_decode(
-            #     batch_size, x_mask, enc_out, beam_width=self.beam_width
+            # predictions = self.beam_decode(
+            #     batch_size, x_mask, encoder_out, beam_width=self.beam_width
             # )
             raise NotImplementedError
         else:
-            preds = self.decode(
-                batch_size,
+            predictions = self.decode(
+                len(batch),
                 (h_source, c_source),
-                source,
+                batch.source.padded,
                 source_encoded,
-                source_mask,
-                target,
+                batch.source.mask,
+                self.teacher_forcing if self.training else False,
+                batch.target.padded if batch.target else None,
             )
-        # -> B x output_size x seq_len.
-        preds = preds.transpose(0, 1).transpose(1, 2)
-        return preds
+        # -> B x seq_len x output_size.
+        predictions = predictions.transpose(0, 1)
+        return predictions
 
 
 class PointerGeneratorLSTMEncoderDecoderFeatures(
     PointerGeneratorLSTMEncoderDecoderNoFeatures
 ):
     """Pointer-generator model with an LSTM backend.
 
     After:
         See, A., Liu, P. J., and Manning, C. D. 2017. Get to the point:
         summarization with pointer-generator networks. In Proceedings of the
         55th Annual Meeting of the Association for Computational Linguistics
         (Volume 1: Long Papers), pages 1073-1083.
     """
 
+    # Constructed inside __init__.
+    feature_attention: attention.Attention
+    feature_embeddings: nn.Embedding
     feature_encoder: nn.LSTM
     linear_h: nn.Linear
     linear_c: nn.Linear
-    feature_attention: attention.Attention
 
     def __init__(self, *args, **kwargs):
         """Initializes the pointer-generator model with an LSTM backend."""
         super().__init__(*args, **kwargs)
+        self._check_layer_sizes()
         # We use the inherited defaults for the source embeddings/encoder.
+        self.feature_embeddings = self.init_embeddings(
+            self.features_vocab_size, self.embedding_size, self.pad_idx
+        )
         self.feature_encoder = nn.LSTM(
             self.embedding_size,
             self.hidden_size,
-            num_layers=self.enc_layers,
+            num_layers=self.encoder_layers,
             dropout=self.dropout,
             batch_first=True,
             bidirectional=self.bidirectional,
         )
         # Initializes the decoder.
         self.linear_h = nn.Linear(2 * self.hidden_size, self.hidden_size)
         self.linear_c = nn.Linear(2 * self.hidden_size, self.hidden_size)
-        enc_size = self.hidden_size * self.num_directions
+        encoder_size = self.hidden_size * self.num_directions
         self.feature_attention = attention.Attention(
-            enc_size, self.hidden_size
+            encoder_size, self.hidden_size
         )
         # Overrides decoder to be larger.
         self.decoder = nn.LSTM(
-            (2 * enc_size) + self.embedding_size,
+            2 * encoder_size + self.embedding_size,
             self.hidden_size,
             dropout=self.dropout,
-            num_layers=self.dec_layers,
+            num_layers=self.decoder_layers,
             batch_first=True,
         )
         # Overrides classifier to take larger input.
         self.classifier = nn.Linear(5 * self.hidden_size, self.output_size)
         # Overrides GenerationProbability to have larger hidden_size.
         self.generation_probability = (
-            generation_probability.GenerationProbability(
-                self.embedding_size, self.hidden_size, 2 * enc_size
+            generation_probability.GenerationProbability(  # noqa: E501
+                self.embedding_size, self.hidden_size, 2 * encoder_size
             )
         )
 
     def encode(
         self,
-        source: torch.Tensor,
-        source_mask: torch.Tensor,
+        source: batches.PaddedTensor,
+        embeddings: nn.Embedding,
         encoder: torch.nn.LSTM,
     ) -> torch.Tensor:
         """Encodes the input with the TransformerEncoder.
 
+        We pass the encoder as an argument to enable use of this function
+        with multiple encoders in derived classes.
+
         Args:
-            source (torch.Tensor).
-            source_mask (torch.Tensor).
+            source (batches.PaddedTensor).
+            embedding (torch.nn.Embedding).
             encoder (torch.nn.LSTM).
 
         Returns:
             torch.Tensor: sequence of encoded symbols.
         """
-        embedded = self.source_embeddings(source)
+        embedded = embeddings(source.padded)
         embedded = self.dropout_layer(embedded)
-        lens = (source_mask == 0).sum(dim=1).to("cpu")
         packed = nn.utils.rnn.pack_padded_sequence(
-            embedded, lens, batch_first=True, enforce_sorted=False
+            embedded, source.lengths(), batch_first=True, enforce_sorted=False
         )
         # -> B x seq_len x encoder_dim,
         # (D*layers x B x hidden_size, D*layers x B x hidden_size).
-        packed_outs, (H, C) = self.encoder(packed)
+        packed_outs, (H, C) = encoder(packed)
         encoded, _ = torch.nn.utils.rnn.pad_packed_sequence(
             packed_outs,
             batch_first=True,
             padding_value=self.pad_idx,
             total_length=None,
         )
         # Sums over directions, keeping layers.
         # -> num_layers x B x hidden_size.
         H = H.view(
-            self.enc_layers, self.num_directions, H.size(1), H.size(2)
+            self.encoder_layers, self.num_directions, H.size(1), H.size(2)
         ).sum(axis=1)
         C = C.view(
-            self.enc_layers, self.num_directions, C.size(1), C.size(2)
+            self.encoder_layers, self.num_directions, C.size(1), C.size(2)
         ).sum(axis=1)
         return encoded, (H, C)
 
     def decode_step(
         self,
         symbol: torch.Tensor,
         last_hiddens: Tuple[torch.Tensor, torch.Tensor],
@@ -364,166 +404,180 @@
         Returns:
             Tuple[torch.Tensor, torch.Tensor].
         """
         embedded = self.target_embeddings(symbol)
         embedded = self.dropout_layer(embedded)
         # -> 1 x B x decoder_dim.
         last_h, last_c = last_hiddens
-        source_context, source_attn_weights = self.source_attention(
+        source_context, source_attention_weights = self.source_attention(
             last_h.transpose(0, 1), source_enc, source_mask
         )
         feature_context, _ = self.feature_attention(
             last_h.transpose(0, 1), feature_enc, feature_mask
         )
         # -> B x 1 x 4*hidden_size.
         context = torch.cat([source_context, feature_context], dim=2)
+        # num_layers x B x hidden_size
         _, (h, c) = self.decoder(
             torch.cat((embedded, context), 2), (last_h, last_c)
         )
-        hidden = h.transpose(0, 1)
+        # -> B x 1 x hidden_size
+        hidden = h[-1, :, :].unsqueeze(1)
         output_probs = self.classifier(torch.cat([hidden, context], dim=2))
         # Ordinary softmax, log will be taken at the end.
         output_probs = nn.functional.softmax(output_probs, dim=2)
         # -> B x 1 x output_size.
-        attn_probs = torch.zeros(
-            symbol.size(0), self.output_size, device=self.device
+        ptr_probs = torch.zeros(
+            symbol.size(0),
+            self.output_size,
+            device=self.device,
+            dtype=source_attention_weights.dtype,
         ).unsqueeze(1)
         # Gets the attentions to the source in terms of the output generations.
         # These are the "pointer" distribution.
         # -> B x 1 x output_size.
-        attn_probs.scatter_add_(
-            2, source_indices.unsqueeze(1), source_attn_weights
+        ptr_probs.scatter_add_(
+            2, source_indices.unsqueeze(1), source_attention_weights
         )
         # Probability of generating (from output_probs).
         gen_probs = self.generation_probability(
             context, hidden, embedded
         ).unsqueeze(2)
         gen_scores = gen_probs * output_probs
-        ptr_scores = (1 - gen_probs) * attn_probs
+        ptr_scores = (1 - gen_probs) * ptr_probs
         scores = gen_scores + ptr_scores
         # Puts scores in log space.
         scores = torch.log(scores)
         return scores, (h, c)
 
     def decode(
         self,
         batch_size: int,
         decoder_hiddens: torch.Tensor,
         source_indices: torch.Tensor,
         source_enc: torch.Tensor,
         source_mask: torch.Tensor,
         feature_enc: torch.Tensor,
         feature_mask: torch.Tensor,
+        teacher_forcing: bool,
         target: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
-        """Decodes a sequence.
+        """Decodes a sequence given the encoded input.
+
+        Decodes until all sequences in a batch have reached [EOS] up to
+        a specified length depending on the `target` args.
 
         Args:
             batch_size (int).
-            decoder_hiddens (torch.Tensor).
-            source_indices (torch.Tensor).
-            source_enc (torch.Tensor).
-            source_mask (torch.Tensor).
-            feature_enc (torch.Tensor).
-            feature_mask (torch.Tensor).
-            target (torch.Tensor, optional).
+            decoder_hiddens (torch.Tensor): .
+            source_indices (torch.Tensor): Indices of the input for
+                calculating pointer weights.
+            source_enc (torch.Tensor): batch of encoded input symbols.
+            source_mask (torch.Tensor): mask for the batch of encoded
+                input symbols.
+            feature_enc (torch.Tensor): batch of encoded feaure symbols.
+            feature_mask (torch.Tensor): mask for the batch of encoded
+                feature symbols.
+            teacher_forcing (bool): Whether or not to decode
+                with teacher forcing.
+            target (torch.Tensor, optional): target symbols;  we
+                decode up to `len(target)` symbols. If it is None, then we
+                decode up to `self.max_target_length` symbols.
 
         Returns:
             torch.Tensor.
         """
         # Feeds in the first decoder input, as a start tag.
         # -> B x 1
         decoder_input = (
-            torch.LongTensor([self.start_idx])
-            .to(self.device)
+            torch.tensor(
+                [self.start_idx], device=self.device, dtype=torch.long
+            )
             .repeat(batch_size)
             .unsqueeze(1)
         )
-        preds = []
+        predictions = []
         num_steps = (
-            target.size(1) if target is not None else self.max_decode_len
+            target.size(1) if target is not None else self.max_target_length
         )
         # Tracks when each sequence has decoded an EOS.
-        finished = torch.zeros(batch_size).to(self.device)
+        finished = torch.zeros(batch_size, device=self.device)
         for t in range(num_steps):
             # pred: B x 1 x output_size.
             output, decoder_hiddens = self.decode_step(
                 decoder_input,
                 decoder_hiddens,
                 source_indices,
                 source_enc,
                 source_mask,
                 feature_enc,
                 feature_mask,
             )
-            preds.append(output.squeeze(1))
-            # If we have a target (training) then the next input is the gold
-            # symbol for this step (teacher forcing).
-            if target is not None:
+            predictions.append(output.squeeze(1))
+            # In teacher forcing mode the next input is the gold symbol
+            # for this step.
+            if teacher_forcing:
+                assert (
+                    target is not None
+                ), "Teacher forcing requested but no target provided"
                 decoder_input = target[:, t].unsqueeze(1)
-            # Otherwise, it must be inference time and we pass the top pred
-            # to the next next timestep (student forcing; greedy decoding).
+            # Otherwise we pass the top pred to the next timestep
+            # (i.e., student forcing, greedy decoding).
             else:
                 decoder_input = self._get_predicted(output)
                 # Tracks which sequences have decoded an EOS.
                 finished = torch.logical_or(
                     finished, (decoder_input == self.end_idx)
                 )
-                # Breaks when all batches predicted an END symbol.
+                # Breaks when all batches predicted an EOS symbol.
+                # If we have a target (and are thus computing loss),
+                # we only break when we have decoded at least the the
+                # same number of steps as the target length.
                 if finished.all():
-                    break
-        preds = torch.stack(preds)
-        return preds
+                    if target is None or decoder_input.size(-1) >= target.size(
+                        -1
+                    ):
+                        break
+        predictions = torch.stack(predictions)
+        return predictions
 
-    def forward(self, batch: base.Batch) -> torch.Tensor:
+    def forward(
+        self,
+        batch: batches.PaddedBatch,
+    ) -> torch.Tensor:
         """Runs the encoder-decoder.
 
         Args:
-            batch (base.Batch): tuple of tensors in the batch.
+            batch (batches.PaddedBatch).
 
         Returns:
             torch.Tensor.
         """
-        # Training mode with targets.
-        if len(batch) == 6:
-            (
-                source,
-                source_mask,
-                features,
-                features_mask,
-                target,
-                target_mask,
-            ) = batch
-        # No targets given at inference.
-        elif len(batch) == 4:
-            source, source_mask, features, features_mask = batch
-            target = None
-        else:
-            raise Error(f"Batch of {len(batch)} elements is invalid")
-        batch_size = source.size(0)
+        assert batch.has_features
         source_encoded, (h_source, c_source) = self.encode(
-            source, source_mask, self.encoder
+            batch.source, self.source_embeddings, self.encoder
         )
         features_encoded, (h_features, c_features) = self.encode(
-            features, features_mask, self.feature_encoder
+            batch.features, self.feature_embeddings, self.feature_encoder
         )
         h_0 = self.linear_h(torch.cat([h_source, h_features], dim=2))
         c_0 = self.linear_c(torch.cat([c_source, c_features], dim=2))
         if self.beam_width is not None and self.beam_width > 1:
-            # preds = self.beam_decode(
-            #     batch_size, x_mask, enc_out, beam_width=self.beam_width
+            # predictions = self.beam_decode(
+            #     batch_size, x_mask, encoder_out, beam_width=self.beam_width
             # )
             raise NotImplementedError
         else:
-            preds = self.decode(
-                batch_size,
+            predictions = self.decode(
+                len(batch),
                 (h_0, c_0),
-                source,
+                batch.source.padded,
                 source_encoded,
-                source_mask,
+                batch.source.mask,
                 features_encoded,
-                features_mask,
-                target,
+                batch.features.mask,
+                self.teacher_forcing if self.training else False,
+                batch.target.padded if batch.target else None,
             )
-        # -> B x output_size x seq_len.
-        preds = preds.transpose(0, 1).transpose(1, 2)
-        return preds
+        # -> B x seq_len x output_size.
+        predictions = predictions.transpose(0, 1)
+        return predictions
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/positional_encoding.py` & `yoyodyne-0.2.3/yoyodyne/models/positional_encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,45 @@
 """Positional encoding."""
 
 import math
-
 from typing import Optional
 
 import torch
 from torch import nn
 
+from .. import defaults
+
 
 class PositionalEncoding(nn.Module):
     """Positional encoding.
 
     After:
         https://pytorch.org/tutorials/beginner/transformer_tutorial.html.
     """
 
     pad_idx: int
 
-    def __init__(self, d_model: int, pad_idx, max_len: int = 100):
+    def __init__(
+        self,
+        d_model: int,
+        pad_idx,
+        max_source_length: int = defaults.MAX_SOURCE_LENGTH,
+    ):
         """
         Args:
             d_model (int).
             pad_idx (int).
-            max_len (int, optional).
+            max_source_length (int).
         """
         super(PositionalEncoding, self).__init__()
         self.pad_idx = pad_idx
-        positional_encoding = torch.zeros(max_len, d_model)
-        position = torch.arange(0, max_len, dtype=torch.float).unsqueeze(1)
+        positional_encoding = torch.zeros(max_source_length, d_model)
+        position = torch.arange(
+            0, max_source_length, dtype=torch.float
+        ).unsqueeze(1)
         scale_factor = -math.log(10000.0) / d_model
         div_term = torch.exp(
             torch.arange(0, d_model, 2).float() * scale_factor
         )
         positional_encoding[:, 0::2] = torch.sin(position * div_term)
         positional_encoding[:, 1::2] = torch.cos(position * div_term)
         positional_encoding = positional_encoding.unsqueeze(0)
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/transducer.py` & `yoyodyne-0.2.3/yoyodyne/models/transducer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,168 +1,167 @@
 """Transducer model class."""
 
 import math
-from typing import Dict, List, Optional, Tuple
+from typing import Callable, Dict, List, Optional, Tuple
 
 import numpy
 import torch
 from maxwell import actions
 from torch import nn
 
-from . import base, expert, lstm
+from . import expert, lstm
+from .. import batches
 
 
 class ActionError(Exception):
     pass
 
 
 class TransducerNoFeatures(lstm.LSTMEncoderDecoder):
-    """Transducer model.
+    """Transducer model with an LSTM backend and no features.
 
     After:
         Makarov, P., and Clematide, S. 2018. Imitation learning for neural
         morphological string transduction. In Proceedings of the 2018
         Conference on Empirical Methods in Natural Language Processing, pages
         2877–2882.
 
     This uses a trained oracle for imitation learning edits.
     """
 
     expert: expert.Expert
+    # Constructed inside __init__.
+    target_embeddings: nn.Embedding
 
     def __init__(
         self,
         expert,
         *args,
         **kwargs,
     ):
-        """Initializes transducer model, using LSTM backend.
+        """Initializes transducer model.
 
         Args:
             expert (expert.Expert): oracle that guides training for transducer.
             *args: passed to superclass.
             **kwargs: passed to superclass.
         """
+        # Alternate outputs than dataset targets.
+        kwargs["output_size"] = len(expert.actions)
+        super().__init__(*args, **kwargs)
         # Model specific variables.
         self.expert = expert  # Oracle to train model.
         self.actions = self.expert.actions
         self.substitutions = self.actions.substitutions
-        self.inserts = self.actions.insertions
-        # Alternate outputs than dataset targets.
-        kwargs["output_size"] = len(expert.actions)
-        super().__init__(*args, **kwargs)
+        self.insertions = self.actions.insertions
         # Target embeddings use alternate padding.
         self.target_embeddings = self.init_embeddings(
             num_embeddings=self.output_size,
             embedding_size=self.embedding_size,
             pad_idx=self.actions.end_idx,
         )
-        self.save_hyperparameters()
 
     def forward(
-        self, batch: base.Batch
+        self,
+        batch: batches.PaddedBatch,
     ) -> Tuple[List[List[int]], torch.Tensor]:
         """Runs the encoder-decoder model.
 
         Args:
-            batch (base.Batch): batch of the input, input mask, output, and
-                output mask.
+            batch (batches.PaddedBatch).
 
         Returns:
             Tuple[List[List[int]], torch.Tensor] of encoded prediction values
                 and loss tensor; due to transducer setup, prediction is
                 performed during training, so these are returned.
         """
-        if len(batch) == 4:
-            source, source_mask, target, target_mask = batch
-        elif len(batch) == 2:
-            source, source_mask = batch
-            target = None
-            target_mask = None
-        else:
-            raise lstm.Error(f"Batch of {len(batch)} elements is invalid")
-        enc_out, _ = self.encode(source, source_mask)
+        encoder_out, _ = self.encode(batch.source)
         # Ignores start symbol.
-        enc_out = enc_out[:, 1:, :]
-        source = source[:, 1:]
-        source_mask = source_mask[:, 1:]
+        encoder_out = encoder_out[:, 1:, :]
+        source_padded = batch.source.padded[:, 1:]
+        source_mask = batch.source.mask[:, 1:]
         prediction, loss = self.decode(
-            enc_out,
-            source,
+            encoder_out,
+            source_padded,
             source_mask,
-            target=target,
-            target_mask=target_mask,
+            teacher_forcing=self.teacher_forcing if self.training else False,
+            target=batch.target.padded if batch.target else None,
+            target_mask=batch.target.mask,
         )
         return prediction, loss
 
     def decode(
         self,
-        enc_out: torch.Tensor,
+        encoder_out: torch.Tensor,
         source: torch.Tensor,
         source_mask: torch.Tensor,
+        teacher_forcing: bool,
         target: Optional[torch.Tensor] = None,
         target_mask: Optional[torch.Tensor] = None,
     ) -> Tuple[List[List[int]], torch.Tensor]:
         """Decodes a sequence given the encoded input.
 
         This essentially serves as a wrapper for looping decode_step.
 
         Args:
-            enc_out (torch.Tensor): input symbols of shape
+            encoder_out (torch.Tensor): input symbols of shape
                 B x seq_len x emb_size.
             source (torch.Tensor): encoded source input.
             source_mask (torch.Tensor): mask for source input.
+            teacher_forcing (bool): Whether or not to decode
+                with teacher forcing. Determines whether or not to rollout
+                optimal actions.
             target (torch.Tensor, optional): encoded target input.
             target_mask (torch.Tensor, optional): mask for target input.
 
         Returns:
             Tuple[List[List[int]], torch.Tensor]: encoded prediction values
                 and loss tensor; due to transducer setup, prediction is
                 performed during training, so these are returned.
         """
         batch_size = source_mask.size(dim=0)
-        input_length = (source_mask == 0).sum(dim=1).to(self.device)
+        input_length = (~source_mask).sum(dim=1)
         # Initializing values.
         alignment = torch.zeros(
-            (batch_size), device=self.device, dtype=torch.int64
+            batch_size, device=self.device, dtype=torch.int64
         )
         action_count = torch.zeros(
-            (batch_size), device=self.device, dtype=torch.int64
+            batch_size, device=self.device, dtype=torch.int64
         )
         last_action = torch.full(
             (batch_size,), self.actions.beg_idx, device=self.device
         )
-        loss = torch.zeros((batch_size), device=self.device)
+        loss = torch.zeros(batch_size, device=self.device)
         prediction = [[] for _ in range(batch_size)]
         # Converting encodings for prediction.
         if target is not None:
             # Target and source need to be integers for SED values.
             # Clips EOW (idx = -1) for source and target.
             source = [
                 s[~smask].tolist()[:-1]
                 for s, smask in zip(source, source_mask)
             ]
             target = [
                 t[~tmask].tolist()[:-1]
                 for t, tmask in zip(target, target_mask)
             ]
         # Start of decoding.
-        last_hiddens = self.init_hiddens(batch_size)
-        for _ in range(self.max_decode_len):
+        last_hiddens = self.init_hiddens(batch_size, self.decoder_layers)
+        for _ in range(self.max_target_length):
             # Checks if completed all sequences.
             not_complete = last_action != self.actions.end_idx
             if not any(not_complete):
                 break
             # Proceeds to make new edit; new action for all current decoding.
             action_count = torch.where(
-                not_complete, action_count + 1, action_count
+                not_complete.to(self.device), action_count + 1, action_count
             )
             # Decoding.
             logits, last_hiddens = self.decode_step(
-                enc_out,
+                encoder_out,
                 last_action,
                 last_hiddens,
                 alignment,
             )
             # If given targets, asks expert for optimal actions.
             optim_action = (
                 self.batch_expert_rollout(
@@ -172,62 +171,63 @@
                 else None
             )
             last_action = self.decode_action_step(
                 logits,
                 alignment,
                 input_length,
                 not_complete,
-                optim_action=optim_action,
+                optim_action=optim_action if teacher_forcing else None,
             )
             alignment = self.update_prediction(
                 last_action, source, alignment, prediction
             )
             # If target, validation or training step loss required.
             if target is not None:
                 log_sum_loss = self.log_sum_softmax_loss(logits, optim_action)
                 loss = torch.where(not_complete, log_sum_loss + loss, loss)
         avg_loss = torch.mean(loss / action_count)
         return prediction, -avg_loss
 
     def decode_step(
         self,
-        enc_out: torch.Tensor,
-        last_act: torch.Tensor,
+        encoder_out: torch.Tensor,
+        last_action: torch.Tensor,
         last_hiddens: Tuple[torch.Tensor, torch.Tensor],
         alignment: torch.Tensor,
     ) -> Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         """Performs decoding step.
 
-        Per item in batch: chooses single symbol in enc_out using alignment.
-        Symbol is concatenated with last_act and then decoded to find logits.
+        Per item in batch: chooses single symbol in encoder_out using
+        alignment. The symbol is concatenated with last_action and then
+        decoded to compute logits.
 
         Args:
-            enc_out (torch.Tensor): output from encoder of shape
+            encoder_out (torch.Tensor): output from encoder of shape
                 B x seq_len x emb_size.
-            last_act (torch.Tensor): edit action from previous decode_step of
-                shape B x seq_len x emb_size.
+            last_action (torch.Tensor): edit action from previous decode_step
+                of shape B x seq_len x emb_size.
             last_hiddens (Tuple[torch.Tensor, torch.Tensor]): previous hidden
-                states from the decoder, both of shape 1 x B x dec_dim.
+                states from the decoder, both of shape 1 x B x decoder_dim.
             alignment (torch.Tensor): index of encoding symbols for decoding,
                 per item in batch of shape B x seq_len.
 
         Returns:
             Tuple[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]: tuple of
                 (logits, hidden_state) values.
         """
         # B x seq_len -> emb_size x 1 x B -> B x 1 x emb_size.
-        alignment_expand = alignment.expand(enc_out.size(-1), 1, -1).transpose(
-            0, -1
-        )
-        char_enc_out = torch.gather(enc_out, 1, alignment_expand)
-        previous_action_embedding = self.target_embeddings(last_act).unsqueeze(
-            dim=1
-        )
+        alignment_expand = alignment.expand(
+            encoder_out.size(-1), 1, -1
+        ).transpose(0, -1)
+        char_encoder_out = torch.gather(encoder_out, 1, alignment_expand)
+        previous_action_embedding = self.target_embeddings(
+            last_action
+        ).unsqueeze(dim=1)
         decoder_input = torch.cat(
-            (char_enc_out, previous_action_embedding), dim=2
+            (char_encoder_out, previous_action_embedding), dim=2
         )
         decoder_output, (h1, c1) = self.decoder(decoder_input, last_hiddens)
         logits = self.classifier(decoder_output).squeeze(dim=1)
         return logits, (h1, c1)
 
     def decode_action_step(
         self,
@@ -240,15 +240,15 @@
         """Decodes logits to find edit action.
 
         Finds possible actions given remaining size of source input and masks
         logits for edit action decoding.
 
         Args:
             logits (torch.Tensor): logit values from decode_step of shape
-                B x output_size.
+                B x num_actions.
             alignment (torch.Tensor): index of encoding symbols for decoding,
                 per item in batch of shape B x seq_len.
             input_length (torch.Tensor): length of each item in batch.
             not_complete (torch.Tensor): boolean values designating which items
                 have not terminated edits.
             optim_actions (List[List[int]], optional): optimal actions
                 determined by expert, present when loss is being calculated.
@@ -273,15 +273,15 @@
             end_of_input (bool): indicates if this is the last input from
                 string; if true, only insertions are available.
 
         Returns:
             List[actions.Edit]: actions known by transducer.
         """
         valid_actions = [self.actions.end_idx]
-        valid_actions.extend(self.inserts)
+        valid_actions.extend(self.insertions)
         if not end_of_input:
             valid_actions.extend([self.actions.copy_idx, self.actions.del_idx])
             valid_actions.extend(self.substitutions)
         return valid_actions
 
     def action_probability_mask(
         self, logits: torch.Tensor, valid_actions: List[int]
@@ -339,15 +339,15 @@
                     ):
                         if nc:
                             optim_logs = probs[action]
                             idx = int(torch.argmax(optim_logs, 0))
                             next_action.append(action[idx])
                         else:  # Already complete, so skip.
                             next_action.append(self.actions.end_idx)
-        return torch.IntTensor(next_action)
+        return torch.tensor(next_action, device=self.device, dtype=torch.int)
 
     # TODO: Merge action classes to remove need for this method.
     @staticmethod
     def remap_actions(
         action_scores: Dict[actions.Edit, float]
     ) -> Dict[actions.Edit, float]:
         """Maps generative oracle's edit to conditional counterpart.
@@ -366,15 +366,15 @@
         for action, score in action_scores.items():
             if isinstance(action, actions.GenerativeEdit):
                 remapped_action = action.conditional_counterpart()
             elif isinstance(action, actions.Edit):
                 remapped_action = action
             else:
                 raise ActionError(
-                    f"Unknown action: {action, score}, "
+                    f"Unknown action: {action}, {score}, "
                     f"action_scores: {action_scores}"
                 )
             remapped_action_scores[remapped_action] = score
         return remapped_action_scores
 
     def expert_rollout(
         self,
@@ -395,15 +395,15 @@
             List[int]: optimal action encodings.
         """
         raw_action_scores = self.expert.score(
             source,
             target,
             alignment,
             prediction,
-            max_action_seq_len=self.max_decode_len,
+            max_action_seq_len=self.max_target_length,
         )
         action_scores = self.remap_actions(raw_action_scores)
         optimal_value = min(action_scores.values())
         optimal_action = sorted(
             [
                 self.actions.encode_unseen_action(action)
                 for action, value in action_scores.items()
@@ -447,15 +447,15 @@
            prediction (List[List[str]]): current predictions for each item in
                batch, one list of symbols per item.
 
         Return:
             torch.Tensor: new alignments for transduction.
         """
         alignment_update = torch.zeros(
-            (alignment.shape), device=self.device, dtype=torch.int64
+            alignment.shape, device=self.device, dtype=torch.int64
         )
         for i in range(len(source)):
             a = self.actions.decode(action[i])
             if isinstance(a, actions.ConditionalCopy):
                 symb = source[i][alignment[i]]
                 prediction[i].append(symb)
                 alignment_update[i] += 1
@@ -465,19 +465,20 @@
                 prediction[i].append(a.new)
             elif isinstance(a, actions.ConditionalSub):
                 alignment_update[i] += 1
                 prediction[i].append(a.new)
             elif isinstance(a, actions.End):
                 prediction[i].append(self.end_idx)
             else:
-                raise ActionError(f"Unknown action: {action}.")
+                raise ActionError(f"Unknown action: {action[i]}")
         return alignment + alignment_update
 
+    @staticmethod
     def log_sum_softmax_loss(
-        self, logits: torch.Tensor, optimal_actions: List[int]
+        logits: torch.Tensor, optimal_actions: List[int]
     ) -> torch.Tensor:
         """Computes log loss.
 
         After:
             Riezler, S. Prescher, D., Kuhn, J. and Johnson, M. 2000.
             Lexicalized stochastic modeling of constraint-based grammars using
             log-linear measures and EM training. In Proceedings of the 38th
@@ -489,60 +490,76 @@
         ]
         log_sum_exp_terms = torch.stack(
             [torch.logsumexp(act, dim=-1) for act in opt_act]
         )
         normalization_term = torch.logsumexp(logits, -1)
         return log_sum_exp_terms - normalization_term
 
-    def loss_func(
-        self,
-        prediction: Tuple[List[List[int]], torch.Tensor],
-        target: torch.Tensor,
-    ) -> torch.Tensor:
-        """Returns loss value for prediction.
+    def _get_loss_func(
+        self, reduction: str
+    ) -> Callable[[torch.Tensor, torch.Tensor], torch.Tensor]:
+        # Prevents base construction of unused loss function.
+        return None
+
+    def training_step(
+        self, batch: batches.PaddedBatch, batch_idx: int
+    ) -> Dict:
+        """Runs one step of training.
+
+        This is called by the PL Trainer.
+
+        Args:
+            batch (batches.PaddedBatch)
+            batch_idx (int).
 
-        Transducer already produces prediction strings and calculates loss
-        during training. This simply serves as a wrapper to allow compatibility
-        with training_step in superclass.
+        Returns:
+            torch.Tensor: loss.
         """
-        _, loss = prediction
+        # Forward pass produces loss by default.
+        _, loss = self(batch)
+        self.log(
+            "train_loss",
+            loss,
+            batch_size=len(batch),
+            on_step=False,
+            on_epoch=True,
+        )
         return loss
 
     def validation_step(
-        self, batch: Tuple[torch.tensor], batch_idx: int
+        self, batch: batches.PaddedBatch, batch_idx: int
     ) -> Dict:
-        preds, loss = self.forward(batch)
+        predictions, loss = self.forward(batch)
         # Evaluation requires prediction as a tensor.
-        preds = self.convert_prediction(preds)
+        predictions = self.convert_prediction(predictions)
         # Processes for accuracy calculation.
-        preds = self.evaluator.finalize_preds(
-            preds, self.end_idx, self.pad_idx, device="cpu"
+        predictions = self.evaluator.finalize_predictions(
+            predictions, self.end_idx, self.pad_idx
         )
-        target = batch[-2]
         return {
-            "val_accuracy": self.evaluator.get_accuracy(
-                preds, target, self.pad_idx
+            "val_accuracy": self.evaluator.accuracy(
+                predictions, batch.target.padded, self.pad_idx
             ),
             "val_loss": loss,
         }
 
     def predict_step(self, batch: Tuple[torch.tensor], batch_idx: int) -> Dict:
-        preds, loss = self.forward(
+        predictions, _ = self.forward(
             batch,
         )
         # Evaluation requires prediction tensor.
-        return self.convert_prediction(preds)
+        return self.convert_prediction(predictions)
 
     def convert_prediction(self, prediction: List[List[int]]) -> torch.Tensor:
         """Converts prediction values to tensor for evaluator compatibility."""
         max_len = len(max(prediction, key=len))
         for i, pred in enumerate(prediction):
             pad = [self.actions.end_idx] * (max_len - len(pred))
             pred.extend(pad)
-            prediction[i] = torch.IntTensor(pred, device="cpu")
+            prediction[i] = torch.tensor(pred, dtype=torch.int)
         return torch.stack(prediction)
 
     def on_train_epoch_start(self) -> None:
         """Scheduler for oracle."""
         self.expert.roll_in_schedule(self.current_epoch)
 
     @staticmethod
@@ -554,113 +571,79 @@
             rand -= p
             if rand <= 0:
                 break
         return action
 
 
 class TransducerFeatures(TransducerNoFeatures):
-    """Transducer model that encodes feature inputs."""
+    """Transducer model with an LSTM backend."""
 
-    features_idx: int
-    features_vocab_size: int
+    feature_embeddings: nn.Embedding
 
-    def __init__(self, features_vocab_size, features_idx, *args, **kwargs):
-        """Initializes transducer model. Uses LSTM backend.
+    def __init__(self, *args, **kwargs):
+        """Initializes transducer model.
 
         Functions equivalently to TransducerNoFeatures except concatenates
         n-hot encoding of feature values to encoded tensor.
 
         Args:
-            features_idx (int): index in data.source_symbol2i that marks
-                start of feature encodings.
+            features_idx (int): index marking the start of feature encodings.
             features_vocab_size (int): size of features vocab.
             *args: passed to superclass.
             **kwargs: passed to superclass.
         """
-        self.features_idx = features_idx
-        self.features_vocab_size = features_vocab_size
         super().__init__(*args, **kwargs)
-        # Re-initializes decoder to accomodate features.
-        self.decoder = nn.LSTM(
-            self.hidden_size * self.num_directions
-            + self.embedding_size
-            + self.features_vocab_size,
-            self.hidden_size,
-            dropout=self.dropout,
-            num_layers=self.dec_layers,
-            batch_first=True,
+        self.feature_embeddings = self.init_embeddings(
+            self.features_vocab_size, self.embedding_size, self.pad_idx
         )
-        self.features_idx = features_idx
-        self.features_vocab_size = features_vocab_size
-        super().__init__(*args, **kwargs)
-        # Re-initializes decoder to accomodate features.
+        # Overrides decoder to accomodate features.
         self.decoder = nn.LSTM(
             self.hidden_size * self.num_directions
-            + self.embedding_size
-            + self.features_vocab_size,
+            + self.embedding_size  # Hidden cells.
+            + self.embedding_size,  # Features.
             self.hidden_size,
             dropout=self.dropout,
-            num_layers=self.dec_layers,
+            num_layers=self.decoder_layers,
             batch_first=True,
         )
 
-    def forward(self, batch: base.Batch) -> torch.Tensor:
+    def forward(
+        self,
+        batch: batches.PaddedBatch,
+    ) -> torch.Tensor:
         """Runs the encoder-decoder model.
 
         Args:
-            batch (base.Batch): batch of the input, input mask, output, and
-                output mask.
+            batch (batches.PaddedBatch).
 
         Returns:
             Tuple[List[List[int]], torch.Tensor]: encoded prediction values
                 and loss tensor; due to transducer setup, prediction is
                 performed during training, so these are returned.
         """
-        if len(batch) == 6:
-            (
-                source,
-                source_mask,
-                features,
-                features_mask,
-                target,
-                target_mask,
-            ) = batch
-        elif len(batch) == 4:
-            source, source_mask, features, features_mask = batch
-            target = None
-            target_mask = None
-        else:
-            raise lstm.Error(f"Batch of {len(batch)} elements is invalid")
-        enc_out, _ = self.encode(source, source_mask)
+        encoder_out, _ = self.encode(batch.source)
         # Ignores start symbol.
-        enc_out = enc_out[:, 1:, :]
-        source = source[:, 1:]
-        source_mask = source_mask[:, 1:]
-        # Converts features to n-hot encoding.
-        with torch.no_grad():
-            # Features are offset by features idx. Shifts one to encode
-            # padding, replacing mask with first index.
-            features = torch.where(
-                features_mask, 0, features - self.features_idx + 1
-            )
-            one_hot_features = nn.functional.one_hot(
-                features, self.features_vocab_size + 1
-            )
-            # Truncates pad at idx 0 then sum one_hots for n_hot vectors.
-            n_hot_features = torch.sum(
-                one_hot_features[:, :, 1:], dim=1, keepdim=True
-            )
-        # B x 1 x n_feat -> B x seq_len x n_feat.
-        n_hot_features = n_hot_features.expand(-1, enc_out.size(1), -1)
-        # Concatenates n-hot encoding onto each symbol.
-        enc_out_feat = torch.cat((enc_out, n_hot_features), dim=2)
+        encoder_out = encoder_out[:, 1:, :]
+        source_padded = batch.source.padded[:, 1:]
+        source_mask = batch.source.mask[:, 1:]
+        # Prepares feature embeddings.
+        features_out = self.feature_embeddings(batch.features.padded)
+        features_out = torch.sum(features_out, dim=1)
+        denom = torch.sum(~batch.features.mask, dim=1, keepdim=True)
+        denom = denom.expand(-1, features_out.size(1))
+        features_out = features_out / denom
+        # Concatenates output with source encoding.
+        features_out = features_out.unsqueeze(dim=1)
+        features_out = features_out.expand(-1, source_padded.size(1), -1)
+        encoder_out_feat = torch.cat((encoder_out, features_out), dim=2)
         prediction, loss = self.decode(
-            enc_out_feat,
-            source,
+            encoder_out_feat,
+            source_padded,
             source_mask,
-            target=target,
-            target_mask=target_mask,
+            teacher_forcing=self.teacher_forcing if self.training else False,
+            target=batch.target.padded if batch.target else None,
+            target_mask=batch.target.mask,
         )
         return prediction, loss
 
 
 # TODO: Implement beam decoding.
```

### Comparing `yoyodyne-0.2.1/yoyodyne/models/transformer.py` & `yoyodyne-0.2.3/yoyodyne/models/transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,180 +1,94 @@
 """Transformer model classes."""
 
+import argparse
 import math
 from typing import Optional
 
 import torch
 from torch import nn
 
-from .. import evaluators
+from .. import batches, defaults
 from . import base, positional_encoding
 
 
-class Error(Exception):
-    pass
-
-
 class TransformerEncoderDecoder(base.BaseEncoderDecoder):
     """Transformer encoder-decoder."""
 
-    vocab_size: int
-    hidden_size: int
-    d_model: int
-    nhead: int
-    max_seq_len: int
-    enc_layers: int
-    dec_layers: int
-    pad_idx: int
-    optim_name: str
-    beta1: float
-    beta2: float
-    warmup_steps: int
-    lr: float
-    evaluator: evaluators.Evaluator
-    scheduler: str
-    start_idx: int
-    end_idx: int
-    embedding_size: int
-    output_size: int
-    dropout: float
-    dropout_layer: nn.Dropout
+    # Model arguments.
+    attention_heads: int
+    max_source_length: int
+    # Constructed inside __init__.
+    esq: float
     source_embeddings: nn.Embedding
     target_embeddings: nn.Embedding
     positional_encoding: positional_encoding.PositionalEncoding
     log_softmax: nn.LogSoftmax
     encoder: nn.TransformerEncoder
     decoder: nn.TransformerDecoder
     classifier: nn.Linear
-    max_decode_len: int
-    beam_width: Optional[int]
-    label_smoothing: Optional[float]
 
     def __init__(
         self,
-        vocab_size,
-        embedding_size,
-        hidden_size,
-        nhead,
-        max_seq_len,
-        output_size,
-        pad_idx,
-        start_idx,
-        end_idx,
-        optim,
-        beta1,
-        beta2,
-        warmup_steps,
-        lr,
-        scheduler,
-        evaluator,
-        max_decode_len,
-        dropout=0.3,
-        enc_layers=4,
-        dec_layers=4,
-        label_smoothing=None,
-        beam_width=None,
+        *args,
+        attention_heads=defaults.ATTENTION_HEADS,
+        max_source_length=defaults.MAX_SOURCE_LENGTH,
         **kwargs,
     ):
         """Initializes the encoder-decoder with attention.
 
         Args:
-            vocab_size (int).
-            embedding_size (int).
-            hidden_size (int).
-            nhead (int).
-            max_seq_len (int).
-            output_size (int).
-            pad_idx (int).
-            start_idx (int).
-            end_idx (int).
-            optim (str).
-            beta1 (float).
-            beta2 (float).
-            warmup_steps (int).
-            lr (float).
-            evaluator (evaluators.Evaluator).
-            scheduler (str).
-            max_decode_len (int).
-            dropout (float, optional).
-            enc_layers (int, optional).
-            dec_layers (int, optional).
-            label_smoothing (float, optional).
-            beam_width (int, optional): defaults to None; if True, then beam
-                search is used for decoding. This should only be used at test
-                time.
-            **kwargs: ignored.
-        """
-        super().__init__()
-        self.vocab_size = vocab_size
-        self.hidden_size = hidden_size
-        self.d_model = embedding_size
-        self.nhead = nhead
-        self.max_seq_len = max_seq_len
-        self.enc_layers = enc_layers
-        self.dec_layers = dec_layers
-        self.pad_idx = pad_idx
-        self.optim_name = optim
-        self.beta1 = beta1
-        self.beta2 = beta2
-        self.warmup_steps = warmup_steps
-        self.lr = lr
-        self.evaluator = evaluator
-        self.scheduler = scheduler
-        self.start_idx = start_idx
-        self.end_idx = end_idx
-        self.embedding_size = embedding_size
-        self.output_size = output_size
-        self.dropout = dropout
-        self.dropout_layer = nn.Dropout(p=self.dropout, inplace=False)
+            attention_heads (int).
+            max_source_length (int).
+            *args: passed to superclass.
+            **kwargs: passed to superclass.
+        """
+        super().__init__(*args, **kwargs)
+        self.attention_heads = attention_heads
+        self.max_source_length = max_source_length
+        self.esq = math.sqrt(self.embedding_size)
         self.source_embeddings = self.init_embeddings(
-            vocab_size, self.d_model, self.pad_idx
+            self.vocab_size, self.embedding_size, self.pad_idx
         )
         self.target_embeddings = self.init_embeddings(
-            output_size, self.d_model, self.pad_idx
+            self.output_size, self.embedding_size, self.pad_idx
         )
         self.positional_encoding = positional_encoding.PositionalEncoding(
-            self.d_model, self.pad_idx, self.max_seq_len
+            self.embedding_size, self.pad_idx, self.max_source_length
         )
         self.log_softmax = nn.LogSoftmax(dim=2)
-        enc_layer = nn.TransformerEncoderLayer(
-            d_model=self.d_model,
+        encoder_layer = nn.TransformerEncoderLayer(
+            d_model=self.embedding_size,
             dim_feedforward=self.hidden_size,
-            nhead=self.nhead,
+            nhead=self.attention_heads,
             dropout=self.dropout,
             activation="relu",
             norm_first=True,
             batch_first=True,
         )
         self.encoder = nn.TransformerEncoder(
-            encoder_layer=enc_layer,
-            num_layers=self.enc_layers,
-            norm=nn.LayerNorm(self.d_model),
+            encoder_layer=encoder_layer,
+            num_layers=self.encoder_layers,
+            norm=nn.LayerNorm(self.embedding_size),
         )
-        dec_layer = nn.TransformerDecoderLayer(
-            d_model=self.d_model,
+        decoder_layer = nn.TransformerDecoderLayer(
+            d_model=self.embedding_size,
             dim_feedforward=self.hidden_size,
-            nhead=self.nhead,
+            nhead=self.attention_heads,
             dropout=self.dropout,
             activation="relu",
             norm_first=True,
             batch_first=True,
         )
         self.decoder = nn.TransformerDecoder(
-            decoder_layer=dec_layer,
-            num_layers=self.dec_layers,
-            norm=nn.LayerNorm(self.d_model),
-        )
-        self.classifier = nn.Linear(self.d_model, output_size)
-        self.max_decode_len = max_decode_len
-        self.label_smoothing = label_smoothing
-        self.beam_width = beam_width
-        self.loss_func = self.get_loss_func("mean")
-        # Saves hyperparameters for PL checkpointing.
-        self.save_hyperparameters()
+            decoder_layer=decoder_layer,
+            num_layers=self.decoder_layers,
+            norm=nn.LayerNorm(self.embedding_size),
+        )
+        self.classifier = nn.Linear(self.embedding_size, self.output_size)
 
     def init_embeddings(
         self, num_embeddings: int, embedding_size: int, pad_idx: int
     ) -> nn.Embedding:
         """Initializes the embedding layer.
 
         Args:
@@ -196,17 +110,15 @@
             symbols (torch.Tensor): batch of symbols to embed of shape
                 B x seq_len.
 
         Returns:
             embedded (torch.Tensor): embedded tensor of shape
                 B x seq_len x embed_dim.
         """
-        word_embedding = self.source_embeddings(symbols) * math.sqrt(
-            self.d_model
-        )
+        word_embedding = self.esq * self.source_embeddings(symbols)
         positional_embedding = self.positional_encoding(symbols)
         out = self.dropout_layer(word_embedding + positional_embedding)
         return out
 
     def target_embed(self, symbols: torch.Tensor) -> torch.Tensor:
         """Embeds the target symbols and adds positional encodings.
 
@@ -214,183 +126,220 @@
             symbols (torch.Tensor): batch of symbols to embed of shape
                 B x seq_len.
 
         Returns:
             embedded (torch.Tensor): embedded tensor of shape
                 B x seq_len x embed_dim.
         """
-        word_embedding = self.target_embeddings(symbols) * math.sqrt(
-            self.d_model
-        )
+        word_embedding = self.esq * self.target_embeddings(symbols)
         positional_embedding = self.positional_encoding(symbols)
         out = self.dropout_layer(word_embedding + positional_embedding)
         return out
 
-    def encode(
-        self, source: torch.Tensor, source_mask: torch.Tensor
-    ) -> torch.Tensor:
+    def encode(self, source: batches.PaddedTensor) -> torch.Tensor:
         """Encodes the source with the TransformerEncoder.
 
         Args:
-            source (torch.Tensor).
-            source_mask (torch.Tensor).
+            source (batches.PaddedTensor).
 
         Returns:
             torch.Tensor: sequence of encoded symbols.
         """
-        embedding = self.source_embed(source)
-        return self.encoder(embedding, src_key_padding_mask=source_mask)
+        embedding = self.source_embed(source.padded)
+        return self.encoder(embedding, src_key_padding_mask=source.mask)
 
     def decode(
         self,
-        enc_hidden: torch.Tensor,
+        encoder_hidden: torch.Tensor,
         source_mask: torch.Tensor,
         target: torch.Tensor,
         target_mask: torch.Tensor,
     ) -> torch.Tensor:
         """Decodes the logits for each step of the output sequence.
 
         Args:
-            enc_hidden (torch.Tensor): source encoder hidden state of shape
-                                   B x seq_len x hidden_size
+            encoder_hidden (torch.Tensor): source encoder hidden state, of
+                shape B x seq_len x hidden_size.
             source_mask (torch.Tensor): encoder hidden state mask.
             target (torch.Tensor): current state of targets, which may be the
                 full target, or previous decoded, of shape
                 B x seq_len x hidden_size.
             target_mask (torch.Tensor): target mask.
 
         Returns:
             _type_: log softmax over targets.
         """
         target_embedding = self.target_embed(target)
-        target_seq_len = target_embedding.size(1)
+        target_sequence_length = target_embedding.size(1)
         # -> seq_len x seq_len.
-        causal_mask = self.generate_square_subsequent_mask(target_seq_len).to(
-            self.device
-        )
+        causal_mask = self.generate_square_subsequent_mask(
+            target_sequence_length
+        ).to(self.device)
         # -> B x seq_len x d_model
-        dec_hidden = self.decoder(
+        decoder_hidden = self.decoder(
             target_embedding,
-            enc_hidden,
+            encoder_hidden,
             tgt_mask=causal_mask,
-            tgt_key_padding_mask=target_mask,
             memory_key_padding_mask=source_mask,
+            tgt_key_padding_mask=target_mask,
         )
-        # -> B x seq_len x vocab_size.
-        output = self.classifier(dec_hidden)
+        # -> B x seq_len x output_size.
+        output = self.classifier(decoder_hidden)
         output = self.log_softmax(output)
         return output
 
     def _decode_greedy(
-        self, enc_hidden: torch.Tensor, source_mask: torch.Tensor
+        self,
+        encoder_hidden: torch.Tensor,
+        source_mask: torch.Tensor,
+        targets: Optional[torch.Tensor],
     ) -> torch.Tensor:
+        """Decodes the output sequence greedily.
+
+        Args:
+            encoder_hidden (torch.Tensor): Hidden states from the encoder.
+            source_mask (torch.Tensor): Mask for the encoded source tokens.
+            targets (torch.Tensor, optional): The optional target tokens,
+                which is only used for early stopping during validation
+                if the decoder has predicted [EOS] for every sequence in
+                the batch.
+
+        Returns:
+            torch.Tensor: predictions from the decoder.
+        """
         # The output distributions to be returned.
         outputs = []
-        batch_size = enc_hidden.size(0)
+        batch_size = encoder_hidden.size(0)
         # The predicted symbols at each iteration.
-        preds = [
+        predictions = [
             torch.tensor(
-                [self.start_idx for _ in range(enc_hidden.size(0))],
+                [self.start_idx for _ in range(encoder_hidden.size(0))],
                 device=self.device,
             )
         ]
         # Tracking when each sequence has decoded an EOS.
         finished = torch.zeros(batch_size, device=self.device)
-        for _ in range(self.max_decode_len):
-            target_tensor = torch.stack(preds, dim=1)
+        for _ in range(self.max_target_length):
+            target_tensor = torch.stack(predictions, dim=1)
             # Uses a dummy mask of all ones.
-            target_mask = torch.ones_like(
-                target_tensor, dtype=torch.float, device=self.device
-            )
+            target_mask = torch.ones_like(target_tensor, dtype=torch.float)
             target_mask = target_mask == 0
             output = self.decode(
-                enc_hidden, source_mask, target_tensor, target_mask
+                encoder_hidden, source_mask, target_tensor, target_mask
             )
             # We only care about the last prediction in the sequence.
             last_output = output[:, -1, :]
             outputs.append(last_output)
-            pred = self._get_predicted(last_output.unsqueeze(1))
-            preds.append(pred.squeeze(1))
+            # -> B x 1 x 1
+            _, pred = torch.max(last_output, dim=1)
+            predictions.append(pred)
             # Updates to track which sequences have decoded an EOS.
-            finished = torch.logical_or(finished, (preds[-1] == self.end_idx))
-            # Break when all batches predicted an EOS symbol.
+            finished = torch.logical_or(
+                finished, (predictions[-1] == self.end_idx)
+            )
+            # Breaks when all batches predicted an EOS symbol.
+            # If we have a target (and are thus computing loss),
+            # we only break when we have decoded at least the the
+            # same number of steps as the target length.
             if finished.all():
-                break
-        # -> B x vocab_size x seq_len
-        return torch.stack(outputs).transpose(0, 1).transpose(1, 2)
+                if targets is None or len(outputs) >= targets.size(-1):
+                    break
+        # -> B x seq_len x output_size.
+        return torch.stack(outputs).transpose(0, 1)
 
-    def forward(self, batch: base.Batch) -> torch.Tensor:
+    def forward(
+        self,
+        batch: batches.PaddedBatch,
+    ) -> torch.Tensor:
         """Runs the encoder-decoder.
 
         Args:
-            batch (Tuple[torch.Tensor, ...]): Tuple of tensors in the batch
-                of shape (source, source_mask, target, target_mask) during
-                training or shape (source, source_mask) during inference.
+            batch (batches.PaddedBatch).
 
         Returns:
             torch.Tensor.
         """
-        # Training mode with targets.
-        if len(batch) == 4:
-            source, source_mask, target, target_mask = batch
+        if self.training and self.teacher_forcing:
+            assert (
+                batch.target.padded is not None
+            ), "Teacher forcing requested but no target provided"
             # Initializes the start symbol for decoding.
             starts = (
-                torch.LongTensor([self.start_idx])
-                .to(self.device)
-                .repeat(target.size(0))
+                torch.tensor(
+                    [self.start_idx], device=self.device, dtype=torch.long
+                )
+                .repeat(batch.target.padded.size(0))
                 .unsqueeze(1)
             )
-            target = torch.cat((starts, target), dim=1)
+            target_padded = torch.cat((starts, batch.target.padded), dim=1)
             target_mask = torch.cat(
-                (starts == self.pad_idx, target_mask), dim=1
+                (starts == self.pad_idx, batch.target.mask), dim=1
+            )
+            encoder_hidden = self.encode(batch.source)
+            output = self.decode(
+                encoder_hidden, batch.source.mask, target_padded, target_mask
             )
-            enc_hidden = self.encode(source, source_mask)
-            output = self.decode(enc_hidden, source_mask, target, target_mask)
-            # -> B x vocab_size x seq_len
-            output = output.transpose(1, 2)[:, :, :-1]
-        # No targets given at inference.
-        elif len(batch) == 2:
-            source, source_mask = batch
-            enc_hidden = self.encode(source, source_mask)
-            # -> B x vocab_size x seq_len.
-            output = self._decode_greedy(enc_hidden, source_mask)
+            # -> B x seq_len x output_size.
+            output = output[:, :-1, :]
         else:
-            raise Error(f"Batch of {len(batch)} elements is invalid")
+            encoder_hidden = self.encode(batch.source)
+            # -> B x seq_len x output_size.
+            output = self._decode_greedy(
+                encoder_hidden,
+                batch.source.mask,
+                batch.target.padded if batch.target else None,
+            )
         return output
 
-    def generate_square_subsequent_mask(self, length: int) -> torch.Tensor:
+    @staticmethod
+    def generate_square_subsequent_mask(length: int) -> torch.Tensor:
         """Generates the target mask so the model cannot see future states.
 
         Args:
             length (int): length of the sequence.
 
         Returns:
             torch.Tensor: mask of shape length x length.
         """
-        return torch.triu(
-            torch.full((length, length), float("-inf")), diagonal=1
+        return torch.triu(torch.full((length, length), -math.inf), diagonal=1)
+
+    @staticmethod
+    def add_argparse_args(parser: argparse.ArgumentParser) -> None:
+        """Adds transformer configuration options to the argument parser.
+
+        These are only needed at training time.
+
+        Args:
+            parser (argparse.ArgumentParser).
+        """
+        parser.add_argument(
+            "--attention_heads",
+            type=int,
+            default=defaults.ATTENTION_HEADS,
+            help="Number of attention heads "
+            "(transformer-backed architectures only. Default: %(default)s.",
         )
 
 
 class FeatureInvariantTransformerEncoderDecoder(TransformerEncoderDecoder):
     """Transformer encoder-decoder with feature invariance.
 
     After:
         Wu, S., Cotterell, R., and Hulden, M. 2021. Applying the transformer to
         character-level transductions. In Proceedings of the 16th Conference of
         the European Chapter of the Association for Computational Linguistics:
         Main Volume, pages 1901-1907.
     """
 
-    features_idx: int
+    # Constructed inside __init__.
+    type_embedding: nn.Embedding
 
-    def __init__(self, *args, features_idx, **kwargs):
+    def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        # For distinguishing features vs character.
-        self.features_idx = features_idx
+        # Distinguishes features vs. character.
         self.type_embedding = self.init_embeddings(
             2, self.embedding_size, self.pad_idx
         )
 
     def source_embed(self, symbols: torch.Tensor) -> torch.Tensor:
         """Embeds the source symbols.
 
@@ -401,22 +350,20 @@
                 B x seq_len.
 
         Returns:
             embedded (torch.Tensor): embedded tensor of shape
                 B x seq_len x embed_dim.
         """
         # Distinguishes features and chars.
-        char_mask = (symbols < self.features_idx).long()
+        char_mask = (
+            symbols < (self.vocab_size - self.features_vocab_size)
+        ).long()
         # 1 or 0.
-        type_embedding = math.sqrt(self.d_model) * self.type_embedding(
-            char_mask
-        )
-        word_embedding = self.source_embeddings(symbols) * math.sqrt(
-            self.d_model
-        )
+        type_embedding = self.esq * self.type_embedding(char_mask)
+        word_embedding = self.esq * self.source_embeddings(symbols)
         positional_embedding = self.positional_encoding(
             symbols, mask=char_mask
         )
         out = self.dropout_layer(
             word_embedding + positional_embedding + type_embedding
         )
         return out
```

### Comparing `yoyodyne-0.2.1/yoyodyne.egg-info/SOURCES.txt` & `yoyodyne-0.2.3/yoyodyne.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 LICENSE.txt
 README.md
-setup.py
+pyproject.toml
 yoyodyne/__init__.py
+yoyodyne/batches.py
 yoyodyne/collators.py
+yoyodyne/dataconfig.py
 yoyodyne/datasets.py
+yoyodyne/defaults.py
 yoyodyne/evaluators.py
+yoyodyne/indexes.py
 yoyodyne/predict.py
 yoyodyne/schedulers.py
 yoyodyne/special.py
 yoyodyne/train.py
 yoyodyne/util.py
 yoyodyne.egg-info/PKG-INFO
 yoyodyne.egg-info/SOURCES.txt
```

