# Comparing `tmp/bio-attention-0.0.7.tar.gz` & `tmp/bio-attention-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.7.tar", last modified: Wed Jun 28 15:12:03 2023, max compression
+gzip compressed data, was "bio-attention-0.0.8.tar", last modified: Fri Jun 30 08:07:44 2023, max compression
```

## Comparing `bio-attention-0.0.7.tar` & `bio-attention-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.890345 bio-attention-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.882345 bio-attention-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.886345 bio-attention-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-28 15:11:54.000000 bio-attention-0.0.7/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-28 15:11:54.000000 bio-attention-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-28 15:11:54.000000 bio-attention-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-28 15:12:03.890345 bio-attention-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-28 15:11:54.000000 bio-attention-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.886345 bio-attention-0.0.7/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16898 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.890345 bio-attention-0.0.7/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22849 2023-06-28 15:11:54.000000 bio-attention-0.0.7/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:12:03.886345 bio-attention-0.0.7/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-28 15:12:03.000000 bio-attention-0.0.7/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-28 15:12:03.000000 bio-attention-0.0.7/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:12:03.000000 bio-attention-0.0.7/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-28 15:12:03.000000 bio-attention-0.0.7/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 15:12:03.000000 bio-attention-0.0.7/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-28 15:11:54.000000 bio-attention-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-28 15:12:03.890345 bio-attention-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.155825 bio-attention-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.147825 bio-attention-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.147825 bio-attention-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 08:07:31.000000 bio-attention-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 08:07:31.000000 bio-attention-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 08:07:31.000000 bio-attention-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:07:44.155825 bio-attention-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-30 08:07:31.000000 bio-attention-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.151825 bio-attention-0.0.8/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17896 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.155825 bio-attention-0.0.8/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.151825 bio-attention-0.0.8/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 08:07:31.000000 bio-attention-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 08:07:44.155825 bio-attention-0.0.8/setup.cfg
```

### Comparing `bio-attention-0.0.7/.github/workflows/publish.yml` & `bio-attention-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/.gitignore` & `bio-attention-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/LICENSE` & `bio-attention-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/PKG-INFO` & `bio-attention-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bio-attention-0.0.7/README.md` & `bio-attention-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/bio_attention/attention.py` & `bio-attention-0.0.8/bio_attention/attention.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from torch import nn, einsum
-from einops import rearrange
+from einops import rearrange, repeat
 import torch.nn.functional as F
 import math
 from bio_attention import positional
 
 
 def compl_mod(m, n):
     return int(n * math.ceil(m / n) - m)
@@ -270,14 +270,16 @@
         causal : bool, optional
             whether to do causal attention or not, by default False
 
         Returns
         -------
         _type_
             _description_
+
+        NOTE: incompatible with user-defined masks
         """
         assert mask is None
 
         assert k.shape[-3] == q.shape[-3], "q and k should have same input length."
 
         q_shape = q.shape
         q, k, v = map(lambda t: rearrange(t, "b ... x n h -> (b ...) x n h"), (q, k, v))
@@ -367,34 +369,50 @@
         self.lin = nn.Linear(dim, 3 * dim)
         self.attn = attn
         self.nh = nh
 
         self.plugin = plugin if plugin is not None else positional.Base()
 
     def forward(self, x, pos=None, mask=None, causal=False, **mod_kwargs):
-        x = self.plugin.mod_x(x, pos=pos, **mod_kwargs)
+        """
+        MASK = is used by mod_x - type positional embeddings if it is of bool type and shape B, *, L
+        MASK can be (B,*,L), (B,*,L,L), or (B,, * NH, L, L).
+        """
+        use_mask_to_mod_x = False
+        if mask is not None:
+            use_mask_to_mod_x = (mask.dtype == torch.bool) and (mask.shape == x.shape[:-1])
+        x = self.plugin.mod_x(x, pos=pos, mask = (mask if use_mask_to_mod_x else None), **mod_kwargs)
         b, l, h = (x.size(0), x.size(-2), x.size(-1))
         q, k, v = torch.split(self.lin(x), h, dim=-1)
         q, k, v = map(
             lambda t: rearrange(t, "... (n h) -> ... n h", n=self.nh), (q, k, v)
-        )
+        ) # B, *, L, NH, H
+        if mask is not None:
+            assert mask.shape[-1] == q.shape[-3]
+            if q.ndim - mask.ndim == 2: #B, *, L -> B, *, L, L
+                mask = repeat(mask, '... l -> ... (l2) l', l2=mask.shape[-1])
+            if q.ndim - mask.ndim == 1: #B, *, L, L  -> B, *, NH, L, L
+                mask = repeat(mask, '... l1 l2 -> ... nh l1 l2', nh=q.shape[-2])
+            assert mask.shape[:-3] == q.shape[:-3]
+
+            if mask.dtype == torch.bool:
+                mask = (~mask).to(q).masked_fill(~mask, -float('inf'))
 
         mod_kwargs |= {"pos_q_k": pos}
 
         q, k, v = self.plugin.mod_qkv(q, k, v, **mod_kwargs)
 
         mask = self.plugin.mod_mask(mask, q, k, v, **mod_kwargs)
 
         return rearrange(
             self.attn(q, k, v, mask=mask, causal=causal),
             "... n h -> ... (n h)",
             n=self.nh,
         )
 
-
 class Residual(nn.Module):
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
     def forward(self, x, *args, **kwargs):
         return self.fn(x, *args, **kwargs) + x
```

### Comparing `bio-attention-0.0.7/bio_attention/embed.py` & `bio-attention-0.0.8/bio_attention/embed.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.8/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.0.8/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.7/bio_attention/positional.py` & `bio-attention-0.0.8/bio_attention/positional.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """
         Args:
             x (torch.tensor): (B,*,L,H)
             pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
             mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
-
+            
         Returns:
             torch.tensor: x with added sinusoidal embeddings.
         """
         shp = list(x.shape)
         l = shp[-2]
         assert shp[-1] == self.dim
 
@@ -72,37 +72,40 @@
 
         sinusoid_inp = self.apply_pos_division(pos_emb.unsqueeze(-1) * self.inv_freq)
         pos_emb = (
             torch.stack((sinusoid_inp.sin(), sinusoid_inp.cos()), dim=-1)
             .view(*shp)
             .to(x.dtype)
         )
+
         if mask is not None:
+            assert mask.dtype == torch.bool
+            mask = F.pad(mask, (pos_emb.shape[-2]-mask.shape[-1], 0), value=True)
             pos_emb = pos_emb * mask.unsqueeze(-1)
 
         if l != shp[-2]:
             pos_emb = F.pad(pos_emb, (0, 0, l-shp[-2], 0))
 
         return x + pos_emb
 
 
 class LearnedVocab(Base):
     def __init__(self, dim, max_seq_len):
         """Learned vocab as in Devlin et al. (2018)
-        Supports specifying positions and masking.
+        Supports specifying positions.
         Only works for discrete positional indices.
 
         Args:
             dim (int): Hidden size of the embeddings
             max_seq_len (int): maximum sequence length or vocab size of the learned embeddings
         """
         super().__init__()
         self.emb = nn.Embedding(max_seq_len, dim)
 
-    def mod_x(self, x, pos=None, mask=None, **kwargs):
+    def mod_x(self, x, pos=None, mask = None, **kwargs):
         """
         Args:
             x (torch.tensor): (B,*,L,H)
             pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
             mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
@@ -111,28 +114,31 @@
             torch.tensor: x with added learned embeddings.
         """
         shp = list(x.shape)
         assert shp[-1] == self.emb.embedding_dim
         pos = self.default_pos_x(x).long() if pos is None else pos
 
         pos_emb = self.emb(pos)
+
         if mask is not None:
+            assert mask.dtype == torch.bool
+            mask = F.pad(mask, (pos_emb.shape[-2]-mask.shape[-1], 0), value=True)
             pos_emb = pos_emb * mask.unsqueeze(-1)
 
         l = pos_emb.shape[-2]
         if l != shp[-2]:
             pos_emb = F.pad(pos_emb, (0, 0, shp[-2]-l, 0))
 
         return x + pos_emb
 
 
 class LearnedContinuous(Base):
     def __init__(self, dim, depth=3, norm=False, divide=1.0, learned_div=False):
         """Learned embeddings with a continuity between absolute positional indices, as learned by a series of linear layers.
-        Supports specifying positions, masking, and division of positional range.
+        Supports specifying positions, and division of positional range.
 
         Args:
             dim (int): Hidden size of the embeddings
             depth (int, optional): number of hidden layers in the positional embedding network. Defaults to 3
             norm (bool, optional): Whether to use layernorms in the MLP. Defaults to False
             divide (float, optional): divide positions by this factor, useful for large (or small) numerical ranges. Defaults to 1.0.
             learned_div (bool, optional): Whether to learn the division factor. Defaults to False.
@@ -160,26 +166,29 @@
         """
         Args:
             x (torch.tensor): (B,*,L,H)
             pos (torch.tensor, optional): (B,*,L). Defaults to None for computing positions from 0 to L-1
             mask (torch.tensor, optional): (B,*,L). A boolean mask to indicate where positions should not have positional encodings added.
                 Defaults to None for no masking
             **kwargs: ignored. Kept for compatibility.
+            
         Returns:
             torch.tensor: x with added learned embeddings.
         """
         shp = list(x.shape)
 
         pos = self.default_pos_x(x).to(x) if pos is None else pos
 
         pos_emb = self.apply_pos_division(pos).unsqueeze(-1)
         for layer in self.mlp:
             pos_emb = layer(pos_emb)
 
         if mask is not None:
+            assert mask.dtype == torch.bool
+            mask = F.pad(mask, (pos_emb.shape[-2]-mask.shape[-1], 0), value=True)
             pos_emb = pos_emb * mask.unsqueeze(-1)
 
         l = pos_emb.shape[-2]
         if l != shp[-2]:
             pos_emb = F.pad(pos_emb, (0, 0, shp[-2]-l, 0))
 
         return x + pos_emb
```

### Comparing `bio-attention-0.0.7/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.0.8/bio_attention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.7
+Version: 0.0.8
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

