# Comparing `tmp/bio-attention-0.0.8.tar.gz` & `tmp/bio-attention-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio-attention-0.0.8.tar", last modified: Fri Jun 30 08:07:44 2023, max compression
+gzip compressed data, was "bio-attention-0.0.9.tar", last modified: Fri Jun 30 08:37:26 2023, max compression
```

## Comparing `bio-attention-0.0.8.tar` & `bio-attention-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.155825 bio-attention-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.147825 bio-attention-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.147825 bio-attention-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 08:07:31.000000 bio-attention-0.0.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 08:07:31.000000 bio-attention-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 08:07:31.000000 bio-attention-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:07:44.155825 bio-attention-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-30 08:07:31.000000 bio-attention-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.151825 bio-attention-0.0.8/bio_attention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17896 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/embed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.155825 bio-attention-0.0.8/bio_attention/img/
--rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/img/2Dslidingwindow-attention.png
--rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/img/windowed_implementation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-30 08:07:31.000000 bio-attention-0.0.8/bio_attention/positional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:07:44.151825 bio-attention-0.0.8/bio_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:07:44.000000 bio-attention-0.0.8/bio_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 08:07:31.000000 bio-attention-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 08:07:44.155825 bio-attention-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.067799 bio-attention-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-30 08:37:18.000000 bio-attention-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-30 08:37:18.000000 bio-attention-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-30 08:37:18.000000 bio-attention-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:37:26.067799 bio-attention-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-30 08:37:18.000000 bio-attention-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/bio_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/embed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.067799 bio-attention-0.0.9/bio_attention/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  2372654 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/img/2Dslidingwindow-attention.png
+-rw-r--r--   0 runner    (1001) docker     (123)   118589 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/img/windowed_implementation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23235 2023-06-30 08:37:18.000000 bio-attention-0.0.9/bio_attention/positional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 08:37:26.063799 bio-attention-0.0.9/bio_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 08:37:26.000000 bio-attention-0.0.9/bio_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-30 08:37:18.000000 bio-attention-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-30 08:37:26.067799 bio-attention-0.0.9/setup.cfg
```

### Comparing `bio-attention-0.0.8/.github/workflows/publish.yml` & `bio-attention-0.0.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/.gitignore` & `bio-attention-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/LICENSE` & `bio-attention-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/PKG-INFO` & `bio-attention-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `bio-attention-0.0.8/README.md` & `bio-attention-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/bio_attention/attention.py` & `bio-attention-0.0.9/bio_attention/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,14 @@
         x = self.plugin.mod_x(x, pos=pos, mask = (mask if use_mask_to_mod_x else None), **mod_kwargs)
         b, l, h = (x.size(0), x.size(-2), x.size(-1))
         q, k, v = torch.split(self.lin(x), h, dim=-1)
         q, k, v = map(
             lambda t: rearrange(t, "... (n h) -> ... n h", n=self.nh), (q, k, v)
         ) # B, *, L, NH, H
         if mask is not None:
-            assert mask.shape[-1] == q.shape[-3]
             if q.ndim - mask.ndim == 2: #B, *, L -> B, *, L, L
                 mask = repeat(mask, '... l -> ... (l2) l', l2=mask.shape[-1])
             if q.ndim - mask.ndim == 1: #B, *, L, L  -> B, *, NH, L, L
                 mask = repeat(mask, '... l1 l2 -> ... nh l1 l2', nh=q.shape[-2])
             assert mask.shape[:-3] == q.shape[:-3]
 
             if mask.dtype == torch.bool:
```

### Comparing `bio-attention-0.0.8/bio_attention/embed.py` & `bio-attention-0.0.9/bio_attention/embed.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/bio_attention/img/2Dslidingwindow-attention.png` & `bio-attention-0.0.9/bio_attention/img/2Dslidingwindow-attention.png`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/bio_attention/img/windowed_implementation.svg` & `bio-attention-0.0.9/bio_attention/img/windowed_implementation.svg`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/bio_attention/positional.py` & `bio-attention-0.0.9/bio_attention/positional.py`

 * *Files identical despite different names*

### Comparing `bio-attention-0.0.8/bio_attention.egg-info/PKG-INFO` & `bio-attention-0.0.9/bio_attention.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bio-attention
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple implementations of attention modules adapted for the biological data domain
 Home-page: https://github.com/gdewael/bio-attention
 Author: Gaetan De Waele
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

