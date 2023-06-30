# Comparing `tmp/flowMC-0.2.0.tar.gz` & `tmp/flowMC-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowMC-0.2.0.tar", last modified: Tue May  9 18:58:39 2023, max compression
+gzip compressed data, was "flowMC-0.2.1.tar", last modified: Fri Jun 30 19:31:31 2023, max compression
```

## Comparing `flowMC-0.2.0.tar` & `flowMC-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-09 18:58:28.000000 flowMC-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-09 18:58:39.528934 flowMC-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-09 18:58:28.000000 flowMC-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 18:58:28.000000 flowMC-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-09 18:58:39.528934 flowMC-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.524934 flowMC-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.524934 flowMC-0.2.0/src/flowMC/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/nfmodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/realNVP.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/rqSpline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/nfmodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/Gaussian_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/HMC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/LocalSampler_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/MALA.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/NF_proposal.py
--rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/Sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/sampler/mMALA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/PRNG_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/PythonFunctionWrap.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:28.000000 flowMC-0.2.0/src/flowMC/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 18:58:39.528934 flowMC-0.2.0/src/flowMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-09 18:58:39.000000 flowMC-0.2.0/src/flowMC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.300243 flowMC-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-30 19:31:20.000000 flowMC-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 19:31:31.300243 flowMC-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-30 19:31:20.000000 flowMC-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-30 19:31:20.000000 flowMC-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-30 19:31:31.300243 flowMC-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/flowMC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/flowMC/nfmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/realNVP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/rqSpline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/nfmodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/flowMC/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/Gaussian_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/HMC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/LocalSampler_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/MALA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/NF_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16040 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/Sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/sampler/mMALA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/flowMC/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/utils/EvolutionaryOptimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/utils/PRNG_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/utils/PythonFunctionWrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:20.000000 flowMC-0.2.1/src/flowMC/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 19:31:31.296243 flowMC-0.2.1/src/flowMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-30 19:31:31.000000 flowMC-0.2.1/src/flowMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-30 19:31:31.000000 flowMC-0.2.1/src/flowMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 19:31:31.000000 flowMC-0.2.1/src/flowMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-30 19:31:31.000000 flowMC-0.2.1/src/flowMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-30 19:31:31.000000 flowMC-0.2.1/src/flowMC.egg-info/top_level.txt
```

### Comparing `flowMC-0.2.0/LICENSE` & `flowMC-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/PKG-INFO` & `flowMC-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.2.0
+Version: 0.2.1
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
-<a href="https://flowmc.readthedocs.io/en/latest/">
+<a href="https://flowmc.readthedocs.io/en/main/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
 </a>
 <a href="https://github.com/kazewong/FlowMC/blob/Packaging/LICENSE">
 <img src="https://badgen.net/badge/License/MIT/blue" alt="doc"/>
 </a>
 
 ![flowMC_logo](./docs//source/logo_0810.png)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.2.0 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.2.1 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
-learning,normalizing,autodiff,jax Requires-Python: <3.11,>=3.8 Description-
+learning,normalizing,autodiff,jax Requires-Python: <3.11,>=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE # flowMC **Normalizing-flow
 enhanced sampling package for probabilistic inference** [doc] [doc] !
 [flowMC_logo](./docs//source/logo_0810.png) flowMC is a Jax-based python
 package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
 The code is open source under MIT license, and it is under active development.
 - Just-in-time compilation is supported. - Native support for GPU acceleration.
 - Suit for problems with multi-modality. - Minimal tuning. # Installation The
```

### Comparing `flowMC-0.2.0/README.md` & `flowMC-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
-<a href="https://flowmc.readthedocs.io/en/latest/">
+<a href="https://flowmc.readthedocs.io/en/main/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
 </a>
 <a href="https://github.com/kazewong/FlowMC/blob/Packaging/LICENSE">
 <img src="https://badgen.net/badge/License/MIT/blue" alt="doc"/>
 </a>
 
 ![flowMC_logo](./docs//source/logo_0810.png)
```

### Comparing `flowMC-0.2.0/src/flowMC/sampler/Gaussian_random_walk.py` & `flowMC-0.2.1/src/flowMC/sampler/Gaussian_random_walk.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/sampler/HMC.py` & `flowMC-0.2.1/src/flowMC/sampler/HMC.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/sampler/LocalSampler_Base.py` & `flowMC-0.2.1/src/flowMC/sampler/LocalSampler_Base.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/sampler/MALA.py` & `flowMC-0.2.1/src/flowMC/sampler/MALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/sampler/NF_proposal.py` & `flowMC-0.2.1/src/flowMC/sampler/NF_proposal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Tuple
 import jax
 import jax.numpy as jnp
 from jax import random, jit, vmap
 from tqdm import tqdm
-
+from flowMC.nfmodel.base import NFModel
+from jaxtyping import Array, PRNGKeyArray, PyTree
+from typing import Callable
 n_sample_max = 100000
 
-
 def nf_metropolis_kernel(
     rng_key: jax.random.PRNGKey,
     proposal_position: jnp.ndarray,
     initial_position: jnp.ndarray,
     log_proposal_pdf: jnp.ndarray,
     log_proposal_nf_pdf: jnp.ndarray,
     log_initial_pdf: jnp.ndarray,
@@ -41,29 +42,26 @@
     u = jnp.log(jax.random.uniform(subkeys, ratio.shape))
     do_accept = u < ratio
     position = jnp.where(do_accept, proposal_position, initial_position)
     log_prob = jnp.where(do_accept, log_proposal_pdf, log_initial_pdf)
     log_prob_nf = jnp.where(do_accept, log_proposal_nf_pdf, log_initial_nf_pdf)
     return position, log_prob, log_prob_nf, do_accept
 
-
 nf_metropolis_kernel = vmap(nf_metropolis_kernel)
 
 
 @jax.jit
 def nf_metropolis_update(i: int, state: Tuple):
     """
     A multistep global sampling kernel for a given normalizing flow model.
 
     Args:
         i: Number of current iteration.
         state: A tuple containing the current state of the sampler.
-
     """
-
     (
         key,
         positions,
         proposal,
         log_prob,
         log_prob_nf,
         log_prob_proposal,
@@ -95,142 +93,102 @@
         log_prob_nf,
         log_prob_proposal,
         log_prob_nf_proposal,
         acceptance,
     )
 
 
-def make_nf_metropolis_sampler(nf_model):
-    """
-    Make the normalizing flow sampler for a given normalizing flow model 
-    for multiple steps and from multiple initial positions.
+def nf_metropolis_sampler(nf_model: NFModel,
+                        rng_key: PRNGKeyArray,
+                        n_steps: int,
+                        target_pdf: Callable,
+                        initial_position: Array,
+                        data: PyTree,
+):
+    r""" Normalizing flow Metropolis sampler.
 
     Args:
-        nf_model: A normalizing flow model.
-        
-    Returns:
-        nf_metropolis_sampler: A normalizing flow sampler that has the following signature:
-
-            Args:
-                rng_key: Jax PRNGKey.
-                n_steps: Number of steps.
-                nf_param: Normalizing flow parameters.
-                nf_variables: Normalizing flow variables.
-                target_pdf: Target pdf.
-                initial_position: Initial position.
-                data: Data.
-
-            Returns:
-                rng_key: Current state of random key
-                all_positions: All positions of the chain
-                all_logp: Log probability of the target function at all positions
-                all_logp_nf: Log probability of the normalizing flow model at all positions
-                acceptance: Acceptance boolean
+        nf_model: Normalizing flow model.
+        rng_key: Jax PRNGKey.
+        n_steps: Number of steps to run the sampler.
+        target_pdf: Target pdf function.
+        initial_position: Initial position of the sampler.
+        data: Data to be passed to the target pdf function.
+    """
+
+    rng_key, *subkeys = random.split(rng_key, 3)
+
+    total_sample = initial_position.shape[0] * n_steps
+
+    log_pdf_nf_initial = nf_model.log_prob(initial_position)
+    log_pdf_initial = target_pdf(initial_position, data)
+
+    if total_sample > n_sample_max:
+        proposal_position = jnp.zeros((total_sample, initial_position.shape[-1]))
+        log_pdf_nf_proposal = jnp.zeros((total_sample,))
+        log_pdf_proposal = jnp.zeros((total_sample,))
+        local_key, subkey = random.split(subkeys[0], 2)
+        for i in tqdm(
+            range(total_sample // n_sample_max),
+            desc="Sampling Globally",
+            miniters=(total_sample // n_sample_max) // 10,
+        ):
+            local_samples = nf_model.sample(subkey, n_sample_max)
+            proposal_position = proposal_position.at[
+                i * n_sample_max : (i + 1) * n_sample_max
+            ].set(local_samples)
+            log_pdf_nf_proposal = log_pdf_nf_proposal.at[
+                i * n_sample_max : (i + 1) * n_sample_max
+            ].set(nf_model.log_prob(local_samples))
+            log_pdf_proposal = log_pdf_proposal.at[
+                i * n_sample_max : (i + 1) * n_sample_max
+            ].set(target_pdf(local_samples, data))
+            local_key, subkey = random.split(local_key, 2)
+
+    else:
+        proposal_position = nf_model.sample(subkeys[0], total_sample)
+        log_pdf_nf_proposal = nf_model.log_prob(proposal_position)
+        log_pdf_proposal = target_pdf(proposal_position, data)
 
-    """
+    proposal_position = proposal_position.reshape(
+        n_steps, initial_position.shape[0], initial_position.shape[1]
+    )
+    log_pdf_nf_proposal = log_pdf_nf_proposal.reshape(
+        n_steps, initial_position.shape[0]
+    )
+    log_pdf_proposal = log_pdf_proposal.reshape(n_steps, initial_position.shape[0])
 
-    @jax.jit
-    def eval_nf_logprob(position, nf_params, nf_variables):
-        return nf_model.apply(
-            {"params": nf_params, "variables": nf_variables},
-            position,
-            method=nf_model.log_prob,
-        )
-
-    def sample_nf(rng_key, n_samples, nf_params, nf_variables):
-        return nf_model.apply(
-            {"params": nf_params, "variables": nf_variables},
-            rng_key,
-            n_samples,
-            method=nf_model.sample,
-        )
-
-    sample_nf = jax.jit(sample_nf, static_argnums=(1))
-
-    def nf_metropolis_sampler(
-        rng_key, n_steps, nf_param, nf_variables, target_pdf, initial_position, data
-    ):
-        rng_key, *subkeys = random.split(rng_key, 3)
-
-        total_sample = initial_position.shape[0] * n_steps
-
-        log_pdf_nf_initial = eval_nf_logprob(
-            initial_position, nf_param, nf_variables
-        )
-        log_pdf_initial = target_pdf(initial_position, data)
-
-        if total_sample > n_sample_max:
-            proposal_position = jnp.zeros((total_sample, initial_position.shape[-1]))
-            log_pdf_nf_proposal = jnp.zeros((total_sample,))
-            log_pdf_proposal = jnp.zeros((total_sample,))
-            local_key, subkey = random.split(subkeys[0], 2)
-            for i in tqdm(
-                range(total_sample // n_sample_max),
-                desc="Sampling Globally",
-                miniters=(total_sample // n_sample_max) // 10,
-            ):
-                local_samples = sample_nf(subkey, n_sample_max, nf_param, nf_variables)
-                proposal_position = proposal_position.at[
-                    i * n_sample_max : (i + 1) * n_sample_max
-                ].set(local_samples)
-                log_pdf_nf_proposal = log_pdf_nf_proposal.at[
-                    i * n_sample_max : (i + 1) * n_sample_max
-                ].set(eval_nf_logprob(local_samples, nf_param, nf_variables))
-                log_pdf_proposal = log_pdf_proposal.at[
-                    i * n_sample_max : (i + 1) * n_sample_max
-                ].set(target_pdf(local_samples, data))
-                local_key, subkey = random.split(local_key, 2)
-
-        else:
-            proposal_position = sample_nf(
-                subkeys[0], total_sample, nf_param, nf_variables
-            )
-            log_pdf_nf_proposal = eval_nf_logprob(
-                proposal_position, nf_param, nf_variables
-            )
-            log_pdf_proposal = target_pdf(proposal_position, data)
-
-        proposal_position = proposal_position.reshape(
-            n_steps, initial_position.shape[0], initial_position.shape[1]
-        )
-        log_pdf_nf_proposal = log_pdf_nf_proposal.reshape(
-            n_steps, initial_position.shape[0]
-        )
-        log_pdf_proposal = log_pdf_proposal.reshape(n_steps, initial_position.shape[0])
-
-        all_positions = (
-            jnp.zeros((n_steps,) + initial_position.shape) + initial_position
-        )
-        all_logp = jnp.zeros((n_steps, initial_position.shape[0])) + log_pdf_initial
-        all_logp_nf = (
-            jnp.zeros((n_steps, initial_position.shape[0])) + log_pdf_nf_initial
-        )
-        acceptance = jnp.zeros((n_steps, initial_position.shape[0]))
-
-        initial_state = (
-            subkeys[1],
-            all_positions,
-            proposal_position,
-            all_logp,
-            all_logp_nf,
-            log_pdf_proposal,
-            log_pdf_nf_proposal,
-            acceptance,
-        )
-        (
-            rng_key,
-            all_positions,
-            proposal_position,
-            all_logp,
-            all_logp_nf,
-            log_pdf_proposal,
-            log_pdf_nf_proposal,
-            acceptance,
-        ) = jax.lax.fori_loop(1, n_steps, nf_metropolis_update, initial_state)
-        all_positions = all_positions.swapaxes(0, 1)
-        all_logp = all_logp.swapaxes(0, 1)
-        all_logp_nf = all_logp_nf.swapaxes(0, 1)
-        acceptance = acceptance.swapaxes(0, 1)
+    all_positions = (
+        jnp.zeros((n_steps,) + initial_position.shape) + initial_position
+    )
+    all_logp = jnp.zeros((n_steps, initial_position.shape[0])) + log_pdf_initial
+    all_logp_nf = (
+        jnp.zeros((n_steps, initial_position.shape[0])) + log_pdf_nf_initial
+    )
+    acceptance = jnp.zeros((n_steps, initial_position.shape[0]))
 
-        return rng_key, all_positions, all_logp, all_logp_nf, acceptance
+    initial_state = (
+        subkeys[1],
+        all_positions,
+        proposal_position,
+        all_logp,
+        all_logp_nf,
+        log_pdf_proposal,
+        log_pdf_nf_proposal,
+        acceptance,
+    )
+    (
+        rng_key,
+        all_positions,
+        proposal_position,
+        all_logp,
+        all_logp_nf,
+        log_pdf_proposal,
+        log_pdf_nf_proposal,
+        acceptance,
+    ) = jax.lax.fori_loop(1, n_steps, nf_metropolis_update, initial_state)
+    all_positions = all_positions.swapaxes(0, 1)
+    all_logp = all_logp.swapaxes(0, 1)
+    all_logp_nf = all_logp_nf.swapaxes(0, 1)
+    acceptance = acceptance.swapaxes(0, 1)
 
-    return nf_metropolis_sampler
+    return rng_key, all_positions, all_logp, all_logp_nf, acceptance
```

### Comparing `flowMC-0.2.0/src/flowMC/sampler/Sampler.py` & `flowMC-0.2.1/src/flowMC/sampler/Sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,68 @@
 from logging import lastResort
 from typing import Callable, Tuple
-import jax
 import jax.numpy as jnp
-import numpy as np
-from flowMC.nfmodel.utils import sample_nf, make_training_loop, eval_nf
-from flowMC.sampler.NF_proposal import make_nf_metropolis_sampler
-from flax.training import train_state  # Useful dataclass to keep train state
-import flax
+from flowMC.nfmodel.utils import make_training_loop
+from flowMC.sampler.NF_proposal import nf_metropolis_sampler
 import optax
 from flowMC.sampler.LocalSampler_Base import LocalSamplerBase
+from flowMC.nfmodel.base import NFModel
 from tqdm import tqdm
+import equinox as eqx
 
 
 class Sampler():
     """
     Sampler class that host configuration parameters, NF model, and local sampler
 
     Args:
         n_dim (int): Dimension of the problem.
         rng_key_set (Tuple): Tuple of random number generator keys.
+        data (Device Array): Extra data to be passed to the likelihood function.
         local_sampler (Callable): Local sampler maker
-        sampler_params (dict): Parameters for the local sampler.
-        likelihood (Callable): Likelihood function.
-        nf_model (Callable): Normalizing flow model.
-        n_loop_training (int, optional): Number of training loops. Defaults to 2.
-        n_loop_production (int, optional): Number of production loops. Defaults to 2.
-        n_local_steps (int, optional): Number of local steps per loop. Defaults to 5.
-        n_global_steps (int, optional): Number of global steps per loop. Defaults to 5.
-        n_chains (int, optional): Number of chains. Defaults to 5.
-        n_epochs (int, optional): Number of epochs per training loop. Defaults to 5.
+        nf_model (NFModel): Normalizing flow model.
+        n_loop_training (int, optional): Number of training loops. Defaults to 3.
+        n_loop_production (int, optional): Number of production loops. Defaults to 3.
+        n_local_steps (int, optional): Number of local steps per loop. Defaults to 50.
+        n_global_steps (int, optional): Number of global steps per loop. Defaults to 50.
+        n_chains (int, optional): Number of chains. Defaults to 20.
+        n_epochs (int, optional): Number of epochs per training loop. Defaults to 30.
         learning_rate (float, optional): Learning rate for the NF model. Defaults to 0.01.
         max_samples (int, optional): Maximum number of samples fed to training the NF model. Defaults to 10000.
         momentum (float, optional): Momentum for the NF model. Defaults to 0.9.
-        batch_size (int, optional): Batch size for the NF model. Defaults to 10.
+        batch_size (int, optional): Batch size for the NF model. Defaults to 10000.
         use_global (bool, optional): Whether to use global sampler. Defaults to True.
         logging (bool, optional): Whether to log the training process. Defaults to True.
-        nf_variable (None, optional): Mean and variance variables for the NF model. Defaults to None.
         keep_quantile (float, optional): Quantile of chains to keep when training the normalizing flow model. Defaults to 0..
         local_autotune (None, optional): Auto-tune function for the local sampler. Defaults to None.
         train_thinning (int, optional): Thinning for the data used to train the normalizing flow. Defaults to 1.
-        model_init (dic, optional): Dictionary with keys "params" and "variables" for the NF model. Defaults to None.
     """
 
     def __init__(
         self,
         n_dim: int,
         rng_key_set: Tuple,
         data: jnp.ndarray,
         local_sampler: LocalSamplerBase,
-        nf_model: Callable,
+        nf_model: NFModel,
         n_loop_training: int = 3,
         n_loop_production: int = 3,
         n_local_steps: int = 50,
         n_global_steps: int = 50,
         n_chains: int = 20,
         n_epochs: int = 30,
         learning_rate: float = 0.01,
         max_samples: int = 10000,
         momentum: float = 0.9,
         batch_size: int = 10000,
         use_global: bool = True,
         logging: bool = True,
-        nf_variable=None,
-        keep_quantile=0,
-        local_autotune=None,
-        train_thinning = 1,
-        model_init = None,
+        keep_quantile: float = 0,
+        local_autotune: Callable = None,
+        train_thinning: int = 1,
     ):
         rng_key_init, rng_keys_mcmc, rng_keys_nf, init_rng_keys_nf = rng_key_set
 
         # Copying input into the model
 
         self.rng_keys_nf = rng_keys_nf
         self.rng_keys_mcmc = rng_keys_mcmc
@@ -84,39 +77,29 @@
         self.max_samples = max_samples
         self.momentum = momentum
         self.batch_size = batch_size
         self.use_global = use_global
         self.logging = logging
         self.keep_quantile = keep_quantile
         self.train_thinning = train_thinning
+        self.variables = {"mean": None, "var": None}
 
         # Initialized local and global samplers
 
         self.local_sampler_class = local_sampler
         self.local_sampler_class.precompilation(n_chains=n_chains, n_dims=n_dim, n_step=n_local_steps, data=data)
         self.local_sampler = self.local_sampler_class.sampler
 
         self.local_autotune = local_autotune
         self.likelihood_vec = self.local_sampler_class.logpdf_vmap
         self.nf_model = nf_model
-        if model_init is None:
-            model_init = nf_model.init(init_rng_keys_nf, jnp.ones((1, self.n_dim)))
-        params = model_init["params"]
-        self.variables = model_init["variables"]
-        if nf_variable is not None:
-            self.variables = self.variables
-        self.global_sampler = make_nf_metropolis_sampler(self.nf_model)
-        
-        self.nf_training_loop, train_epoch, train_step = make_training_loop(
-            self.nf_model
-        )
+        # self.global_sampler = make_nf_metropolis_sampler(self.nf_model)
+
         tx = optax.adam(self.learning_rate, self.momentum)
-        self.state = train_state.TrainState.create(
-            apply_fn=nf_model.apply, params=params, tx=tx
-        )
+        self.nf_training_loop, train_epoch, train_step = make_training_loop(tx)
 
         # Initialized result dictionary
         training = {}
         training["chains"] = jnp.empty((self.n_chains, 0, self.n_dim))
         training["log_prob"] = jnp.empty((self.n_chains, 0))
         training["local_accs"] = jnp.empty((self.n_chains, 0))
         training["global_accs"] = jnp.empty((self.n_chains, 0))
@@ -191,14 +174,16 @@
         )
 
         if self.use_global == True:
             if training == True:
                 positions = self.summary['training']['chains'][:,::self.train_thinning]
                 log_prob_output = self.summary['training']['log_prob'][:,::self.train_thinning]
 
+
+
                 if self.keep_quantile > 0:
                     max_log_prob = jnp.max(log_prob_output, axis=1)
                     cut = jnp.quantile(max_log_prob, self.keep_quantile)
                     cut_chains = positions[max_log_prob > cut]
                 else:
                     cut_chains = positions
                 chain_size = cut_chains.shape[0] * cut_chains.shape[1]
@@ -210,42 +195,41 @@
                     flat_chain = cut_chains.reshape(-1, self.n_dim)
 
                 if flat_chain.shape[0] < self.max_samples:
                     # This is to pad the training data to avoid recompilation.
                     flat_chain = jnp.repeat(flat_chain, (self.max_samples // flat_chain.shape[0])+1, axis=0)
                     flat_chain = flat_chain[:self.max_samples]
 
-                variables = self.variables.unfreeze()
-                variables["base_mean"] = jnp.mean(flat_chain, axis=0)
-                variables["base_cov"] = jnp.cov(flat_chain.T)
-                self.variables = flax.core.freeze(variables)
+                self.variables["mean"] = jnp.mean(flat_chain, axis=0)
+                self.variables["cov"] = jnp.cov(flat_chain.T)
+                self.nf_model = eqx.tree_at(lambda m: m._data_mean, self.nf_model, self.variables["mean"])
+                self.nf_model = eqx.tree_at(lambda m: m._data_cov, self.nf_model, self.variables["cov"])
 
-                self.rng_keys_nf, self.state, loss_values = self.nf_training_loop(
+                self.rng_keys_nf, self.nf_model, loss_values = self.nf_training_loop(
                     self.rng_keys_nf,
-                    self.state,
-                    self.variables,
+                    self.nf_model,
                     flat_chain,
                     self.n_epochs,
                     self.batch_size,
+                    self.logging
                 )
                 self.summary['training']['loss_vals'] = jnp.append(
                     self.summary['training']['loss_vals'], loss_values.reshape(1, -1), axis=0
                 )
 
             (
                 self.rng_keys_nf,
                 nf_chain,
                 log_prob,
                 log_prob_nf,
                 global_acceptance,
-            ) = self.global_sampler(
+            ) = nf_metropolis_sampler(
+                self.nf_model,
                 self.rng_keys_nf,
                 self.n_global_steps,
-                self.state.params,
-                self.variables,
                 self.likelihood_vec,
                 positions[:, -1],
                 data,
             )
 
             self.summary[summary_mode]['chains'] = jnp.append(
                 self.summary[summary_mode]['chains'], nf_chain, axis=1
@@ -350,39 +334,28 @@
         Args:
             n_samples (int): Number of samples to generate.
 
         Returns:
             Device Array: Samples generated using the normalizing flow.
         """
 
-        nf_samples = sample_nf(
-            self.nf_model,
-            self.state.params,
-            self.rng_keys_nf,
-            n_samples,
-            self.variables,
-        )
-        return nf_samples
+        samples = self.nf_model.sample(self.rng_keys_nf, n_samples)
+        return samples
 
     def evalulate_flow(self, samples: jnp.ndarray) -> jnp.ndarray:
         """
         Evaluate the log probability of the normalizing flow.
 
         Args:
             samples (Device Array): Samples to evaluate.
 
         Returns:
             Device Array: Log probability of the samples.
         """
-        log_prob = eval_nf(
-            self.nf_model,
-            self.state.params,
-            samples,
-            self.variables,
-        )
+        log_prob = self.nf_model.log_prob(samples)
         return log_prob
 
     def reset(self):
         """
         Reset the sampler state.
 
         """
```

### Comparing `flowMC-0.2.0/src/flowMC/sampler/mMALA.py` & `flowMC-0.2.1/src/flowMC/sampler/mMALA.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/utils/PRNG_keys.py` & `flowMC-0.2.1/src/flowMC/utils/PRNG_keys.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC/utils/PythonFunctionWrap.py` & `flowMC-0.2.1/src/flowMC/utils/PythonFunctionWrap.py`

 * *Files identical despite different names*

### Comparing `flowMC-0.2.0/src/flowMC.egg-info/PKG-INFO` & `flowMC-0.2.1/src/flowMC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: flowMC
-Version: 0.2.0
+Version: 0.2.1
 Summary: Normalizing flow exhanced sampler in jax
 Home-page: https://github.com/kazewong/flowMC
 Author: Kaze Wong, Marylou Gabrié, Dan Foreman-Mackey
 Author-email: kazewong.physics@gmail.com
 License: MIT
 Keywords: sampling,inference,machine learning,normalizing,autodiff,jax
-Requires-Python: <3.11,>=3.8
+Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flowMC
 
 **Normalizing-flow enhanced sampling package for probabilistic inference**
 
-<a href="https://flowmc.readthedocs.io/en/latest/">
+<a href="https://flowmc.readthedocs.io/en/main/">
 <img src="https://badgen.net/badge/Read/the doc/blue" alt="doc"/>
 </a>
 <a href="https://github.com/kazewong/FlowMC/blob/Packaging/LICENSE">
 <img src="https://badgen.net/badge/License/MIT/blue" alt="doc"/>
 </a>
 
 ![flowMC_logo](./docs//source/logo_0810.png)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: flowMC Version: 0.2.0 Summary: Normalizing flow
+Metadata-Version: 2.1 Name: flowMC Version: 0.2.1 Summary: Normalizing flow
 exhanced sampler in jax Home-page: https://github.com/kazewong/flowMC Author:
 Kaze Wong, Marylou GabriÃ©, Dan Foreman-Mackey Author-email:
 kazewong.physics@gmail.com License: MIT Keywords: sampling,inference,machine
-learning,normalizing,autodiff,jax Requires-Python: <3.11,>=3.8 Description-
+learning,normalizing,autodiff,jax Requires-Python: <3.11,>=3.9 Description-
 Content-Type: text/markdown License-File: LICENSE # flowMC **Normalizing-flow
 enhanced sampling package for probabilistic inference** [doc] [doc] !
 [flowMC_logo](./docs//source/logo_0810.png) flowMC is a Jax-based python
 package for normalizing-flow enhanced Markov chain Monte Carlo (MCMC) sampling.
 The code is open source under MIT license, and it is under active development.
 - Just-in-time compilation is supported. - Native support for GPU acceleration.
 - Suit for problems with multi-modality. - Minimal tuning. # Installation The
```

### Comparing `flowMC-0.2.0/src/flowMC.egg-info/SOURCES.txt` & `flowMC-0.2.1/src/flowMC.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,22 +5,25 @@
 src/flowMC/__init__.py
 src/flowMC.egg-info/PKG-INFO
 src/flowMC.egg-info/SOURCES.txt
 src/flowMC.egg-info/dependency_links.txt
 src/flowMC.egg-info/requires.txt
 src/flowMC.egg-info/top_level.txt
 src/flowMC/nfmodel/__init__.py
+src/flowMC/nfmodel/base.py
+src/flowMC/nfmodel/common.py
 src/flowMC/nfmodel/mlp.py
 src/flowMC/nfmodel/realNVP.py
 src/flowMC/nfmodel/rqSpline.py
 src/flowMC/nfmodel/utils.py
 src/flowMC/sampler/Gaussian_random_walk.py
 src/flowMC/sampler/HMC.py
 src/flowMC/sampler/LocalSampler_Base.py
 src/flowMC/sampler/MALA.py
 src/flowMC/sampler/NF_proposal.py
 src/flowMC/sampler/Sampler.py
 src/flowMC/sampler/__init__.py
 src/flowMC/sampler/mMALA.py
+src/flowMC/utils/EvolutionaryOptimizer.py
 src/flowMC/utils/PRNG_keys.py
 src/flowMC/utils/PythonFunctionWrap.py
 src/flowMC/utils/__init__.py
```

