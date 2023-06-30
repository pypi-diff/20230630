# Comparing `tmp/alpaca_eval-0.1.5.tar.gz` & `tmp/alpaca_eval-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.1.5.tar", last modified: Thu Jun 22 01:49:46 2023, max compression
+gzip compressed data, was "alpaca_eval-0.1.6.tar", last modified: Fri Jun 30 14:23:05 2023, max compression
```

## Comparing `alpaca_eval-0.1.5.tar` & `alpaca_eval-0.1.6.tar`

### file list

```diff
@@ -1,174 +1,177 @@
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:46.007835 alpaca_eval-0.1.5/
--rw-rw-r--   0 rtaori   (20446) root         (0)    11409 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/LICENSE
--rw-rw-r--   0 rtaori   (20446) root         (0)      187 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/MANIFEST.in
--rw-rw-r--   0 rtaori   (20446) root         (0)    66360 2023-06-22 01:49:46.005835 alpaca_eval-0.1.5/PKG-INFO
--rw-rw-r--   0 rtaori   (20446) root         (0)    65538 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/README.md
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.543830 alpaca_eval-0.1.5/example/
--rw-rw-r--   0 rtaori   (20446) root         (0)   517613 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/example/outputs.json
--rw-rw-r--   0 rtaori   (20446) root         (0)       38 2023-06-22 01:49:46.008835 alpaca_eval-0.1.5/setup.cfg
--rw-rw-r--   0 rtaori   (20446) root         (0)     2123 2023-06-12 20:45:15.000000 alpaca_eval-0.1.5/setup.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.426829 alpaca_eval-0.1.5/src/
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.585830 alpaca_eval-0.1.5/src/alpaca_eval/
--rw-rw-r--   0 rtaori   (20446) root         (0)       22 2023-06-22 01:48:21.000000 alpaca_eval-0.1.5/src/alpaca_eval/__init__.py
--rw-rw-r--   0 rtaori   (20446) root         (0)    21396 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/analyze.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.626831 alpaca_eval-0.1.5/src/alpaca_eval/annotators/
--rw-rw-r--   0 rtaori   (20446) root         (0)       33 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/annotators/__init__.py
--rw-rw-r--   0 rtaori   (20446) root         (0)    33988 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     4018 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/completion_parsers.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     5317 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/constants.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.644831 alpaca_eval-0.1.5/src/alpaca_eval/decoders/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1913 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/__init__.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     4873 2023-06-16 13:47:30.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/anthropic.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     3476 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/cohere.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     3905 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_api.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     4899 2023-06-16 13:47:30.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_local.py
--rw-rw-r--   0 rtaori   (20446) root         (0)    12623 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/decoders/openai.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.648831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/
--rw-rw-r--   0 rtaori   (20446) root         (0)     9753 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/README.md
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.655831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1204 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      270 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.662831 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-rw-r--   0 rtaori   (20446) root         (0)      905 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     1140 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.707832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1650 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     5869 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     2475 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     3721 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     3423 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     6849 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     6797 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     6700 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     6045 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)     1016 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     3969 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     5932 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)     5370 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.716832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)     7373 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      362 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.723832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1048 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      324 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.730832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1116 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      325 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.738832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1197 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      754 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.746832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1137 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      317 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.754832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-rw-r--   0 rtaori   (20446) root         (0)      259 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)     1087 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.760832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/cohere/
--rw-rw-r--   0 rtaori   (20446) root         (0)      303 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.764832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)      314 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.773832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1298 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      452 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.778832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)      322 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.782832 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)      317 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.790833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)      319 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)     1051 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.797833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1054 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      367 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.805833 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-rw-r--   0 rtaori   (20446) root         (0)     1017 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      341 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.473829 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.819833 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-rw-r--   0 rtaori   (20446) root         (0)     2037 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-rw-r--   0 rtaori   (20446) root         (0)      904 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-rw-r--   0 rtaori   (20446) root         (0)     1820 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-rw-r--   0 rtaori   (20446) root         (0)      351 2023-06-08 16:32:49.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.824833 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/
--rw-rw-r--   0 rtaori   (20446) root         (0)     2929 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-rw-r--   0 rtaori   (20446) root         (0)    21870 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/main.py
--rw-rw-r--   0 rtaori   (20446) root         (0)     1313 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/metrics.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.525830 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.833833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      415 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      171 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.838833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-65b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      415 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.846833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      382 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      152 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.851833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-rw-r--   0 rtaori   (20446) root         (0)      433 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.855833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-rw-r--   0 rtaori   (20446) root         (0)      456 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.859833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/chatgpt/
--rw-rw-r--   0 rtaori   (20446) root         (0)      196 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.867833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/
--rw-rw-r--   0 rtaori   (20446) root         (0)      184 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)       34 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.874833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/
--rw-rw-r--   0 rtaori   (20446) root         (0)      199 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)       13 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.878833 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere-chat/
--rw-rw-r--   0 rtaori   (20446) root         (0)      205 2023-06-16 14:10:37.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.882834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-rw-r--   0 rtaori   (20446) root         (0)      405 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.886834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-rw-r--   0 rtaori   (20446) root         (0)      401 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.894834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/
--rw-rw-r--   0 rtaori   (20446) root         (0)      100 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      178 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.898834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-13b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.902834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-33b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.905834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-65b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      430 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.913834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      425 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      195 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.921834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      429 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      186 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.930834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      407 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.934834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      449 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.943834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      436 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)       42 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.952834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      458 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)       51 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.958834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-rw-r--   0 rtaori   (20446) root         (0)      438 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.963834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_001/
--rw-rw-r--   0 rtaori   (20446) root         (0)      211 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.972834 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/
--rw-rw-r--   0 rtaori   (20446) root         (0)      211 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)       34 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.981835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      387 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.990835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      383 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:46.000835 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-rw-r--   0 rtaori   (20446) root         (0)      394 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-rw-r--   0 rtaori   (20446) root         (0)      185 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)    22484 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/plotting.py
--rw-rw-r--   0 rtaori   (20446) root         (0)      283 2023-06-08 16:32:50.000000 alpaca_eval-0.1.5/src/alpaca_eval/types.py
--rw-rw-r--   0 rtaori   (20446) root         (0)    15815 2023-06-22 01:41:05.000000 alpaca_eval-0.1.5/src/alpaca_eval/utils.py
-drwxrwsr-x   0 rtaori   (20446) root         (0)        0 2023-06-22 01:49:45.617831 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/
--rw-rw-r--   0 rtaori   (20446) root         (0)    66360 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/PKG-INFO
--rw-rw-r--   0 rtaori   (20446) root         (0)     6457 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/SOURCES.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)        1 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/dependency_links.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)       54 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/entry_points.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)      418 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/requires.txt
--rw-rw-r--   0 rtaori   (20446) root         (0)       12 2023-06-22 01:49:45.000000 alpaca_eval-0.1.5/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.481435 alpaca_eval-0.1.6/
+-rw-r--r--   0 rtaori     (501) staff       (20)    11409 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/LICENSE
+-rw-r--r--   0 rtaori     (501) staff       (20)      187 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/MANIFEST.in
+-rw-r--r--   0 rtaori     (501) staff       (20)    66360 2023-06-30 14:23:05.481277 alpaca_eval-0.1.6/PKG-INFO
+-rw-r--r--   0 rtaori     (501) staff       (20)    65538 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/README.md
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.448241 alpaca_eval-0.1.6/example/
+-rw-r--r--   0 rtaori     (501) staff       (20)   517613 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/example/outputs.json
+-rw-r--r--   0 rtaori     (501) staff       (20)       38 2023-06-30 14:23:05.481474 alpaca_eval-0.1.6/setup.cfg
+-rw-r--r--   0 rtaori     (501) staff       (20)     2131 2023-06-30 14:20:34.000000 alpaca_eval-0.1.6/setup.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.438399 alpaca_eval-0.1.6/src/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.451501 alpaca_eval-0.1.6/src/alpaca_eval/
+-rw-r--r--   0 rtaori     (501) staff       (20)       22 2023-06-30 14:21:44.000000 alpaca_eval-0.1.6/src/alpaca_eval/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    21396 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.464851 alpaca_eval-0.1.6/src/alpaca_eval/annotators/
+-rw-r--r--   0 rtaori     (501) staff       (20)       33 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    33988 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     4018 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     5317 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/constants.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.466710 alpaca_eval-0.1.6/src/alpaca_eval/decoders/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1913 2023-06-29 22:23:29.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     4873 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     3476 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     3905 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     4899 2023-06-15 20:34:36.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    12623 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.466859 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 rtaori     (501) staff       (20)     9753 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.467255 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1204 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      270 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.467698 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 rtaori     (501) staff       (20)      905 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     1140 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.469817 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1650 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5869 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     2475 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3721 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3423 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6849 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6797 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6700 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     6045 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1016 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     3969 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5932 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)     5370 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.470180 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     7373 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      362 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.470477 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1048 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      324 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.470755 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1116 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      325 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.471026 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1197 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      754 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.471289 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1137 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.471587 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 rtaori     (501) staff       (20)      259 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1087 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.471722 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 rtaori     (501) staff       (20)      303 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.471847 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      314 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.472116 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1298 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      452 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.472257 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      322 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.472423 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      317 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.472705 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      319 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)     1051 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.472975 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1054 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      367 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.473365 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 rtaori     (501) staff       (20)     1017 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      341 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.445622 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.474115 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 rtaori     (501) staff       (20)     2110 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)      904 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)     1820 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)      351 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.474267 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 rtaori     (501) staff       (20)     2929 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 rtaori     (501) staff       (20)    21870 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/main.py
+-rw-r--r--   0 rtaori     (501) staff       (20)     1313 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.447232 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.474577 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      415 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      171 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.474714 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      415 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.475070 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      382 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      152 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.475252 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 rtaori     (501) staff       (20)      433 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.475441 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 rtaori     (501) staff       (20)      456 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.475574 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 rtaori     (501) staff       (20)      196 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.475819 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 rtaori     (501) staff       (20)      184 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.476167 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 rtaori     (501) staff       (20)      199 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       13 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.476332 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 rtaori     (501) staff       (20)      205 2023-06-16 14:14:12.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.476455 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 rtaori     (501) staff       (20)      435 2023-06-29 05:02:14.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.476681 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 rtaori     (501) staff       (20)      431 2023-06-29 05:02:16.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477010 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 rtaori     (501) staff       (20)      100 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      178 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477135 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477258 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477387 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      430 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477638 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      425 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      195 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.477990 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      429 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      186 2023-06-19 03:07:06.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.478346 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      407 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.478509 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      449 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.478821 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      436 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       42 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.479119 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      458 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       51 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.479410 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 rtaori     (501) staff       (20)      438 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.479614 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.479897 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 rtaori     (501) staff       (20)      211 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)       34 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.480162 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      401 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      271 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.480458 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      387 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.480741 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      383 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.481007 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 rtaori     (501) staff       (20)      394 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 rtaori     (501) staff       (20)      185 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)    22484 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/plotting.py
+-rw-r--r--   0 rtaori     (501) staff       (20)      283 2023-06-08 16:33:22.000000 alpaca_eval-0.1.6/src/alpaca_eval/types.py
+-rw-r--r--   0 rtaori     (501) staff       (20)    15815 2023-06-28 08:49:47.000000 alpaca_eval-0.1.6/src/alpaca_eval/utils.py
+drwxr-xr-x   0 rtaori     (501) staff       (20)        0 2023-06-30 14:23:05.452234 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/
+-rw-r--r--   0 rtaori     (501) staff       (20)    66360 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 rtaori     (501) staff       (20)     6567 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)        1 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)       54 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)      434 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 rtaori     (501) staff       (20)       12 2023-06-30 14:23:05.000000 alpaca_eval-0.1.6/src/alpaca_eval.egg-info/top_level.txt
```

### Comparing `alpaca_eval-0.1.5/LICENSE` & `alpaca_eval-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/PKG-INFO` & `alpaca_eval-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.1.5
+Version: 0.1.6
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.5 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.1.6 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.1.5/README.md` & `alpaca_eval-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/example/outputs.json` & `alpaca_eval-0.1.6/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/setup.py` & `alpaca_eval-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 PACKAGES_DEV = ["pre-commit>=3.2.0", "black>=23.1.0", "isort"]
 PACKAGES_ANALYSIS = [
     "seaborn",
     "matplotlib",
     "jupyterlab"
 ]
 PACKAGES_LOCAL = ["accelerate", "transformers", "bitsandbytes", "xformers", "peft", "optimum", "scipy"]
-PACKAGES_ALL_API = ["anthropic", "huggingface_hub", "cohere"]
+PACKAGES_ALL_API = ["anthropic<=0.2.10", "huggingface_hub", "cohere"]
 PACKAGES_ALL = PACKAGES_LOCAL + PACKAGES_ALL_API + PACKAGES_ANALYSIS + PACKAGES_DEV
 
 setuptools.setup(
     name="alpaca_eval",
     version=version,
     description="AlpacaEval : An Automatic Evaluator of Instruction-following Models",
     package_dir={"": "src"},
```

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/analyze.py` & `alpaca_eval-0.1.6/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.1.6/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.1.6/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/constants.py` & `alpaca_eval-0.1.6/src/alpaca_eval/constants.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/anthropic.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.1.6/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.1.6/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
 gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32
 claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89
 chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109
+ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155
 wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194
 airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202
 airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212
 guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227
 vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237
 oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268
 minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271
```

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.1.6/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/main.py` & `alpaca_eval-0.1.6/src/alpaca_eval/main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/metrics.py` & `alpaca_eval-0.1.6/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/plotting.py` & `alpaca_eval-0.1.6/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval/utils.py` & `alpaca_eval-0.1.6/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.1.6/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.1.5
+Version: 0.1.6
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.5 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.1.6 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.1.5/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.1.6/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -104,13 +104,15 @@
 src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
 src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
 src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
 src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
 src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
 src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
 src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
 src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
 src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
```

