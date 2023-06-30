# Comparing `tmp/latentis-0.0.1.tar.gz` & `tmp/latentis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentis-0.0.1.tar", last modified: Fri Jun 23 01:58:50 2023, max compression
+gzip compressed data, was "latentis-0.0.2.tar", last modified: Fri Jun 30 19:54:43 2023, max compression
```

## Comparing `latentis-0.0.1.tar` & `latentis-0.0.2.tar`

### file list

```diff
@@ -1,43 +1,40 @@
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/
--rw-r--r--   0 valentino  (1000) valentino  (1000)      314 2023-06-17 23:37:40.000000 latentis-0.0.1/.editorconfig
--rw-r--r--   0 valentino  (1000) valentino  (1000)      108 2023-06-17 23:37:40.000000 latentis-0.0.1/.env.template
--rw-r--r--   0 valentino  (1000) valentino  (1000)      142 2023-06-17 23:37:40.000000 latentis-0.0.1/.flake8
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/.github/
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/.github/workflows/
--rw-r--r--   0 valentino  (1000) valentino  (1000)     5346 2023-06-23 01:49:12.000000 latentis-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 valentino  (1000) valentino  (1000)     4689 2023-06-17 23:37:40.000000 latentis-0.0.1/.github/workflows/test_suite.yml
--rw-r--r--   0 valentino  (1000) valentino  (1000)     3677 2023-06-17 23:37:40.000000 latentis-0.0.1/.gitignore
--rw-r--r--   0 valentino  (1000) valentino  (1000)     4126 2023-06-17 23:37:40.000000 latentis-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1090 2023-06-17 23:37:40.000000 latentis-0.0.1/LICENSE
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1574 2023-06-23 01:58:50.581584 latentis-0.0.1/PKG-INFO
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1171 2023-06-23 01:57:37.000000 latentis-0.0.1/README.md
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/data/
--rw-r--r--   0 valentino  (1000) valentino  (1000)       15 2023-06-17 23:37:40.000000 latentis-0.0.1/data/.gitignore
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/docs/
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1428 2023-06-17 23:53:19.000000 latentis-0.0.1/docs/index.md
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/docs/overrides/
--rw-r--r--   0 valentino  (1000) valentino  (1000)      190 2023-06-17 23:37:40.000000 latentis-0.0.1/docs/overrides/main.html
--rw-r--r--   0 valentino  (1000) valentino  (1000)      167 2023-06-18 01:17:12.000000 latentis-0.0.1/env.yaml
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1718 2023-06-17 23:52:52.000000 latentis-0.0.1/mkdocs.yml
--rw-r--r--   0 valentino  (1000) valentino  (1000)      854 2023-06-20 14:54:37.000000 latentis-0.0.1/pyproject.toml
--rw-r--r--   0 valentino  (1000) valentino  (1000)      883 2023-06-23 01:58:50.584918 latentis-0.0.1/setup.cfg
--rw-r--r--   0 valentino  (1000) valentino  (1000)      561 2023-06-20 22:27:50.000000 latentis-0.0.1/setup.py
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/src/
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/src/latentis/
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1213 2023-06-18 00:22:14.000000 latentis-0.0.1/src/latentis/__init__.py
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/src/latentis/relative/
--rw-r--r--   0 valentino  (1000) valentino  (1000)        0 2023-06-18 00:42:07.000000 latentis-0.0.1/src/latentis/relative/__init__.py
--rw-r--r--   0 valentino  (1000) valentino  (1000)     7417 2023-06-23 01:49:03.000000 latentis-0.0.1/src/latentis/relative/projection.py
--rw-r--r--   0 valentino  (1000) valentino  (1000)     6051 2023-06-18 02:11:21.000000 latentis-0.0.1/src/latentis/relative/space.py
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/src/latentis/translate/
--rw-r--r--   0 valentino  (1000) valentino  (1000)        0 2023-06-18 00:41:59.000000 latentis-0.0.1/src/latentis/translate/__init__.py
--rw-r--r--   0 valentino  (1000) valentino  (1000)     5921 2023-06-18 00:40:56.000000 latentis-0.0.1/src/latentis/translate/translation.py
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/src/latentis.egg-info/
--rw-r--r--   0 valentino  (1000) valentino  (1000)     1574 2023-06-23 01:58:50.000000 latentis-0.0.1/src/latentis.egg-info/PKG-INFO
--rw-r--r--   0 valentino  (1000) valentino  (1000)      691 2023-06-23 01:58:50.000000 latentis-0.0.1/src/latentis.egg-info/SOURCES.txt
--rw-r--r--   0 valentino  (1000) valentino  (1000)        1 2023-06-23 01:58:50.000000 latentis-0.0.1/src/latentis.egg-info/dependency_links.txt
--rw-r--r--   0 valentino  (1000) valentino  (1000)        1 2023-06-20 15:16:44.000000 latentis-0.0.1/src/latentis.egg-info/not-zip-safe
--rw-r--r--   0 valentino  (1000) valentino  (1000)      292 2023-06-23 01:58:50.000000 latentis-0.0.1/src/latentis.egg-info/requires.txt
--rw-r--r--   0 valentino  (1000) valentino  (1000)        9 2023-06-23 01:58:50.000000 latentis-0.0.1/src/latentis.egg-info/top_level.txt
-drwxr-xr-x   0 valentino  (1000) valentino  (1000)        0 2023-06-23 01:58:50.581584 latentis-0.0.1/tests/
--rw-r--r--   0 valentino  (1000) valentino  (1000)        0 2023-06-17 23:37:40.000000 latentis-0.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-06-30 19:49:17.000000 latentis-0.0.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-30 19:49:17.000000 latentis-0.0.2/.env.template
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-30 19:49:17.000000 latentis-0.0.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.672421 latentis-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     5538 2023-06-30 19:49:17.000000 latentis-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4689 2023-06-30 19:49:17.000000 latentis-0.0.2/.github/workflows/test_suite.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3677 2023-06-30 19:49:17.000000 latentis-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     4126 2023-06-30 19:49:17.000000 latentis-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-30 19:49:17.000000 latentis-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-06-30 19:54:43.676421 latentis-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1180 2023-06-30 19:49:17.000000 latentis-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-30 19:49:17.000000 latentis-0.0.2/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-06-30 19:49:17.000000 latentis-0.0.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-30 19:49:17.000000 latentis-0.0.2/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-06-30 19:54:31.000000 latentis-0.0.2/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1718 2023-06-30 19:49:17.000000 latentis-0.0.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-06-30 19:49:17.000000 latentis-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-06-30 19:54:43.676421 latentis-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-30 19:49:17.000000 latentis-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.672421 latentis-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/src/latentis/
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-30 19:49:17.000000 latentis-0.0.2/src/latentis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/src/latentis/relative/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-30 19:49:17.000000 latentis-0.0.2/src/latentis/relative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5826 2023-06-30 19:49:17.000000 latentis-0.0.2/src/latentis/relative/projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5241 2023-06-30 19:49:17.000000 latentis-0.0.2/src/latentis/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (122)      372 2023-06-30 19:49:17.000000 latentis-0.0.2/src/latentis/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 19:54:43.676421 latentis-0.0.2/src/latentis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 19:52:31.000000 latentis-0.0.2/src/latentis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-30 19:54:43.000000 latentis-0.0.2/src/latentis.egg-info/top_level.txt
```

### Comparing `latentis-0.0.1/.github/workflows/publish.yml` & `latentis-0.0.2/.github/workflows/publish.yml`

 * *Files 7% similar despite different names*

```diff
@@ -96,18 +96,18 @@
         run: |
           echo "Installed Python: $(python --version)"
           echo "Expected: ${{ matrix.python-version }}"
           python --version | grep "Python ${{ matrix.python-version }}"
 
       # https://stackoverflow.com/questions/70520120/attributeerror-module-setuptools-distutils-has-no-attribute-version
       # https://github.com/pytorch/pytorch/pull/69904
-      - name: Downgrade setuptools due to a but in PyTorch 1.10.1
-        shell: bash -l {0}
-        run: |
-          pip install setuptools==59.5.0 --upgrade
+      # - name: Downgrade setuptools due to a but in PyTorch 1.10.1
+      #   shell: bash -l {0}
+      #   run: |
+      #     pip install setuptools==59.5.0 --upgrade
 
       - name: Update conda environment
         run: mamba env update -n ${{ env.PY_CONDA_ENV_NAME }} -f ${{ env.CONDA_ENV_FILE }}
         if: steps.conda_cache.outputs.cache-hit != 'true'
 
       # Update pip env whether or not there was a conda cache hit
       - name: Update pip environment
@@ -116,39 +116,45 @@
         if: steps.conda_cache.outputs.cache-hit == 'true'
 
       - run: pip3 list
         shell: bash -l {0}
       - run: mamba info
       - run: mamba list
 
-       # Ensure the hack for the python version worked
+      # Ensure the hack for the python version worked
       - name: Ensure we have the right Python
         shell: bash -l {0}
         run: |
           echo "Installed Python: $(python --version)"
           echo "Expected: ${{ matrix.python-version }}"
           python --version | grep "Python ${{ matrix.python-version }}"
 
       - name: Run pre-commits
         shell: bash -l {0}
         run: |
           pre-commit install
           pre-commit run -v --all-files --show-diff-on-failure
 
-      - name: Test with pytest
-        shell: bash -l {0}
-        run: |
-          pytest -v
+      # - name: Test with pytest
+      #   shell: bash -l {0}
+      #   run: |
+      #     pytest -v
+
+      # - name: Build docs website
+      #   shell: bash -l {0}
+      #   run: |
+      #     git config user.name ci-bot
+      #     git config user.email ci-bot@ci.com
+      #     mike deploy --rebase --push --update-aliases ${RELEASE_TAG_VERSION} latest
 
-      - name: Build docs website
-        shell: bash -l {0}
-        run: |
-          git config user.name ci-bot
-          git config user.email ci-bot@ci.com
-          mike deploy --rebase --push --update-aliases ${RELEASE_TAG_VERSION} latest
+      - name: Check working directory status
+        run: git status
+
+      - name: Restore working directory (env.yaml Python version)
+        run: git checkout .
 
       - name: Build SDist and wheel
         run: pipx run build
 
       - name: Check metadata
         run: pipx run twine check dist/*
```

### Comparing `latentis-0.0.1/.github/workflows/test_suite.yml` & `latentis-0.0.2/.github/workflows/test_suite.yml`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/.gitignore` & `latentis-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/.pre-commit-config.yaml` & `latentis-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/LICENSE` & `latentis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/PKG-INFO` & `latentis-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for analyzing and transforming neural latent spaces.
 Home-page: https://github.com/flegyas/latentis
 Author: Valentino Maiorca
 Author-email: valentino@maiorca.xyz
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # Latentis
 
 <img align="center" alt="CI" src="https://img.shields.io/github/workflow/status/flegyas/latentis/Test%20Suite/main?label=main%20checks">
 <img align="center" alt="Docs" src="https://img.shields.io/github/deployments/flegyas/latentis/github-pages?label=docs">
 <img align="center" alt="NN Template" src="https://shields.io/badge/nn--template-0.2.3-emerald?style=flat&amp;labelColor=gray">
 <img align="center" alt="Python" src="https://img.shields.io/badge/python-3.10-blue.svg">
-<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000
+<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 
 A Python package for analyzing and transforming neural latent spaces.
 
 
 ## Installation
 
 ```bash
```

### Comparing `latentis-0.0.1/README.md` & `latentis-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Latentis
 
 <img align="center" alt="CI" src="https://img.shields.io/github/workflow/status/flegyas/latentis/Test%20Suite/main?label=main%20checks">
 <img align="center" alt="Docs" src="https://img.shields.io/github/deployments/flegyas/latentis/github-pages?label=docs">
 <img align="center" alt="NN Template" src="https://shields.io/badge/nn--template-0.2.3-emerald?style=flat&amp;labelColor=gray">
 <img align="center" alt="Python" src="https://img.shields.io/badge/python-3.10-blue.svg">
-<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000
+<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 
 A Python package for analyzing and transforming neural latent spaces.
 
 
 ## Installation
 
 ```bash
```

### Comparing `latentis-0.0.1/docs/index.md` & `latentis-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/mkdocs.yml` & `latentis-0.0.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/pyproject.toml` & `latentis-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -33,7 +33,11 @@
 
 [tool.bandit]
 skips = ["B101"]
 
 [build-system]
 requires = ["setuptools", "wheel", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
+
+[tool.setuptools_scm]
+write_to = "src/latentis/_version.py"
+write_to_template = '__version__ = "{version}"'
```

### Comparing `latentis-0.0.1/setup.cfg` & `latentis-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/src/latentis/__init__.py` & `latentis-0.0.2/src/latentis/__init__.py`

 * *Files identical despite different names*

### Comparing `latentis-0.0.1/src/latentis/relative/projection.py` & `latentis-0.0.2/src/latentis/relative/projection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
-from typing import Callable, Optional, Sequence, Tuple
+from typing import Optional, Sequence
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
-TransformType = Callable[[torch.Tensor, torch.Tensor], Tuple[torch.Tensor, torch.Tensor]]
+from latentis.types import TransformType
 
 
 class RelativeProjection(nn.Module):
     def __init__(self, name: str, func: TransformType) -> None:
         super().__init__()
         self._name: str = name
         self.func: TransformType = func
@@ -26,44 +26,28 @@
     return torch.linalg.lstsq(anchors.T, x.T)[0].T
 
 
 def cosine_dist(
     x: torch.Tensor,
     anchors: torch.Tensor,
 ) -> torch.Tensor:
-    x_norm = torch.norm(x, dim=-1)
-    anchors_norm = torch.norm(anchors, dim=-1)
-
-    # if the norm is already 1, then the cosine distance is just the dot product
-    if not torch.allclose(x_norm, torch.ones_like(x_norm)) or not torch.allclose(
-        anchors_norm, torch.ones_like(anchors_norm)
-    ):
-        x = x / x_norm.unsqueeze(-1)
-        anchors = anchors / anchors_norm.unsqueeze(-1)
+    x = F.normalize(x, p=2, dim=-1)
+    anchors = F.normalize(anchors, p=2, dim=-1)
 
     return x @ anchors.T
 
 
 def geodesic_dist(
     x: torch.Tensor,
     anchors: torch.Tensor,
 ) -> torch.Tensor:
-    x_norm = torch.norm(x, dim=-1)
-    anchors_norm = torch.norm(anchors, dim=-1)
-
-    # if the norm is already 1, then the cosine distance is just the dot product
-    if not torch.allclose(x_norm, torch.ones_like(x_norm)) or not torch.allclose(
-        anchors_norm, torch.ones_like(anchors_norm)
-    ):
-        x = x / x_norm.unsqueeze(-1)
-        anchors = anchors / anchors_norm.unsqueeze(-1)
-
-    cos_dists = x @ anchors.T
+    x = F.normalize(x, p=2, dim=-1)
+    anchors = F.normalize(anchors, p=2, dim=-1)
 
-    return torch.arccos(cos_dists)
+    return 1 - torch.arccos(x @ anchors.T)
 
 
 def lp_dist(
     x: torch.Tensor,
     anchors: torch.Tensor,
     p: int,
 ) -> torch.Tensor:
@@ -73,105 +57,61 @@
 def euclidean_dist(
     x: torch.Tensor,
     anchors: torch.Tensor,
 ) -> torch.Tensor:
     return lp_dist(x=x, anchors=anchors, p=2)
 
 
-def centering(x: torch.Tensor, anchors: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-    anchor_mean: torch.Tensor = anchors.mean(dim=0)
-    return x - anchor_mean
-
-
-def std_scaling(x: torch.Tensor, anchors: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-    anchor_std: torch.Tensor = anchors.std(dim=0)
-    return x / anchor_std
-
-
-def standard_scaling(x: torch.Tensor, anchors: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
-    return std_scaling(*centering(x=x, anchors=anchors))
-
-
-class Transform(nn.Module):
-    def __init__(self, name: str) -> None:
-        super().__init__()
-        self._name: str = name
-        self.fit_data = {"std_anchors": ..., "mean_anchors": ...}
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    def fit(self, x: torch.Tensor, *args, **kwargs) -> None:
-        raise NotImplementedError
-
-    def forward(self, x: torch.Tensor, *args, **kwargs) -> torch.Tensor:
-        raise NotImplementedError
-
-    def __repr__(self):
-        return f"{self.__class__.__name__}(name={self.name})"
-
-
-# TODO: Convert to Transform modules for efficiency
-class Transforms:
-    CENTERING = centering
-    STD_SCALING = std_scaling
-    STANDARD_SCALING = standard_scaling
-    L2 = lambda x, anchors: F.normalize(x, p=2, dim=-1)  # noqa E731
-
-
 class Projections:
     COSINE = RelativeProjection(name="cosine", func=cosine_dist)
     GEODESIC = RelativeProjection(name="geodesic", func=geodesic_dist)
     COB = RelativeProjection(name="change_of_basis", func=change_of_basis)
     EUCLIDEAN = RelativeProjection(name="euclidean", func=euclidean_dist)
     L1 = RelativeProjection(name="l1", func=functools.partial(lp_dist, p=1))
 
 
 class RelativeProjector(nn.Module):
     # TODO: Add support for anchor optimization
     def __init__(
         self,
         projection: RelativeProjection,
-        abs_transforms: Sequence[TransformType] | None = None,
-        rel_transforms: Sequence[TransformType] | None = None,
+        anchors: Optional[torch.Tensor] = None,
+        abs_transforms: Optional[Sequence[TransformType]] = None,
+        rel_transforms: Optional[Sequence[TransformType]] = None,
     ) -> None:
         super().__init__()
         self.projection: TransformType = projection
 
-        self.abs_transforms = (
+        self.abs_transforms = nn.ModuleList(
             abs_transforms
             if isinstance(abs_transforms, Sequence)
             else []
             if abs_transforms is None
             else [abs_transforms]
         )
-        self.rel_transforms = (
+        self.rel_transforms = nn.ModuleList(
             rel_transforms
             if isinstance(rel_transforms, Sequence)
             else []
             if rel_transforms is None
             else [rel_transforms]
         )
 
-    def set_anchors(self, anchors: torch.Tensor) -> None:
-        orig_anchors = anchors.clone()
-        self.register_buffer("orig_anchors", orig_anchors)
-
-        for abs_transform in self.abs_transforms:
-            anchors = abs_transform(x=anchors, anchors=anchors)
+        if anchors is not None:
+            self.register_buffer("anchors", anchors)
 
+    def set_anchors(self, anchors: torch.Tensor) -> "RelativeProjector":
         self.register_buffer("anchors", anchors)
         return self
 
     @property
     def name(self) -> str:
         return self._name
 
-    def forward(self, x: torch.Tensor, anchors: Optional[torch.Tensor]) -> torch.Tensor:
+    def forward(self, x: torch.Tensor, anchors: Optional[torch.Tensor] = None) -> torch.Tensor:
         assert anchors is not None or self.anchors is not None, "anchors must be provided"
         anchors = anchors if anchors is not None else self.anchors
 
         # absolute normalization/transformation
         transformed_x = x
         transformed_anchors = anchors
         for abs_transform in self.abs_transforms:
@@ -191,34 +131,42 @@
 
 
 class PointWiseProjector(RelativeProjector):
     def __init__(
         self,
         name: str,
         func: TransformType,
-        abs_transforms: Sequence[TransformType] | None = None,
-        rel_transforms: Sequence[TransformType] | None = None,
+        anchors: Optional[torch.Tensor] = None,
+        abs_transforms: Optional[Sequence[TransformType]] = None,
+        rel_transforms: Optional[Sequence[TransformType]] = None,
     ) -> None:
-        super().__init__(name=name, projection=func, abs_transforms=abs_transforms, rel_transforms=rel_transforms)
+        super().__init__(
+            name=name, projection=func, anchors=anchors, abs_transforms=abs_transforms, rel_transforms=rel_transforms
+        )
+
+    def forward(self, x: torch.Tensor, anchors: Optional[torch.Tensor] = None) -> torch.Tensor:
+        assert anchors is not None or self.anchors is not None, "anchors must be provided"
+        anchors = anchors if anchors is not None else self.anchors
 
-    def forward(self, x: torch.Tensor, anchors: torch.Tensor) -> torch.Tensor:
         # absolute normalization/transformation
         transformed_x = x
+        transformed_anchors = anchors
         for abs_transform in self.abs_transforms:
             transformed_x = abs_transform(x=transformed_x, anchors=anchors)
+            transformed_anchors = abs_transform(x=transformed_anchors, anchors=anchors)
 
-        transformed_anchors = abs_transform(x=anchors, anchors=anchors)
-
+        # relative projection of x with respect to the anchors
         rel_x = []
         for point in x:
             partial_rel_data = []
             for anchor in transformed_anchors:
                 partial_rel_data.append(self.projection(x=point, anchors=anchor))
             rel_x.append(partial_rel_data)
         rel_x = torch.as_tensor(rel_x, dtype=anchors.dtype, device=anchors.device)
 
         # relative normalization/transformation
         for rel_transform in self.rel_transforms:
-            # todo: handle the case where the rel_transform needs additional arguments (e.g. rel_anchors, x, ...)
+            # TODO: handle the case where the rel_transform needs additional arguments (e.g. rel_anchors, x, ...)
+            # maybe with a custom Compose object with kwargs
             rel_x = rel_transform(x=rel_x, anchors=anchors)
 
         return rel_x
```

### Comparing `latentis-0.0.1/src/latentis.egg-info/PKG-INFO` & `latentis-0.0.2/src/latentis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentis
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for analyzing and transforming neural latent spaces.
 Home-page: https://github.com/flegyas/latentis
 Author: Valentino Maiorca
 Author-email: valentino@maiorca.xyz
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # Latentis
 
 <img align="center" alt="CI" src="https://img.shields.io/github/workflow/status/flegyas/latentis/Test%20Suite/main?label=main%20checks">
 <img align="center" alt="Docs" src="https://img.shields.io/github/deployments/flegyas/latentis/github-pages?label=docs">
 <img align="center" alt="NN Template" src="https://shields.io/badge/nn--template-0.2.3-emerald?style=flat&amp;labelColor=gray">
 <img align="center" alt="Python" src="https://img.shields.io/badge/python-3.10-blue.svg">
-<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000
+<img align="center" alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
 
 A Python package for analyzing and transforming neural latent spaces.
 
 
 ## Installation
 
 ```bash
```

### Comparing `latentis-0.0.1/src/latentis.egg-info/SOURCES.txt` & `latentis-0.0.2/src/latentis.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 setup.py
 .github/workflows/publish.yml
 .github/workflows/test_suite.yml
 data/.gitignore
 docs/index.md
 docs/overrides/main.html
 src/latentis/__init__.py
+src/latentis/_version.py
+src/latentis/transforms.py
+src/latentis/types.py
 src/latentis.egg-info/PKG-INFO
 src/latentis.egg-info/SOURCES.txt
 src/latentis.egg-info/dependency_links.txt
 src/latentis.egg-info/not-zip-safe
 src/latentis.egg-info/requires.txt
 src/latentis.egg-info/top_level.txt
 src/latentis/relative/__init__.py
-src/latentis/relative/projection.py
-src/latentis/relative/space.py
-src/latentis/translate/__init__.py
-src/latentis/translate/translation.py
-tests/__init__.py
+src/latentis/relative/projection.py
```

