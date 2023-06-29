# Comparing `tmp/griptape-0.9.0.tar.gz` & `tmp/griptape-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape-0.9.0.tar", max compression
+gzip compressed data, was "griptape-0.9.1.tar", max compression
```

## Comparing `griptape-0.9.0.tar` & `griptape-0.9.1.tar`

### file list

```diff
@@ -1,118 +1,120 @@
--rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.9.0/LICENSE
--rw-r--r--   0        0        0     4497 2023-05-15 06:28:28.376351 griptape-0.9.0/README.md
--rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.9.0/griptape/__init__.py
--rw-r--r--   0        0        0      486 2023-05-10 16:01:15.657261 griptape-0.9.0/griptape/artifacts/__init__.py
--rw-r--r--   0        0        0     1385 2023-05-10 16:17:57.768622 griptape-0.9.0/griptape/artifacts/base_artifact.py
--rw-r--r--   0        0        0      799 2023-05-10 17:33:20.087370 griptape-0.9.0/griptape/artifacts/blob_artifact.py
--rw-r--r--   0        0        0      359 2023-05-09 18:59:20.776163 griptape-0.9.0/griptape/artifacts/error_artifact.py
--rw-r--r--   0        0        0      356 2023-05-10 16:01:15.661516 griptape-0.9.0/griptape/artifacts/info_artifact.py
--rw-r--r--   0        0        0      648 2023-05-19 10:55:24.781106 griptape-0.9.0/griptape/artifacts/list_artifact.py
--rw-r--r--   0        0        0      918 2023-05-18 13:09:17.200524 griptape-0.9.0/griptape/artifacts/text_artifact.py
--rw-r--r--   0        0        0      126 2023-05-03 20:08:48.695610 griptape-0.9.0/griptape/core/__init__.py
--rw-r--r--   0        0        0     3883 2023-05-19 07:34:20.088113 griptape-0.9.0/griptape/core/activity_mixin.py
--rw-r--r--   0        0        0     4710 2023-05-19 12:02:32.818108 griptape-0.9.0/griptape/core/base_tool.py
--rw-r--r--   0        0        0     1102 2023-05-19 07:40:21.539874 griptape-0.9.0/griptape/core/decorators.py
--rw-r--r--   0        0        0     1879 2023-05-18 09:54:34.968210 griptape-0.9.0/griptape/drivers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 15:37:50.794303 griptape-0.9.0/griptape/drivers/embedding/__init__.py
--rw-r--r--   0        0        0     1125 2023-05-18 11:35:36.866020 griptape-0.9.0/griptape/drivers/embedding/base_embedding_driver.py
--rw-r--r--   0        0        0     2574 2023-05-18 11:36:10.238385 griptape-0.9.0/griptape/drivers/embedding/openai_embedding_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.9.0/griptape/drivers/memory/__init__.py
--rw-r--r--   0        0        0      242 2023-05-16 13:21:44.218015 griptape-0.9.0/griptape/drivers/memory/base_memory_driver.py
--rw-r--r--   0        0        0      563 2023-05-16 13:21:44.220400 griptape-0.9.0/griptape/drivers/memory/disk_memory_driver.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.9.0/griptape/drivers/prompt/__init__.py
--rw-r--r--   0        0        0     1084 2023-05-17 13:47:48.161699 griptape-0.9.0/griptape/drivers/prompt/base_prompt_driver.py
--rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.9.0/griptape/drivers/prompt/cohere_prompt_driver.py
--rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.9.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
--rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.9.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
--rw-r--r--   0        0        0     2699 2023-05-16 15:50:04.805033 griptape-0.9.0/griptape/drivers/prompt/openai_prompt_driver.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.9.0/griptape/drivers/storage/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 16:43:06.908509 griptape-0.9.0/griptape/drivers/storage/blob/__init__.py
--rw-r--r--   0        0        0      417 2023-05-09 17:07:04.025663 griptape-0.9.0/griptape/drivers/storage/blob/base_blob_storage_driver.py
--rw-r--r--   0        0        0      762 2023-05-09 17:07:04.028021 griptape-0.9.0/griptape/drivers/storage/blob/memory_blob_storage_driver.py
--rw-r--r--   0        0        0        0 2023-05-09 16:04:11.435219 griptape-0.9.0/griptape/drivers/storage/text/__init__.py
--rw-r--r--   0        0        0      434 2023-05-10 20:05:06.365336 griptape-0.9.0/griptape/drivers/storage/text/base_text_storage_driver.py
--rw-r--r--   0        0        0     1373 2023-05-09 16:05:38.013785 griptape-0.9.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py
--rw-r--r--   0        0        0      569 2023-05-09 17:14:35.966970 griptape-0.9.0/griptape/drivers/storage/text/memory_text_storage_driver.py
--rw-r--r--   0        0        0        0 2023-05-18 09:49:51.365989 griptape-0.9.0/griptape/drivers/storage/vector/__init__.py
--rw-r--r--   0        0        0     1836 2023-05-19 12:30:31.483080 griptape-0.9.0/griptape/drivers/storage/vector/base_vector_storage_driver.py
--rw-r--r--   0        0        0     2205 2023-05-19 12:34:09.595472 griptape-0.9.0/griptape/drivers/storage/vector/pinecone_vector_storage_driver.py
--rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.9.0/griptape/executors/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-19 07:34:20.085769 griptape-0.9.0/griptape/executors/base_executor.py
--rw-r--r--   0        0        0     3304 2023-05-08 20:16:06.614331 griptape-0.9.0/griptape/executors/docker_executor.py
--rw-r--r--   0        0        0     2162 2023-05-10 23:06:37.186354 griptape-0.9.0/griptape/executors/local_executor.py
--rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.9.0/griptape/memory/__init__.py
--rw-r--r--   0        0        0      779 2023-05-09 18:59:20.783209 griptape-0.9.0/griptape/memory/buffer_memory.py
--rw-r--r--   0        0        0     1772 2023-05-16 13:21:44.215715 griptape-0.9.0/griptape/memory/memory.py
--rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.9.0/griptape/memory/run.py
--rw-r--r--   0        0        0     2105 2023-05-09 18:59:20.779182 griptape-0.9.0/griptape/memory/summary_memory.py
--rw-r--r--   0        0        0      203 2023-05-09 21:24:07.655284 griptape-0.9.0/griptape/ramps/__init__.py
--rw-r--r--   0        0        0     1541 2023-05-09 19:44:03.721738 griptape-0.9.0/griptape/ramps/base_ramp.py
--rw-r--r--   0        0        0     1323 2023-05-19 07:34:20.090080 griptape-0.9.0/griptape/ramps/blob_storage_ramp.py
--rw-r--r--   0        0        0     2572 2023-05-19 07:34:20.091709 griptape-0.9.0/griptape/ramps/text_storage_ramp.py
--rw-r--r--   0        0        0      100 2023-05-10 23:10:33.578044 griptape-0.9.0/griptape/resources/docker_executor/Dockerfile
--rw-r--r--   0        0        0       64 2023-05-05 15:39:50.489813 griptape-0.9.0/griptape/rules/__init__.py
--rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.9.0/griptape/rules/rule.py
--rw-r--r--   0        0        0      144 2023-05-05 15:39:50.487681 griptape-0.9.0/griptape/rules/ruleset.py
--rw-r--r--   0        0        0     1165 2023-05-10 16:03:43.577569 griptape-0.9.0/griptape/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.9.0/griptape/schemas/artifacts/__init__.py
--rw-r--r--   0        0        0      275 2023-05-10 16:34:41.421057 griptape-0.9.0/griptape/schemas/artifacts/artifact_schema.py
--rw-r--r--   0        0        0      409 2023-05-07 16:29:29.348073 griptape-0.9.0/griptape/schemas/artifacts/blob_artifact_schema.py
--rw-r--r--   0        0        0      303 2023-05-06 19:49:43.542366 griptape-0.9.0/griptape/schemas/artifacts/error_artifact_schema.py
--rw-r--r--   0        0        0      300 2023-05-09 21:33:24.929758 griptape-0.9.0/griptape/schemas/artifacts/info_artifact_schema.py
--rw-r--r--   0        0        0      354 2023-05-10 16:16:15.649988 griptape-0.9.0/griptape/schemas/artifacts/list_artifact_schema.py
--rw-r--r--   0        0        0      300 2023-05-06 19:49:43.546323 griptape-0.9.0/griptape/schemas/artifacts/text_artifact_schema.py
--rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.9.0/griptape/schemas/base_schema.py
--rw-r--r--   0        0        0        0 2023-05-03 19:15:12.616328 griptape-0.9.0/griptape/schemas/memory/__init__.py
--rw-r--r--   0        0        0      299 2023-05-03 19:35:36.457310 griptape-0.9.0/griptape/schemas/memory/buffer_memory_schema.py
--rw-r--r--   0        0        0      372 2023-05-10 16:35:39.384699 griptape-0.9.0/griptape/schemas/memory/memory_schema.py
--rw-r--r--   0        0        0      350 2023-05-03 19:15:12.616696 griptape-0.9.0/griptape/schemas/memory/run_schema.py
--rw-r--r--   0        0        0      372 2023-05-03 19:44:56.927223 griptape-0.9.0/griptape/schemas/memory/summary_memory_schema.py
--rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.9.0/griptape/schemas/polymorphic_schema.py
--rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.9.0/griptape/structures/__init__.py
--rw-r--r--   0        0        0     1586 2023-05-18 08:07:17.483013 griptape-0.9.0/griptape/structures/agent.py
--rw-r--r--   0        0        0     2608 2023-05-18 08:07:17.483398 griptape-0.9.0/griptape/structures/pipeline.py
--rw-r--r--   0        0        0     2844 2023-05-18 10:06:46.880896 griptape-0.9.0/griptape/structures/structure.py
--rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.9.0/griptape/structures/structure_with_memory.py
--rw-r--r--   0        0        0     2762 2023-05-18 08:07:17.483802 griptape-0.9.0/griptape/structures/workflow.py
--rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.9.0/griptape/summarizers/__init__.py
--rw-r--r--   0        0        0      426 2023-05-03 19:38:21.128646 griptape-0.9.0/griptape/summarizers/base_summarizer.py
--rw-r--r--   0        0        0     1401 2023-05-06 17:03:28.895388 griptape-0.9.0/griptape/summarizers/prompt_driver_summarizer.py
--rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.9.0/griptape/tasks/__init__.py
--rw-r--r--   0        0        0     8847 2023-05-18 08:09:25.422365 griptape-0.9.0/griptape/tasks/action_subtask.py
--rw-r--r--   0        0        0     3901 2023-05-18 07:58:36.991716 griptape-0.9.0/griptape/tasks/base_task.py
--rw-r--r--   0        0        0     2055 2023-05-18 07:58:36.994737 griptape-0.9.0/griptape/tasks/prompt_task.py
--rw-r--r--   0        0        0     4710 2023-05-18 08:09:25.417190 griptape-0.9.0/griptape/tasks/toolkit_task.py
--rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.9.0/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
--rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.9.0/griptape/templates/prompts/agent.j2
--rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.9.0/griptape/templates/prompts/memory.j2
--rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.9.0/griptape/templates/prompts/pipeline.j2
--rw-r--r--   0        0        0      482 2023-05-05 19:11:47.103721 griptape-0.9.0/griptape/templates/prompts/ramp.j2
--rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.9.0/griptape/templates/prompts/run.j2
--rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.9.0/griptape/templates/prompts/summarize.j2
--rw-r--r--   0        0        0      454 2023-05-18 08:26:35.125874 griptape-0.9.0/griptape/templates/prompts/tasks/prompt/base.j2
--rw-r--r--   0        0        0      122 2023-05-18 08:20:34.420734 griptape-0.9.0/griptape/templates/prompts/tasks/prompt/conversation.j2
--rw-r--r--   0        0        0     2168 2023-05-18 08:26:35.124073 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/base.j2
--rw-r--r--   0        0        0      187 2023-05-06 17:03:28.888976 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/conversation.j2
--rw-r--r--   0        0        0      179 2023-05-06 17:03:28.912824 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/subtask.j2
--rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/subtasks.j2
--rw-r--r--   0        0        0      482 2023-05-05 19:11:47.105201 griptape-0.9.0/griptape/templates/prompts/tool.j2
--rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.9.0/griptape/templates/prompts/workflow.j2
--rw-r--r--   0        0        0      131 2023-05-10 18:51:24.681023 griptape-0.9.0/griptape/templates/ramps/blob_storage.j2
--rw-r--r--   0        0        0      131 2023-05-10 18:51:24.678788 griptape-0.9.0/griptape/templates/ramps/text_storage.j2
--rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.9.0/griptape/tokenizers/__init__.py
--rw-r--r--   0        0        0      960 2023-05-17 13:00:38.742159 griptape-0.9.0/griptape/tokenizers/base_tokenizer.py
--rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.9.0/griptape/tokenizers/cohere_tokenizer.py
--rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.9.0/griptape/tokenizers/hugging_face_tokenizer.py
--rw-r--r--   0        0        0     1697 2023-05-17 11:38:47.481284 griptape-0.9.0/griptape/tokenizers/tiktoken_tokenizer.py
--rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.9.0/griptape/utils/__init__.py
--rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.9.0/griptape/utils/command_runner.py
--rw-r--r--   0        0        0      509 2023-04-23 22:46:42.637126 griptape-0.9.0/griptape/utils/conversation.py
--rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.9.0/griptape/utils/j2.py
--rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.9.0/griptape/utils/manifest_validator.py
--rw-r--r--   0        0        0        0 2023-05-06 19:56:24.051141 griptape-0.9.0/griptape/utils/marshmallow/__init__.py
--rw-r--r--   0        0        0       52 2023-05-06 19:58:37.405568 griptape-0.9.0/griptape/utils/marshmallow/fields/__init__.py
--rw-r--r--   0        0        0      422 2023-05-06 20:47:07.097992 griptape-0.9.0/griptape/utils/marshmallow/fields/bytes.py
--rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.9.0/griptape/utils/paths.py
--rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.9.0/griptape/utils/python_runner.py
--rw-r--r--   0        0        0     1175 2023-05-19 13:00:15.414369 griptape-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5970 1970-01-01 00:00:00.000000 griptape-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 20:17:23.178260 griptape-0.9.1/LICENSE
+-rw-r--r--   0        0        0     4497 2023-05-15 06:28:28.376351 griptape-0.9.1/README.md
+-rw-r--r--   0        0        0       65 2023-04-24 19:02:26.305879 griptape-0.9.1/griptape/__init__.py
+-rw-r--r--   0        0        0      486 2023-05-10 16:01:15.657261 griptape-0.9.1/griptape/artifacts/__init__.py
+-rw-r--r--   0        0        0     1385 2023-05-10 16:17:57.768622 griptape-0.9.1/griptape/artifacts/base_artifact.py
+-rw-r--r--   0        0        0      797 2023-05-20 08:17:28.304030 griptape-0.9.1/griptape/artifacts/blob_artifact.py
+-rw-r--r--   0        0        0      359 2023-05-09 18:59:20.776163 griptape-0.9.1/griptape/artifacts/error_artifact.py
+-rw-r--r--   0        0        0      356 2023-05-10 16:01:15.661516 griptape-0.9.1/griptape/artifacts/info_artifact.py
+-rw-r--r--   0        0        0      648 2023-05-19 10:55:24.781106 griptape-0.9.1/griptape/artifacts/list_artifact.py
+-rw-r--r--   0        0        0      918 2023-05-18 13:09:17.200524 griptape-0.9.1/griptape/artifacts/text_artifact.py
+-rw-r--r--   0        0        0       72 2023-05-21 14:20:30.221370 griptape-0.9.1/griptape/chunkers/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-21 15:29:57.193093 griptape-0.9.1/griptape/chunkers/text_chunker.py
+-rw-r--r--   0        0        0      126 2023-05-03 20:08:48.695610 griptape-0.9.1/griptape/core/__init__.py
+-rw-r--r--   0        0        0     3883 2023-05-19 07:34:20.088113 griptape-0.9.1/griptape/core/activity_mixin.py
+-rw-r--r--   0        0        0     4710 2023-05-19 12:02:32.818108 griptape-0.9.1/griptape/core/base_tool.py
+-rw-r--r--   0        0        0     1102 2023-05-19 07:40:21.539874 griptape-0.9.1/griptape/core/decorators.py
+-rw-r--r--   0        0        0     1879 2023-05-18 09:54:34.968210 griptape-0.9.1/griptape/drivers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 15:37:50.794303 griptape-0.9.1/griptape/drivers/embedding/__init__.py
+-rw-r--r--   0        0        0     1125 2023-05-18 11:35:36.866020 griptape-0.9.1/griptape/drivers/embedding/base_embedding_driver.py
+-rw-r--r--   0        0        0     2574 2023-05-18 11:36:10.238385 griptape-0.9.1/griptape/drivers/embedding/openai_embedding_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.067569 griptape-0.9.1/griptape/drivers/memory/__init__.py
+-rw-r--r--   0        0        0      242 2023-05-16 13:21:44.218015 griptape-0.9.1/griptape/drivers/memory/base_memory_driver.py
+-rw-r--r--   0        0        0      563 2023-05-16 13:21:44.220400 griptape-0.9.1/griptape/drivers/memory/disk_memory_driver.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.068205 griptape-0.9.1/griptape/drivers/prompt/__init__.py
+-rw-r--r--   0        0        0     1084 2023-05-17 13:47:48.161699 griptape-0.9.1/griptape/drivers/prompt/base_prompt_driver.py
+-rw-r--r--   0        0        0     1279 2023-04-30 17:35:29.003157 griptape-0.9.1/griptape/drivers/prompt/cohere_prompt_driver.py
+-rw-r--r--   0        0        0     1956 2023-04-30 17:35:29.016094 griptape-0.9.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py
+-rw-r--r--   0        0        0     1733 2023-04-30 17:35:29.013147 griptape-0.9.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py
+-rw-r--r--   0        0        0     2699 2023-05-16 15:50:04.805033 griptape-0.9.1/griptape/drivers/prompt/openai_prompt_driver.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:16.212093 griptape-0.9.1/griptape/drivers/storage/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:43:06.908509 griptape-0.9.1/griptape/drivers/storage/blob/__init__.py
+-rw-r--r--   0        0        0      417 2023-05-09 17:07:04.025663 griptape-0.9.1/griptape/drivers/storage/blob/base_blob_storage_driver.py
+-rw-r--r--   0        0        0      762 2023-05-09 17:07:04.028021 griptape-0.9.1/griptape/drivers/storage/blob/memory_blob_storage_driver.py
+-rw-r--r--   0        0        0        0 2023-05-09 16:04:11.435219 griptape-0.9.1/griptape/drivers/storage/text/__init__.py
+-rw-r--r--   0        0        0      434 2023-05-10 20:05:06.365336 griptape-0.9.1/griptape/drivers/storage/text/base_text_storage_driver.py
+-rw-r--r--   0        0        0     1373 2023-05-09 16:05:38.013785 griptape-0.9.1/griptape/drivers/storage/text/dynamodb_text_storage_driver.py
+-rw-r--r--   0        0        0      569 2023-05-09 17:14:35.966970 griptape-0.9.1/griptape/drivers/storage/text/memory_text_storage_driver.py
+-rw-r--r--   0        0        0        0 2023-05-18 09:49:51.365989 griptape-0.9.1/griptape/drivers/storage/vector/__init__.py
+-rw-r--r--   0        0        0     1836 2023-05-19 12:30:31.483080 griptape-0.9.1/griptape/drivers/storage/vector/base_vector_storage_driver.py
+-rw-r--r--   0        0        0     2205 2023-05-19 12:34:09.595472 griptape-0.9.1/griptape/drivers/storage/vector/pinecone_vector_storage_driver.py
+-rw-r--r--   0        0        0      203 2023-04-23 17:45:35.150209 griptape-0.9.1/griptape/executors/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-19 07:34:20.085769 griptape-0.9.1/griptape/executors/base_executor.py
+-rw-r--r--   0        0        0     3304 2023-05-08 20:16:06.614331 griptape-0.9.1/griptape/executors/docker_executor.py
+-rw-r--r--   0        0        0     2162 2023-05-10 23:06:37.186354 griptape-0.9.1/griptape/executors/local_executor.py
+-rw-r--r--   0        0        0      271 2023-04-24 16:31:58.604436 griptape-0.9.1/griptape/memory/__init__.py
+-rw-r--r--   0        0        0      779 2023-05-09 18:59:20.783209 griptape-0.9.1/griptape/memory/buffer_memory.py
+-rw-r--r--   0        0        0     1772 2023-05-16 13:21:44.215715 griptape-0.9.1/griptape/memory/memory.py
+-rw-r--r--   0        0        0      360 2023-04-23 22:49:52.124272 griptape-0.9.1/griptape/memory/run.py
+-rw-r--r--   0        0        0     2105 2023-05-09 18:59:20.779182 griptape-0.9.1/griptape/memory/summary_memory.py
+-rw-r--r--   0        0        0      203 2023-05-09 21:24:07.655284 griptape-0.9.1/griptape/ramps/__init__.py
+-rw-r--r--   0        0        0     1541 2023-05-09 19:44:03.721738 griptape-0.9.1/griptape/ramps/base_ramp.py
+-rw-r--r--   0        0        0     1323 2023-05-19 07:34:20.090080 griptape-0.9.1/griptape/ramps/blob_storage_ramp.py
+-rw-r--r--   0        0        0     2572 2023-05-19 07:34:20.091709 griptape-0.9.1/griptape/ramps/text_storage_ramp.py
+-rw-r--r--   0        0        0      100 2023-05-10 23:10:33.578044 griptape-0.9.1/griptape/resources/docker_executor/Dockerfile
+-rw-r--r--   0        0        0      122 2023-05-21 19:43:38.389505 griptape-0.9.1/griptape/rules/__init__.py
+-rw-r--r--   0        0        0      110 2023-04-09 19:15:55.927427 griptape-0.9.1/griptape/rules/rule.py
+-rw-r--r--   0        0        0      144 2023-05-05 15:39:50.487681 griptape-0.9.1/griptape/rules/ruleset.py
+-rw-r--r--   0        0        0     1165 2023-05-10 16:03:43.577569 griptape-0.9.1/griptape/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-26 19:51:29.069000 griptape-0.9.1/griptape/schemas/artifacts/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-10 16:34:41.421057 griptape-0.9.1/griptape/schemas/artifacts/artifact_schema.py
+-rw-r--r--   0        0        0      409 2023-05-07 16:29:29.348073 griptape-0.9.1/griptape/schemas/artifacts/blob_artifact_schema.py
+-rw-r--r--   0        0        0      303 2023-05-06 19:49:43.542366 griptape-0.9.1/griptape/schemas/artifacts/error_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-09 21:33:24.929758 griptape-0.9.1/griptape/schemas/artifacts/info_artifact_schema.py
+-rw-r--r--   0        0        0      354 2023-05-10 16:16:15.649988 griptape-0.9.1/griptape/schemas/artifacts/list_artifact_schema.py
+-rw-r--r--   0        0        0      300 2023-05-06 19:49:43.546323 griptape-0.9.1/griptape/schemas/artifacts/text_artifact_schema.py
+-rw-r--r--   0        0        0      222 2023-03-10 19:50:27.265545 griptape-0.9.1/griptape/schemas/base_schema.py
+-rw-r--r--   0        0        0        0 2023-05-03 19:15:12.616328 griptape-0.9.1/griptape/schemas/memory/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-03 19:35:36.457310 griptape-0.9.1/griptape/schemas/memory/buffer_memory_schema.py
+-rw-r--r--   0        0        0      372 2023-05-10 16:35:39.384699 griptape-0.9.1/griptape/schemas/memory/memory_schema.py
+-rw-r--r--   0        0        0      350 2023-05-03 19:15:12.616696 griptape-0.9.1/griptape/schemas/memory/run_schema.py
+-rw-r--r--   0        0        0      372 2023-05-03 19:44:56.927223 griptape-0.9.1/griptape/schemas/memory/summary_memory_schema.py
+-rw-r--r--   0        0        0     5937 2023-04-23 17:06:19.960660 griptape-0.9.1/griptape/schemas/polymorphic_schema.py
+-rw-r--r--   0        0        0      374 2023-04-23 23:11:51.760187 griptape-0.9.1/griptape/structures/__init__.py
+-rw-r--r--   0        0        0     1586 2023-05-18 08:07:17.483013 griptape-0.9.1/griptape/structures/agent.py
+-rw-r--r--   0        0        0     2608 2023-05-18 08:07:17.483398 griptape-0.9.1/griptape/structures/pipeline.py
+-rw-r--r--   0        0        0     2836 2023-05-21 19:44:48.359031 griptape-0.9.1/griptape/structures/structure.py
+-rw-r--r--   0        0        0     1397 2023-04-23 23:24:38.546649 griptape-0.9.1/griptape/structures/structure_with_memory.py
+-rw-r--r--   0        0        0     2762 2023-05-18 08:07:17.483802 griptape-0.9.1/griptape/structures/workflow.py
+-rw-r--r--   0        0        0      210 2023-04-30 17:43:48.623726 griptape-0.9.1/griptape/summarizers/__init__.py
+-rw-r--r--   0        0        0      426 2023-05-03 19:38:21.128646 griptape-0.9.1/griptape/summarizers/base_summarizer.py
+-rw-r--r--   0        0        0     1401 2023-05-06 17:03:28.895388 griptape-0.9.1/griptape/summarizers/prompt_driver_summarizer.py
+-rw-r--r--   0        0        0      292 2023-04-27 20:37:15.607423 griptape-0.9.1/griptape/tasks/__init__.py
+-rw-r--r--   0        0        0     8847 2023-05-18 08:09:25.422365 griptape-0.9.1/griptape/tasks/action_subtask.py
+-rw-r--r--   0        0        0     3901 2023-05-18 07:58:36.991716 griptape-0.9.1/griptape/tasks/base_task.py
+-rw-r--r--   0        0        0     2055 2023-05-18 07:58:36.994737 griptape-0.9.1/griptape/tasks/prompt_task.py
+-rw-r--r--   0        0        0     4710 2023-05-18 08:09:25.417190 griptape-0.9.1/griptape/tasks/toolkit_task.py
+-rw-r--r--   0        0        0      489 2023-04-06 20:17:23.179590 griptape-0.9.1/griptape/templates/converters/chatgpt_plugin/ai-plugin.json.j2
+-rw-r--r--   0        0        0       76 2023-04-24 15:53:53.079453 griptape-0.9.1/griptape/templates/prompts/agent.j2
+-rw-r--r--   0        0        0      187 2023-03-19 16:50:11.402281 griptape-0.9.1/griptape/templates/prompts/memory.j2
+-rw-r--r--   0        0        0      150 2023-04-23 21:55:48.282971 griptape-0.9.1/griptape/templates/prompts/pipeline.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.103721 griptape-0.9.1/griptape/templates/prompts/ramp.j2
+-rw-r--r--   0        0        0       47 2023-03-26 19:51:29.072709 griptape-0.9.1/griptape/templates/prompts/run.j2
+-rw-r--r--   0        0        0      303 2023-03-26 19:51:29.072961 griptape-0.9.1/griptape/templates/prompts/summarize.j2
+-rw-r--r--   0        0        0      454 2023-05-18 08:26:35.125874 griptape-0.9.1/griptape/templates/prompts/tasks/prompt/base.j2
+-rw-r--r--   0        0        0      122 2023-05-18 08:20:34.420734 griptape-0.9.1/griptape/templates/prompts/tasks/prompt/conversation.j2
+-rw-r--r--   0        0        0     2168 2023-05-18 08:26:35.124073 griptape-0.9.1/griptape/templates/prompts/tasks/toolkit/base.j2
+-rw-r--r--   0        0        0      187 2023-05-06 17:03:28.888976 griptape-0.9.1/griptape/templates/prompts/tasks/toolkit/conversation.j2
+-rw-r--r--   0        0        0      179 2023-05-06 17:03:28.912824 griptape-0.9.1/griptape/templates/prompts/tasks/toolkit/subtask.j2
+-rw-r--r--   0        0        0       64 2023-04-23 22:36:52.419627 griptape-0.9.1/griptape/templates/prompts/tasks/toolkit/subtasks.j2
+-rw-r--r--   0        0        0      482 2023-05-05 19:11:47.105201 griptape-0.9.1/griptape/templates/prompts/tool.j2
+-rw-r--r--   0        0        0       40 2023-04-23 22:01:47.862316 griptape-0.9.1/griptape/templates/prompts/workflow.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.681023 griptape-0.9.1/griptape/templates/ramps/blob_storage.j2
+-rw-r--r--   0        0        0      131 2023-05-10 18:51:24.678788 griptape-0.9.1/griptape/templates/ramps/text_storage.j2
+-rw-r--r--   0        0        0      383 2023-04-24 18:12:25.639754 griptape-0.9.1/griptape/tokenizers/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-17 13:00:38.742159 griptape-0.9.1/griptape/tokenizers/base_tokenizer.py
+-rw-r--r--   0        0        0      683 2023-04-24 18:12:25.672520 griptape-0.9.1/griptape/tokenizers/cohere_tokenizer.py
+-rw-r--r--   0        0        0      674 2023-04-24 18:12:25.648974 griptape-0.9.1/griptape/tokenizers/hugging_face_tokenizer.py
+-rw-r--r--   0        0        0     1697 2023-05-17 11:38:47.481284 griptape-0.9.1/griptape/tokenizers/tiktoken_tokenizer.py
+-rw-r--r--   0        0        0      463 2023-04-27 20:13:16.215797 griptape-0.9.1/griptape/utils/__init__.py
+-rw-r--r--   0        0        0      567 2023-04-30 20:59:42.640287 griptape-0.9.1/griptape/utils/command_runner.py
+-rw-r--r--   0        0        0      507 2023-05-21 07:49:33.327055 griptape-0.9.1/griptape/utils/conversation.py
+-rw-r--r--   0        0        0      857 2023-04-23 21:18:54.936489 griptape-0.9.1/griptape/utils/j2.py
+-rw-r--r--   0        0        0      371 2023-04-06 20:17:23.179953 griptape-0.9.1/griptape/utils/manifest_validator.py
+-rw-r--r--   0        0        0        0 2023-05-06 19:56:24.051141 griptape-0.9.1/griptape/utils/marshmallow/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-06 19:58:37.405568 griptape-0.9.1/griptape/utils/marshmallow/fields/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-06 20:47:07.097992 griptape-0.9.1/griptape/utils/marshmallow/fields/bytes.py
+-rw-r--r--   0        0        0      206 2023-04-23 21:20:43.200189 griptape-0.9.1/griptape/utils/paths.py
+-rw-r--r--   0        0        0      751 2023-04-09 19:15:55.918730 griptape-0.9.1/griptape/utils/python_runner.py
+-rw-r--r--   0        0        0     1175 2023-05-21 19:46:18.515283 griptape-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5970 1970-01-01 00:00:00.000000 griptape-0.9.1/PKG-INFO
```

### Comparing `griptape-0.9.0/LICENSE` & `griptape-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/README.md` & `griptape-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/artifacts/base_artifact.py` & `griptape-0.9.1/griptape/artifacts/base_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/artifacts/blob_artifact.py` & `griptape-0.9.1/griptape/artifacts/blob_artifact.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 @define(frozen=True)
 class BlobArtifact(BaseArtifact):
     value: bytes = field()
     name: str = field(kw_only=True)
     dir: Optional[str] = field(default=None, kw_only=True)
 
     @dir.validator
-    def validate_tools(self, _, dir: Optional[str]) -> None:
+    def validate_dir(self, _, dir: Optional[str]) -> None:
         if dir and dir.startswith("/"):
             raise ValueError("path can't be absolute")
 
     @property
     def full_path(self) -> str:
         return os.path.join(self.dir, self.name) if self.dir else self.name
```

### Comparing `griptape-0.9.0/griptape/artifacts/list_artifact.py` & `griptape-0.9.1/griptape/artifacts/list_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/artifacts/text_artifact.py` & `griptape-0.9.1/griptape/artifacts/text_artifact.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/core/activity_mixin.py` & `griptape-0.9.1/griptape/core/activity_mixin.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/core/base_tool.py` & `griptape-0.9.1/griptape/core/base_tool.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/core/decorators.py` & `griptape-0.9.1/griptape/core/decorators.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/__init__.py` & `griptape-0.9.1/griptape/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/embedding/base_embedding_driver.py` & `griptape-0.9.1/griptape/drivers/embedding/base_embedding_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/embedding/openai_embedding_driver.py` & `griptape-0.9.1/griptape/drivers/embedding/openai_embedding_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/memory/disk_memory_driver.py` & `griptape-0.9.1/griptape/drivers/memory/disk_memory_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/prompt/base_prompt_driver.py` & `griptape-0.9.1/griptape/drivers/prompt/base_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/prompt/cohere_prompt_driver.py` & `griptape-0.9.1/griptape/drivers/prompt/cohere_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py` & `griptape-0.9.1/griptape/drivers/prompt/hugging_face_hub_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py` & `griptape-0.9.1/griptape/drivers/prompt/hugging_face_pipeline_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/prompt/openai_prompt_driver.py` & `griptape-0.9.1/griptape/drivers/prompt/openai_prompt_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/storage/blob/memory_blob_storage_driver.py` & `griptape-0.9.1/griptape/drivers/storage/blob/memory_blob_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/storage/text/dynamodb_text_storage_driver.py` & `griptape-0.9.1/griptape/drivers/storage/text/dynamodb_text_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/storage/text/memory_text_storage_driver.py` & `griptape-0.9.1/griptape/drivers/storage/text/memory_text_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/storage/vector/base_vector_storage_driver.py` & `griptape-0.9.1/griptape/drivers/storage/vector/base_vector_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/drivers/storage/vector/pinecone_vector_storage_driver.py` & `griptape-0.9.1/griptape/drivers/storage/vector/pinecone_vector_storage_driver.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/executors/base_executor.py` & `griptape-0.9.1/griptape/executors/base_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/executors/docker_executor.py` & `griptape-0.9.1/griptape/executors/docker_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/executors/local_executor.py` & `griptape-0.9.1/griptape/executors/local_executor.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/memory/buffer_memory.py` & `griptape-0.9.1/griptape/memory/buffer_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/memory/memory.py` & `griptape-0.9.1/griptape/memory/memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/memory/summary_memory.py` & `griptape-0.9.1/griptape/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/ramps/base_ramp.py` & `griptape-0.9.1/griptape/ramps/base_ramp.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/ramps/blob_storage_ramp.py` & `griptape-0.9.1/griptape/ramps/blob_storage_ramp.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/ramps/text_storage_ramp.py` & `griptape-0.9.1/griptape/ramps/text_storage_ramp.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/schemas/__init__.py` & `griptape-0.9.1/griptape/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/schemas/polymorphic_schema.py` & `griptape-0.9.1/griptape/schemas/polymorphic_schema.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/structures/agent.py` & `griptape-0.9.1/griptape/structures/agent.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/structures/pipeline.py` & `griptape-0.9.1/griptape/structures/pipeline.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/structures/structure.py` & `griptape-0.9.1/griptape/structures/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 from abc import ABC, abstractmethod
 from logging import Logger
 from typing import Optional, Union, TYPE_CHECKING
 from attr import define, field, Factory
 from rich.logging import RichHandler
 from griptape.drivers import BasePromptDriver, OpenAiPromptDriver
-from griptape.rules.ruleset import Ruleset
+from griptape.rules import Ruleset
 
 if TYPE_CHECKING:
     from griptape.tasks import BaseTask
 
 
 @define
 class Structure(ABC):
```

### Comparing `griptape-0.9.0/griptape/structures/structure_with_memory.py` & `griptape-0.9.1/griptape/structures/structure_with_memory.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/structures/workflow.py` & `griptape-0.9.1/griptape/structures/workflow.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/summarizers/prompt_driver_summarizer.py` & `griptape-0.9.1/griptape/summarizers/prompt_driver_summarizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tasks/action_subtask.py` & `griptape-0.9.1/griptape/tasks/action_subtask.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tasks/base_task.py` & `griptape-0.9.1/griptape/tasks/base_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tasks/prompt_task.py` & `griptape-0.9.1/griptape/tasks/prompt_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tasks/toolkit_task.py` & `griptape-0.9.1/griptape/tasks/toolkit_task.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/templates/prompts/tasks/toolkit/base.j2` & `griptape-0.9.1/griptape/templates/prompts/tasks/toolkit/base.j2`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tokenizers/base_tokenizer.py` & `griptape-0.9.1/griptape/tokenizers/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tokenizers/cohere_tokenizer.py` & `griptape-0.9.1/griptape/tokenizers/cohere_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tokenizers/hugging_face_tokenizer.py` & `griptape-0.9.1/griptape/tokenizers/hugging_face_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/tokenizers/tiktoken_tokenizer.py` & `griptape-0.9.1/griptape/tokenizers/tiktoken_tokenizer.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/utils/command_runner.py` & `griptape-0.9.1/griptape/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/utils/j2.py` & `griptape-0.9.1/griptape/utils/j2.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/griptape/utils/python_runner.py` & `griptape-0.9.1/griptape/utils/python_runner.py`

 * *Files identical despite different names*

### Comparing `griptape-0.9.0/pyproject.toml` & `griptape-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape"
-version = "0.9.0"
+version = "0.9.1"
 description = "Modular Python framework for LLM workflows, tools, memory, and data."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape"
 
 packages = [
```

### Comparing `griptape-0.9.0/PKG-INFO` & `griptape-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape
-Version: 0.9.0
+Version: 0.9.1
 Summary: Modular Python framework for LLM workflows, tools, memory, and data.
 Home-page: https://github.com/griptape-ai/griptape
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

