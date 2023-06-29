# Comparing `tmp/zeno_build-0.0.2.tar.gz` & `tmp/zeno_build-0.0.3.tar.gz`

## Comparing `zeno_build-0.0.2.tar` & `zeno_build-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,51 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/__init__.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/cache_utils.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/version.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/__init__.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/capitalization.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/exact_match.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/frequency.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_features/length.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_metrics/__init__.py
--rw-r--r--   0        0        0    16370 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/evaluation/text_metrics/critique.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/experiment_run.py
--rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/experiments/search_space.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/__init__.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/chat_generate.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/dataset_config.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/global_models.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/lm_config.py
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/text_generate.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/__init__.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/cohere_utils.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/huggingface_utils.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/models/providers/openai_utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/base.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/exhaustive.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/random.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/standard.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/optimizers/vizier.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/__init__.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/chat_prompt.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/prompts/prompt_utils.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/__init__.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/aggregate_results.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/reporting_utils.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 zeno_build-0.0.2/zeno_build/reporting/visualize.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.2/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.2/LICENSE
--rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 zeno_build-0.0.2/README.md
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 zeno_build-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/cache_utils.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/version.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/__init__.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/audio_metrics/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/audio_metrics/error.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/__init__.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/code_metrics/execution_accuracy_utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/__init__.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/capitalization.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/clustering.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/exact_match.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/frequency.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/length.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_features/numbers.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_metrics/__init__.py
+-rw-r--r--   0        0        0    16437 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_metrics/critique.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_tokenizers/__init__.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/evaluation/text_tokenizers/unicode.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/experiment_run.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/experiments/search_space.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/__init__.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/chat_generate.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/dataset_config.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/global_models.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/lm_config.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/text_generate.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/__init__.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/cohere_utils.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/huggingface_utils.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/models/providers/openai_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/__init__.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/base.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/exhaustive.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/random.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/standard.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/optimizers/vizier.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/__init__.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/chat_prompt.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/prompts/prompt_utils.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/__init__.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/aggregate_results.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/reporting_utils.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 zeno_build-0.0.3/zeno_build/reporting/visualize.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 zeno_build-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zeno_build-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 zeno_build-0.0.3/README.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 zeno_build-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 zeno_build-0.0.3/PKG-INFO
```

### Comparing `zeno_build-0.0.2/zeno_build/evaluation/text_features/capitalization.py` & `zeno_build-0.0.3/zeno_build/evaluation/text_features/capitalization.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/evaluation/text_features/exact_match.py` & `zeno_build-0.0.3/zeno_build/evaluation/text_features/exact_match.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/evaluation/text_features/frequency.py` & `zeno_build-0.0.3/zeno_build/evaluation/text_features/frequency.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from zeno import DistillReturn, ZenoOptions, distill
 
 
 def _count_max_word_freq(string: Any) -> int:
     """Count max word frequency in a single string."""
     if not isinstance(string, str):
         raise TypeError(f"Input must be a string but got {type(string)} for {string}.")
-    return max(Counter(string.split()).values())
+    tokens = string.split()
+    if not tokens:
+        return 0
+    else:
+        return max(Counter(tokens).values())
 
 
 @distill
 def input_max_word_freq(df: DataFrame, ops: ZenoOptions) -> DistillReturn:
     """Max frequency of words in the input.
 
     Args:
```

### Comparing `zeno_build-0.0.2/zeno_build/evaluation/text_features/length.py` & `zeno_build-0.0.3/zeno_build/evaluation/text_features/length.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/evaluation/text_metrics/critique.py` & `zeno_build-0.0.3/zeno_build/evaluation/text_metrics/critique.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import os
 
 import tqdm
 from inspiredco.critique import Critique
 from inspiredco.critique_utils.exceptions import CritiqueError
 from pandas import DataFrame
+from requests.exceptions import ConnectionError
 from zeno import DistillReturn, MetricReturn, ZenoOptions, distill, metric
 
 
 def call_critique(
     df: DataFrame,
     ops: ZenoOptions,
     metric_name: str,
@@ -63,15 +64,15 @@
                     metric=metric_name,
                     config=config,
                     dataset=eval_dict[i : i + batch_size],
                 )
                 for r in result["examples"]:
                     all_results.append(round(r["value"], 6))
                 break
-            except CritiqueError:
+            except (CritiqueError, ConnectionError):
                 if j == 2:
                     raise
                 else:
                     logging.warning(f"Error evaluating {metric_name}, retrying...")
 
     return DistillReturn(distill_output=all_results)
```

### Comparing `zeno_build-0.0.2/zeno_build/experiments/search_space.py` & `zeno_build-0.0.3/zeno_build/experiments/search_space.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Search space for hyperparameter optimization."""
 
 from __future__ import annotations
 
+import itertools
 import json
 import os
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar
 
 T = TypeVar("T")
@@ -91,14 +92,19 @@
     """A search space for hyperparameter optimization."""
 
     @abstractmethod
     def contains_params(self, params: dict[str, Any]) -> bool:
         """Check whether the search space contains the given parameters."""
         ...
 
+    @abstractmethod
+    def get_non_constant_dimensions(self) -> list[str]:
+        """Get the names of the non-constant dimensions."""
+        ...
+
     def get_valid_param_files(
         self, output_dir: str, include_in_progress: bool
     ) -> list[str]:
         """Get the valid parameter files in the given directory.
 
         Args:
             output_dir: The directory where the parameter files are stored.
@@ -144,14 +150,18 @@
         for k, v in params.items():
             if k not in self.dimensions:
                 return False
             if not self.dimensions[k].value_in_scope(v):
                 return False
         return True
 
+    def get_non_constant_dimensions(self) -> list[str]:
+        """See base class."""
+        return [k for k, v in self.dimensions.items() if not isinstance(v, Constant)]
+
 
 class CompositeSearchSpace(SearchSpace):
     """A search space consisting of multiple search spaces."""
 
     def __init__(self, spaces: list[SearchSpace], weights: list[float] | None = None):
         """Initialize the search space.
 
@@ -162,7 +172,19 @@
         """
         self.spaces = spaces
         self.weights = weights or [1.0 / len(spaces)] * len(spaces)
 
     def contains_params(self, params: dict[str, Any]) -> bool:
         """Check if the parameters are contained in the search space."""
         return any([s.contains_params(params) for s in self.spaces])
+
+    def get_non_constant_dimensions(self) -> list[str]:
+        """See base class."""
+        return sorted(
+            list(
+                set(
+                    itertools.chain.from_iterable(
+                        s.get_non_constant_dimensions() for s in self.spaces
+                    )
+                )
+            )
+        )
```

### Comparing `zeno_build-0.0.2/zeno_build/models/chat_generate.py` & `zeno_build-0.0.3/zeno_build/models/chat_generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
     context_length: int,
-    requests_per_minute: int = 300,
+    requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from a list of chat-style prompts.
 
     Args:
         variables: The variables to be replaced in the prompt template.
         prompt_template: The template for the prompt.
         api_based_model_config: The API-based model configuration.
```

### Comparing `zeno_build-0.0.2/zeno_build/models/dataset_config.py` & `zeno_build-0.0.3/zeno_build/models/dataset_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/models/lm_config.py` & `zeno_build-0.0.3/zeno_build/models/lm_config.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/models/text_generate.py` & `zeno_build-0.0.3/zeno_build/models/text_generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 
 import openai
 import tqdm
 
 from zeno_build.models import global_models, lm_config
+from zeno_build.models.providers.huggingface_utils import text_generate_from_huggingface
 from zeno_build.prompts.prompt_utils import replace_variables
 
 
 async def generate_from_text_prompt(
     variables: list[dict[str, str]],
     prompt_template: str,
     model_config: lm_config.LMConfig,
@@ -30,15 +31,24 @@
     Returns:
         The generated text.
     """
     print(
         f"Generating with {prompt_template=}, {model_config.model=}, "
         f"{temperature=}, {max_tokens=}, {top_p=}..."
     )
-    if model_config.provider == "openai":
+    if model_config.provider == "huggingface":
+        return text_generate_from_huggingface(
+            variables,
+            prompt_template,
+            model_config,
+            temperature,
+            max_tokens,
+            top_p,
+        )
+    elif model_config.provider == "openai":
         async_responses = [
             openai.Completion.acreate(
                 engine=model_config.model,
                 prompt=replace_variables(prompt_template, vars),
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
```

### Comparing `zeno_build-0.0.2/zeno_build/models/providers/cohere_utils.py` & `zeno_build-0.0.3/zeno_build/models/providers/cohere_utils.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/models/providers/openai_utils.py` & `zeno_build-0.0.3/zeno_build/models/providers/openai_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,29 +34,50 @@
                     top_p=top_p,
                 )
             except openai.error.RateLimitError:
                 logging.warning(
                     "OpenAI API rate limit exceeded. Sleeping for 10 seconds."
                 )
                 await asyncio.sleep(10)
+            except asyncio.exceptions.TimeoutError:
+                logging.warning("OpenAI API timeout. Sleeping for 10 seconds.")
+                await asyncio.sleep(10)
+            except openai.error.InvalidRequestError:
+                logging.warning("OpenAI API Invalid Request: Prompt was filtered")
+                return {
+                    "choices": [
+                        {"message": {"content": "Invalid Request: Prompt was filtered"}}
+                    ]
+                }
+            except openai.error.APIConnectionError:
+                logging.warning(
+                    "OpenAI API Connection Error: Error Communicating with OpenAI"
+                )
+                await asyncio.sleep(10)
+            except openai.error.Timeout:
+                logging.warning("OpenAI APITimeout Error: OpenAI Timeout")
+                await asyncio.sleep(10)
+            except openai.error.ServiceUnavailableError as e:
+                logging.warning(f"OpenAI service unavailable error: {e}")
+                await asyncio.sleep(10)
             except openai.error.APIError as e:
                 logging.warning(f"OpenAI API error: {e}")
-                break
+                await asyncio.sleep(10)
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_completion(
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
     context_length: int,
-    requests_per_minute: int = 300,
+    requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from OpenAI Completion API.
 
     Args:
         full_contexts: List of full contexts to generate from.
         prompt_template: Prompt template to use.
         model_config: Model configuration.
@@ -133,29 +154,32 @@
                 logging.warning(
                     "OpenAI API Connection Error: Error Communicating with OpenAI"
                 )
                 await asyncio.sleep(10)
             except openai.error.Timeout:
                 logging.warning("OpenAI APITimeout Error: OpenAI Timeout")
                 await asyncio.sleep(10)
+            except openai.error.ServiceUnavailableError as e:
+                logging.warning(f"OpenAI service unavailable error: {e}")
+                await asyncio.sleep(10)
             except openai.error.APIError as e:
                 logging.warning(f"OpenAI API error: {e}")
-                break
+                await asyncio.sleep(10)
         return {"choices": [{"message": {"content": ""}}]}
 
 
 async def generate_from_openai_chat_completion(
     full_contexts: list[chat_prompt.ChatMessages],
     prompt_template: chat_prompt.ChatMessages,
     model_config: lm_config.LMConfig,
     temperature: float,
     max_tokens: int,
     top_p: float,
     context_length: int,
-    requests_per_minute: int = 300,
+    requests_per_minute: int = 150,
 ) -> list[str]:
     """Generate from OpenAI Chat Completion API.
 
     Args:
         full_contexts: List of full contexts to generate from.
         prompt_template: Prompt template to use.
         model_config: Model configuration.
```

### Comparing `zeno_build-0.0.2/zeno_build/optimizers/base.py` & `zeno_build-0.0.3/zeno_build/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/optimizers/exhaustive.py` & `zeno_build-0.0.3/zeno_build/optimizers/exhaustive.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/optimizers/random.py` & `zeno_build-0.0.3/zeno_build/optimizers/random.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/optimizers/vizier.py` & `zeno_build-0.0.3/zeno_build/optimizers/vizier.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/prompts/chat_prompt.py` & `zeno_build-0.0.3/zeno_build/prompts/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/reporting/aggregate_results.py` & `zeno_build-0.0.3/zeno_build/reporting/aggregate_results.py`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/zeno_build/reporting/reporting_utils.py` & `zeno_build-0.0.3/zeno_build/reporting/reporting_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """Utility functions to help with reporting."""
 
 from typing import Any
 
-from zeno_build.experiments import search_space
-from zeno_build.experiments.search_space import CombinatorialSearchSpace
+from zeno_build.experiments.search_space import SearchSpace
 
 
-def parameters_to_name(
-    parameters: dict[str, Any], space: CombinatorialSearchSpace
-) -> str:
+def parameters_to_name(parameters: dict[str, Any], space: SearchSpace) -> str:
     """Convert parameters into a readable model name.
 
     Args:
         parameters: The parameters to convert.
         space: The search space to use.
 
     Returns:
         A string representation of the model.
     """
     return " ".join(
         [
             parameters[k] if isinstance(parameters[k], str) else f"{k}={parameters[k]}"
-            for k, v in space.dimensions.items()
-            if not isinstance(v, search_space.Constant)
+            for k in space.get_non_constant_dimensions()
         ]
     )
```

### Comparing `zeno_build-0.0.2/zeno_build/reporting/visualize.py` & `zeno_build-0.0.3/zeno_build/reporting/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,11 +53,12 @@
         metadata=df,
         view=view,
         models=list(model_results.keys()),
         functions=[get_model] + functions,
         data_column=data_column,
         label_column="label",
         batch_size=100000,
+        multiprocessing=False,
     )
     config = config.copy(update=zeno_config)
 
     zeno(config)
```

### Comparing `zeno_build-0.0.2/.gitignore` & `zeno_build-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/LICENSE` & `zeno_build-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zeno_build-0.0.2/README.md` & `zeno_build-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -40,20 +40,31 @@
 have a bunch of examples of how you can use `zeno-build` for different tasks,
 such as [chatbots](examples/chatbot/),
 [text summarization](examples/summarization/), or [text
 classification](examples/text_classification/).
 
 Each of the examples include code for running experiments and evaluating the
 results. `zeno-build` will produce a comprehensive report with the
-[Zeno](https://zenoml.com/) ML analysis platform. To give you a flavor of what
-these reports will look like, check out a few of our pre-made reports below:
+[Zeno](https://zenoml.com/) AI evaluation platform.
 
-- [Zeno Chatbot Report](examples/chatbot/report/): A report comparing different methods
+## Interactive Demos/Reports
+
+Using Zeno Build, we have generated reports and online browsing demos of
+state-of-the-art systems for different popular generative AI tasks.
+Check out our pre-made reports below:
+
+- **Chatbots** ([Report](examples/chatbot/report/),
+  [Browser](https://zeno-ml-chatbot-report.hf.space/)):
+  A report comparing different methods
   for creating chatbots, including API-based models such as ChatGPT and Cohere,
   with open-source models such as Vicuna, Alpaca, and MPT.
+- **Translation** ([Report](examples/analysis_gpt_mt/report/),
+  [Browser](https://zeno-ml-translation-report.hf.space/)):
+  A report comparing GPT-based methods, Microsoft Translator, and the best system
+  from the Conference on Machine Translation.
 
 ## Building Your Own Apps (and Contributing Back)
 
 Each of the examples in the [examples/](examples/) directory is specifically designed
 to be self-contained and easy to modify. To get started building your own apps,
 we suggest that you first click into the directory and read the general README,
 find the closest example to what you're trying to do, copy the example to the
```

### Comparing `zeno_build-0.0.2/pyproject.toml` & `zeno_build-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
-dependencies = ["aiolimiter>=1.0.0", "inspiredco>=0.0.2", "zenoml>=0.6.0"]
+dependencies = ["aiolimiter>=1.0.0", "inspiredco>=0.0.2", "zenoml>=0.6.1"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["mypy>=1.2.0", "pre-commit>=3.2.0", "pytest>=6.0.0", "black>=23.3.0"]
 
 [tool.hatch.build]
 include = ["*.py"]
```

### Comparing `zeno_build-0.0.2/PKG-INFO` & `zeno_build-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeno_build
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for comparing multiple llm-based systems.
 Author-email: Ángel Alexander Cabrera <alex.cabrera@gmail.com>, Graham Neubig <neubig@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Zeno
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,15 @@
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Requires-Dist: aiolimiter>=1.0.0
 Requires-Dist: inspiredco>=0.0.2
-Requires-Dist: zenoml>=0.6.0
+Requires-Dist: zenoml>=0.6.1
 Provides-Extra: test
 Requires-Dist: black>=23.3.0; extra == 'test'
 Requires-Dist: mypy>=1.2.0; extra == 'test'
 Requires-Dist: pre-commit>=3.2.0; extra == 'test'
 Requires-Dist: pytest>=6.0.0; extra == 'test'
 Description-Content-Type: text/markdown
 
@@ -81,20 +81,31 @@
 have a bunch of examples of how you can use `zeno-build` for different tasks,
 such as [chatbots](examples/chatbot/),
 [text summarization](examples/summarization/), or [text
 classification](examples/text_classification/).
 
 Each of the examples include code for running experiments and evaluating the
 results. `zeno-build` will produce a comprehensive report with the
-[Zeno](https://zenoml.com/) ML analysis platform. To give you a flavor of what
-these reports will look like, check out a few of our pre-made reports below:
+[Zeno](https://zenoml.com/) AI evaluation platform.
 
-- [Zeno Chatbot Report](examples/chatbot/report/): A report comparing different methods
+## Interactive Demos/Reports
+
+Using Zeno Build, we have generated reports and online browsing demos of
+state-of-the-art systems for different popular generative AI tasks.
+Check out our pre-made reports below:
+
+- **Chatbots** ([Report](examples/chatbot/report/),
+  [Browser](https://zeno-ml-chatbot-report.hf.space/)):
+  A report comparing different methods
   for creating chatbots, including API-based models such as ChatGPT and Cohere,
   with open-source models such as Vicuna, Alpaca, and MPT.
+- **Translation** ([Report](examples/analysis_gpt_mt/report/),
+  [Browser](https://zeno-ml-translation-report.hf.space/)):
+  A report comparing GPT-based methods, Microsoft Translator, and the best system
+  from the Conference on Machine Translation.
 
 ## Building Your Own Apps (and Contributing Back)
 
 Each of the examples in the [examples/](examples/) directory is specifically designed
 to be self-contained and easy to modify. To get started building your own apps,
 we suggest that you first click into the directory and read the general README,
 find the closest example to what you're trying to do, copy the example to the
```

