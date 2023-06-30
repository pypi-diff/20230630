# Comparing `tmp/langport-0.2.1.tar.gz` & `tmp/langport-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.2.1.tar", last modified: Wed Jun 21 04:12:11 2023, max compression
+gzip compressed data, was "langport-0.3.0.tar", last modified: Fri Jun 30 07:29:25 2023, max compression
```

## Comparing `langport-0.2.1.tar` & `langport-0.3.0.tar`

### file list

```diff
@@ -1,136 +1,143 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.2.1/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5596 2023-06-21 04:12:11.779040 langport-0.2.1/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5120 2023-06-21 04:11:50.000000 langport-0.2.1/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.2.1/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.2.1/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.2.1/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.2.1/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.2.1/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.2.1/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/mpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.2.1/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.2.1/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.2.1/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/codegen.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/falcon.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/starcoder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/text2vec.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5000 2023-06-21 04:11:50.000000 langport-0.2.1/langport/model/executor/generation/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15698 2023-06-21 04:11:50.000000 langport-0.2.1/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.2.1/langport/model/executor/ggml.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/executor/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.2.1/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-19 18:47:41.000000 langport-0.2.1/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.2.1/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.2.1/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.2.1/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.2.1/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/huggingface_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.2.1/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/tabby_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.2.1/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.775040 langport-0.2.1/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.2.1/langport/routers/gateway/common.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/gateway/openai_compatible.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.2.1/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.2.1/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.2.1/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/cluster_monitor.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/cluster_monitor_app.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/graphite_feeder.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/huggingface_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-21 04:11:50.000000 langport-0.2.1/langport/service/gateway/openai_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/gateway/tabby_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.2.1/langport/service/server/generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.2.1/langport/service/server/ggml_generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-21 04:11:44.000000 langport-0.2.1/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.2.1/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.2.1/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.2.1/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.2.1/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-21 04:11:50.000000 langport-0.2.1/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.779040 langport-0.2.1/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.2.1/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.2.1/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.2.1/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-21 04:12:11.771040 langport-0.2.1/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5596 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4172 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      237 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-21 04:12:11.000000 langport-0.2.1/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1082 2023-06-21 04:11:50.000000 langport-0.2.1/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-21 04:12:11.779040 langport-0.2.1/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.3.0/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5811 2023-06-30 07:29:25.437850 langport-0.3.0/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5311 2023-06-30 05:10:13.000000 langport-0.3.0/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.3.0/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.3.0/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.3.0/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.3.0/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.3.0/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.3.0/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6133 2023-06-30 07:16:30.000000 langport-0.3.0/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-06-30 07:13:56.000000 langport-0.3.0/langport/data/conversation/settings/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      262 2023-06-21 13:48:49.000000 langport-0.3.0/langport/data/conversation/settings/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.3.0/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.3.0/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.3.0/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      691 2023-06-21 13:45:50.000000 langport-0.3.0/langport/model/adapters/baichuan.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      631 2023-06-30 07:16:13.000000 langport-0.3.0/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      848 2023-06-21 13:47:17.000000 langport-0.3.0/langport/model/adapters/wizardlm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.3.0/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5000 2023-06-25 16:41:24.000000 langport-0.3.0/langport/model/executor/generation/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16189 2023-06-25 16:41:24.000000 langport-0.3.0/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2260 2023-06-21 04:13:56.000000 langport-0.3.0/langport/model/executor/generation/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2110 2023-06-18 13:11:45.000000 langport-0.3.0/langport/model/executor/ggml.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7679 2023-06-30 07:18:19.000000 langport-0.3.0/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1567 2023-06-21 14:56:58.000000 langport-0.3.0/langport/model/executor/optimum.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-30 05:32:15.000000 langport-0.3.0/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-30 07:22:43.000000 langport-0.3.0/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.3.0/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.3.0/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.3.0/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.3.0/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.3.0/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.3.0/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.433850 langport-0.3.0/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.3.0/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16286 2023-06-30 05:36:09.000000 langport-0.3.0/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.3.0/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.3.0/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-30 05:34:00.000000 langport-0.3.0/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.3.0/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4920 2023-06-25 16:41:24.000000 langport-0.3.0/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.3.0/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2614 2023-06-30 07:23:01.000000 langport-0.3.0/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2911 2023-06-18 13:11:45.000000 langport-0.3.0/langport/service/server/ggml_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2582 2023-06-21 04:13:56.000000 langport-0.3.0/langport/service/server/optimum_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7271 2023-06-30 05:09:13.000000 langport-0.3.0/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.3.0/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.3.0/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.3.0/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.3.0/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-06-25 16:41:24.000000 langport-0.3.0/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.437850 langport-0.3.0/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.3.0/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.3.0/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.3.0/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-30 07:29:25.429850 langport-0.3.0/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5811 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4473 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-30 07:29:25.000000 langport-0.3.0/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1127 2023-06-21 04:13:56.000000 langport-0.3.0/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-30 07:29:25.437850 langport-0.3.0/setup.cfg
```

### Comparing `langport-0.2.1/LICENSE` & `langport-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/PKG-INFO` & `langport-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: langport
-Version: 0.2.1
-Summary: A large language model serving platform.
-Project-URL: Homepage, https://github.com/vtuber-plan/langport
-Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: ggml
-License-File: LICENSE
-
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -40,21 +26,39 @@
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
+## Support Model Architectures
+* LLaMa
+* GLM
+* Bloom
+* OPT
+* GPT2
+* GPT Neo
+* GPT Big Code
+
+## Tested Models
+* LLaMa
+* Vicuna
+* ChatGLM
+* ChatGLM2
+* Falcon
+* Starcoder
+* WizardLM
+* OpenBuddy
+
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
-
 ## News
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -1,44 +1,39 @@
-Metadata-Version: 2.1 Name: langport Version: 0.2.1 Summary: A large language
-model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
-langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
-issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
-RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
-RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
-setting. We create 32 threads to submit chat tasks to the server, and the
-following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
-of FastChat and LangPort with different max model concurrency settings. !
-[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
+LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
+LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
+## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
+V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
+server, and the following figure shows the Queries Per Second (QPS) and Tokens
+Per Second (TPS) of FastChat and LangPort with different max model concurrency
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
+Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
+Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
+worker support. - [2023/06/01] Add HuggingFace text generation API support. -
+[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
+script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
+inference supported. - [2023/05/10] Langport project started. ## Install ###
+Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
+git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
+worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
+use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
+source 1. Clone this repository ```bash git clone https://github.com/vtuber-
+plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
 upgrade pip pip install -e . ``` ## Start the server It is simple to start a
 single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
```

### Comparing `langport-0.2.1/README.md` & `langport-0.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: langport
+Version: 0.3.0
+Summary: A large language model serving platform.
+Project-URL: Homepage, https://github.com/vtuber-plan/langport
+Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: ggml
+Provides-Extra: optimum
+License-File: LICENSE
+
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
   <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/vtuber-plan/langport?style=social">
 </a>
@@ -26,21 +41,39 @@
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
+## Support Model Architectures
+* LLaMa
+* GLM
+* Bloom
+* OPT
+* GPT2
+* GPT Neo
+* GPT Big Code
+
+## Tested Models
+* LLaMa
+* Vicuna
+* ChatGLM
+* ChatGLM2
+* Falcon
+* Starcoder
+* WizardLM
+* OpenBuddy
+
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
-
 ## News
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -1,37 +1,46 @@
+Metadata-Version: 2.1 Name: langport Version: 0.3.0 Summary: A large language
+model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
+langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
+Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
-RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
-RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
-setting. We create 32 threads to submit chat tasks to the server, and the
-following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
-of FastChat and LangPort with different max model concurrency settings. !
-[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
+LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
+LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
+## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
+V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
+server, and the following figure shows the Queries Per Second (QPS) and Tokens
+Per Second (TPS) of FastChat and LangPort with different max model concurrency
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
+Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
+Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
+worker support. - [2023/06/01] Add HuggingFace text generation API support. -
+[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
+script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
+inference supported. - [2023/05/10] Langport project started. ## Install ###
+Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
+git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
+worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
+use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
+source 1. Clone this repository ```bash git clone https://github.com/vtuber-
+plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
 upgrade pip pip install -e . ``` ## Start the server It is simple to start a
 single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
```

### Comparing `langport-0.2.1/langport/constants.py` & `langport-0.3.0/langport/constants.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/core/base_node.py` & `langport-0.3.0/langport/core/base_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/core/cluster_node.py` & `langport-0.3.0/langport/core/cluster_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/core/cluster_worker.py` & `langport-0.3.0/langport/core/cluster_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/data/conversation/__init__.py` & `langport-0.3.0/langport/data/conversation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ADD_COLON_TWO = auto()
     ADD_COLON_SPACE_SINGLE = auto()
     NO_COLON_SINGLE = auto()
     ADD_NEW_LINE_SINGLE = auto()
     DOLLY = auto()
     RWKV = auto()
     PHOENIX = auto()
+    CHATGLM = auto()
 
 
 @dataclasses.dataclass
 class ConversationSettings:
     # The name of this settings
     name: str
     # Two roles
@@ -124,14 +125,24 @@
             ret = self.system
             for role, message in self.messages:
                 if message:
                     ret += role + ": " + "<s>" + message + "</s>"
                 else:
                     ret += role + ": " + "<s>"
             return ret
+        elif self.settings.sep_style == SeparatorStyle.CHATGLM:
+            ret = self.system
+            for i, (role, message) in enumerate(self.messages):
+                if message:
+                    if i % 2 == 0:
+                        ret += f"[Round {i+1}]\n\n"
+                    ret += role + "：" + message + self.settings.sep
+                else:
+                    ret += role + "："
+            return ret
         else:
             raise ValueError(f"Invalid style: {self.settings.sep_style}")
 
     def append_message(self, role: str, message: str):
         """Append a new message."""
         self.messages.append([role, message])
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `langport-0.2.1/langport/data/conversation/conversation_settings.py` & `langport-0.3.0/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/baize.py` & `langport-0.3.0/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/bard.py` & `langport-0.3.0/langport/model/adapters/bard.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/billa.py` & `langport-0.3.0/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/chatgpt.py` & `langport-0.3.0/langport/model/adapters/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/claude.py` & `langport-0.3.0/langport/model/adapters/claude.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/dolly_v2.py` & `langport-0.3.0/langport/model/adapters/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/falcon.py` & `langport-0.3.0/langport/model/adapters/falcon.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/koala.py` & `langport-0.3.0/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/oasst_pythia.py` & `langport-0.3.0/langport/model/adapters/oasst_pythia.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/openbuddy.py` & `langport-0.3.0/langport/model/adapters/openbuddy.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/phoenix.py` & `langport-0.3.0/langport/model/adapters/phoenix.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/rwkv.py` & `langport-0.3.0/langport/model/adapters/rwkv.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/stable_lm.py` & `langport-0.3.0/langport/model/adapters/stable_lm.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/adapters/vicuna.py` & `langport-0.3.0/langport/model/adapters/vicuna.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/compression.py` & `langport-0.3.0/langport/model/compression.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/base.py` & `langport-0.3.0/langport/model/executor/base.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/embedding/__init__.py` & `langport-0.3.0/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/embedding/huggingface.py` & `langport-0.3.0/langport/model/executor/embedding/huggingface.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/generation/__init__.py` & `langport-0.3.0/langport/model/executor/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/generation/chatgpt.py` & `langport-0.3.0/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/generation/ggml.py` & `langport-0.3.0/langport/model/executor/generation/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/generation/huggingface.py` & `langport-0.3.0/langport/model/executor/generation/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,16 +202,27 @@
                 out = self.model.decoder(
                     input_ids=decoder_input_ids,
                     use_cache=self.model.generation_config.use_cache,
                     encoder_outputs=encoder_outputs,
                     past_key_values=past_key_values,
                 )
             else:
+                if step > 0:
+                    dynamic_attention_mask = torch.cat(
+                        (attention_mask, 
+                        torch.ones(
+                            inputs.batch_size, step,
+                            dtype=torch.long, device=decoder_input_ids.device
+                        )), dim=1
+                    )
+                else:
+                    dynamic_attention_mask = attention_mask
                 out = self.model(
                     input_ids=decoder_input_ids,
+                    attention_mask=dynamic_attention_mask,
                     use_cache=self.model.generation_config.use_cache,
                     past_key_values=past_key_values,
                 )
             logits = out.logits
             past_key_values = out.past_key_values
             decoder_input_ids_list = []
```

### Comparing `langport-0.2.1/langport/model/executor/ggml.py` & `langport-0.3.0/langport/model/executor/ggml.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/executor/huggingface.py` & `langport-0.3.0/langport/model/executor/huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from typing import Optional
 
 from langport.model.adapters.dolly_v2 import DollyV2Adapter
 from langport.model.adapters.rwkv import RwkvAdapter
 from langport.model.adapters.t5 import T5Adapter
 from langport.model.adapters.text2vec import BertAdapter
+from langport.model.adapters.chatglm import ChatGLMAdapter
+
 from langport.model.executor.base import LocalModelExecutor
 
 import torch
 
 from transformers import (
     AutoModelForCausalLM,
+    AutoModel,
     AutoTokenizer,
     AutoModelForSeq2SeqLM,
     T5Tokenizer,
     BertTokenizer,
     BertModel,
 )
 
@@ -73,17 +76,24 @@
             tokenizer = T5Tokenizer.from_pretrained(model_path, use_fast=False)
             model = AutoModelForSeq2SeqLM.from_pretrained(
                 model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
             )
         elif isinstance(adapter, BertAdapter):
             tokenizer = BertTokenizer.from_pretrained(model_path)
             model = BertModel.from_pretrained(model_path, **from_pretrained_kwargs)
-
+        elif isinstance(adapter, ChatGLMAdapter):
+            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False, trust_remote_code=True)
+            if "trust_remote_code" in from_pretrained_kwargs:
+                from_pretrained_kwargs.pop("trust_remote_code")
+            model = AutoModel.from_pretrained(
+                model_path, low_cpu_mem_usage=True, trust_remote_code=True, **from_pretrained_kwargs
+            )
         else:
-            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
+            trust_remote_code = from_pretrained_kwargs.get("trust_remote_code", False)
+            tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False, trust_remote_code=trust_remote_code)
             model = AutoModelForCausalLM.from_pretrained(
                 model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
             )
 
         return model, tokenizer
 
     def load_model(
```

### Comparing `langport-0.2.1/langport/model/model_adapter.py` & `langport-0.3.0/langport/model/model_adapter.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/model_args.py` & `langport-0.3.0/langport/model/model_args.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/models/rwkv_model.py` & `langport-0.3.0/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/model/monkey_patch_non_inplace.py` & `langport-0.3.0/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/protocol/huggingface_api_protocol.py` & `langport-0.3.0/langport/protocol/huggingface_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/protocol/openai_api_protocol.py` & `langport-0.3.0/langport/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/protocol/tabby_api_protocol.py` & `langport-0.3.0/langport/protocol/tabby_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/protocol/worker_protocol.py` & `langport-0.3.0/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/routers/gateway/common.py` & `langport-0.3.0/langport/routers/gateway/common.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/routers/gateway/openai_compatible.py` & `langport-0.3.0/langport/routers/gateway/openai_compatible.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     temperature: float,
     top_p: float,
     max_tokens: Optional[int],
     echo: Optional[bool],
     stream: Optional[bool],
     stop: Optional[Union[str, List[str]]],
 ) -> Dict[str, Any]:
-    is_chatglm = "chatglm" in model_name.lower()
+    # is_chatglm = "chatglm" in model_name.lower()
     conv = get_conversation_template(model_name)
 
     if isinstance(messages, str):
         prompt = messages
     else:
         for message in messages:
             msg_role = message["role"]
@@ -84,19 +84,15 @@
             elif msg_role == "assistant":
                 conv.append_message(conv.settings.roles[1], message["content"])
             else:
                 raise ValueError(f"Unknown role: {msg_role}")
 
         # Add a blank message for the assistant.
         conv.append_message(conv.settings.roles[1], None)
-
-        if is_chatglm:
-            prompt = conv.messages[conv.offset :]
-        else:
-            prompt = conv.get_prompt()
+        prompt = conv.get_prompt()
 
     if max_tokens is None:
         max_tokens = 512
 
     gen_params = {
         "model": model_name,
         "prompt": prompt,
```

### Comparing `langport-0.2.1/langport/routers/server/core_node.py` & `langport-0.3.0/langport/routers/server/core_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/routers/server/embedding_node.py` & `langport-0.3.0/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/routers/server/generation_node.py` & `langport-0.3.0/langport/routers/server/generation_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/cluster_monitor.py` & `langport-0.3.0/langport/service/gateway/cluster_monitor.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/cluster_monitor_app.py` & `langport-0.3.0/langport/service/gateway/cluster_monitor_app.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/fauxpilot_api.py` & `langport-0.3.0/langport/service/gateway/fauxpilot_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/graphite_feeder.py` & `langport-0.3.0/langport/service/gateway/graphite_feeder.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/huggingface_api.py` & `langport-0.3.0/langport/service/gateway/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/openai_api.py` & `langport-0.3.0/langport/service/gateway/openai_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/gateway/tabby_api.py` & `langport-0.3.0/langport/service/gateway/tabby_api.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/server/chatgpt_generation_worker.py` & `langport-0.3.0/langport/service/server/chatgpt_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/server/dummy_worker.py` & `langport-0.3.0/langport/service/server/dummy_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/server/embedding_worker.py` & `langport-0.3.0/langport/service/server/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/service/server/generation_worker.py` & `langport-0.3.0/langport/service/server/generation_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         num_gpus=args.num_gpus,
         max_gpu_memory=args.max_gpu_memory,
         load_8bit=args.load_8bit,
         cpu_offloading=args.cpu_offloading,
         deepspeed=args.deepspeed,
         trust_remote_code=args.trust_remote_code
     )
-
+    
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
         limit_model_concurrency=args.limit_model_concurrency,
         max_batch=args.batch,
```

### Comparing `langport-0.2.1/langport/service/server/ggml_generation_worker.py` & `langport-0.3.0/langport/service/server/ggml_generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/utils/__init__.py` & `langport-0.3.0/langport/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,26 @@
                     "we recommend you use Python >= 3.9 for UTF-8 encoding."
                 )
             logging.basicConfig(level=logging.INFO)
     logging.getLogger().handlers[0].setFormatter(formatter)
 
     # Redirect stdout and stderr to loggers
     stdout_logger = logging.getLogger("stdout")
-    stdout_logger.setLevel(logging.INFO)
+    stdout_logger.setLevel(logging.DEBUG)
     sl = StreamToLogger(stdout_logger, logging.INFO)
     sys.stdout = sl
 
-    stderr_logger = logging.getLogger("stderr")
-    stderr_logger.setLevel(logging.ERROR)
-    sl = StreamToLogger(stderr_logger, logging.ERROR)
-    sys.stderr = sl
+    # stderr_logger = logging.getLogger("stderr")
+    # stderr_logger.setLevel(logging.ERROR)
+    # sl = StreamToLogger(stderr_logger, logging.ERROR)
+    # sys.stderr = sl
 
     # Get logger
     logger = logging.getLogger(logger_name)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(logging.DEBUG)
 
     # Add a file handler for all loggers
     if handler is None:
         os.makedirs(LOGDIR, exist_ok=True)
         filename = os.path.join(LOGDIR, logger_filename)
         handler = logging.handlers.TimedRotatingFileHandler(
             filename, when="D", utc=True, encoding="utf-8"
```

### Comparing `langport-0.2.1/langport/utils/evaluation.py` & `langport-0.3.0/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/utils/http_pool.py` & `langport-0.3.0/langport/utils/http_pool.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/utils/interval_timer.py` & `langport-0.3.0/langport/utils/interval_timer.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/workers/embedding_worker.py` & `langport-0.3.0/langport/workers/embedding_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport/workers/generation_worker.py` & `langport-0.3.0/langport/workers/generation_worker.py`

 * *Files identical despite different names*

### Comparing `langport-0.2.1/langport.egg-info/PKG-INFO` & `langport-0.3.0/langport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: langport
-Version: 0.2.1
+Version: 0.3.0
 Summary: A large language model serving platform.
 Project-URL: Homepage, https://github.com/vtuber-plan/langport
 Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: ggml
+Provides-Extra: optimum
 License-File: LICENSE
 
 <div align="center">
 
 # LangPort
 
 <a href="https://github.com/vtuber-plan/langport">
@@ -40,21 +41,39 @@
 - Batch inference for higher throughput.
 - Support for encoder-only, decoder-only and encoder-decoder models.
 - OpenAI-compatible RESTful APIs.
 - FauxPilot-compatible RESTful APIs.
 - HuggingFace-compatible RESTful APIs.
 - Tabby-compatible RESTful APIs.
 
+## Support Model Architectures
+* LLaMa
+* GLM
+* Bloom
+* OPT
+* GPT2
+* GPT Neo
+* GPT Big Code
+
+## Tested Models
+* LLaMa
+* Vicuna
+* ChatGLM
+* ChatGLM2
+* Falcon
+* Starcoder
+* WizardLM
+* OpenBuddy
+
 ## Benchmark
 We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16 setting.
 We create 32 threads to submit chat tasks to the server, and the following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS) of FastChat and LangPort with different max model concurrency settings.
 
 ![benchmark_chat](assets/benchmark_chat.jpg)
 
-
 ## News
 - [2023/06/18] Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support.
 - [2023/06/09] Add LLama.cpp worker support.
 - [2023/06/01] Add HuggingFace Bert embedding worker support.
 - [2023/06/01] Add HuggingFace text generation API support.
 - [2023/06/01] Add tabby API support.
 - [2023/05/23] Add chat throughput test script.
```

#### html2text {}

```diff
@@ -1,44 +1,46 @@
-Metadata-Version: 2.1 Name: langport Version: 0.2.1 Summary: A large language
+Metadata-Version: 2.1 Name: langport Version: 0.3.0 Summary: A large language
 model serving platform. Project-URL: Homepage, https://github.com/vtuber-plan/
 langport Project-URL: Bug Tracker, https://github.com/vtuber-plan/langport/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
-Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml License-
-File: LICENSE
+Content-Type: text/markdown Provides-Extra: dev Provides-Extra: ggml Provides-
+Extra: optimum License-File: LICENSE
        # LangPort [GitHub_Repo_stars] [License] ![architecture](assets/
                                architecture.jpg)
 LangPort is a open-source large language model serving platform. Our goal is to
 build a super fast LLM inference service. This project is inspired by [lmsys/
 fastchat](https://github.com/lm-sys/FastChat), we hope that the serving
 platform is lightweight and fast, but fastchat includes other features such as
 training and evaluation make it complicated. The core features include: -
 Huggingface transformers support. - ggml (llama.cpp) support. - A distributed
 serving system for state-of-the-art models. - Streaming generation support with
 various decoding strategies. - Batch inference for higher throughput. - Support
 for encoder-only, decoder-only and encoder-decoder models. - OpenAI-compatible
 RESTful APIs. - FauxPilot-compatible RESTful APIs. - HuggingFace-compatible
-RESTful APIs. - Tabby-compatible RESTful APIs. ## Benchmark We use single
-RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy V0.9) under the bf16
-setting. We create 32 threads to submit chat tasks to the server, and the
-following figure shows the Queries Per Second (QPS) and Tokens Per Second (TPS)
-of FastChat and LangPort with different max model concurrency settings. !
-[benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18] Add ggml
-(llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09] Add
-LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding worker
-support. - [2023/06/01] Add HuggingFace text generation API support. - [2023/
-06/01] Add tabby API support. - [2023/05/23] Add chat throughput test script. -
-[2023/05/22] New distributed architecture. - [2023/05/14] Batch inference
-supported. - [2023/05/10] Langport project started. ## Install ### Method 1:
-With pip ```bash pip install langport ``` or: ```bash pip install git+https://
-github.com/vtuber-plan/langport.git ``` If you need ggml generation worker, use
-this command: ```bash pip install langport[ggml] ``` If you wanna use GPU:
-```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From source 1.
-Clone this repository ```bash git clone https://github.com/vtuber-plan/
-langport.git cd langport ``` 2. Install the Package ```bash pip install --
+RESTful APIs. - Tabby-compatible RESTful APIs. ## Support Model Architectures *
+LLaMa * GLM * Bloom * OPT * GPT2 * GPT Neo * GPT Big Code ## Tested Models *
+LLaMa * Vicuna * ChatGLM * ChatGLM2 * Falcon * Starcoder * WizardLM * OpenBuddy
+## Benchmark We use single RTX3090 to run a finetuned 7B LLaMA model (OpenBuddy
+V0.9) under the bf16 setting. We create 32 threads to submit chat tasks to the
+server, and the following figure shows the Queries Per Second (QPS) and Tokens
+Per Second (TPS) of FastChat and LangPort with different max model concurrency
+settings. ![benchmark_chat](assets/benchmark_chat.jpg) ## News - [2023/06/18]
+Add ggml (llama.cpp gpt.cpp starcoder.cpp etc.) worker support. - [2023/06/09]
+Add LLama.cpp worker support. - [2023/06/01] Add HuggingFace Bert embedding
+worker support. - [2023/06/01] Add HuggingFace text generation API support. -
+[2023/06/01] Add tabby API support. - [2023/05/23] Add chat throughput test
+script. - [2023/05/22] New distributed architecture. - [2023/05/14] Batch
+inference supported. - [2023/05/10] Langport project started. ## Install ###
+Method 1: With pip ```bash pip install langport ``` or: ```bash pip install
+git+https://github.com/vtuber-plan/langport.git ``` If you need ggml generation
+worker, use this command: ```bash pip install langport[ggml] ``` If you wanna
+use GPU: ```bash CT_CUBLAS=1 pip install langport[ggml] ``` ### Method 2: From
+source 1. Clone this repository ```bash git clone https://github.com/vtuber-
+plan/langport.git cd langport ``` 2. Install the Package ```bash pip install --
 upgrade pip pip install -e . ``` ## Start the server It is simple to start a
 single node chat API service: ``` bash python -
 m langport.service.server.generation_worker --port 21001 --model-path  python -
 m langport.service.gateway.openai_api ``` If you need the embeddings API or
 other features, you can deploy a distributed inference cluster: ``` bash python
 -m langport.service.server.dummy_worker --port 21001 python -
 m langport.service.server.generation_worker --model-path  --neighbors http://
```

### Comparing `langport-0.2.1/langport.egg-info/SOURCES.txt` & `langport-0.3.0/langport.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 langport/data/__init__.py
 langport/data/conversation/__init__.py
 langport/data/conversation/conversation_settings.py
 langport/data/conversation/settings/__init__.py
 langport/data/conversation/settings/baize.py
 langport/data/conversation/settings/bard.py
 langport/data/conversation/settings/billa.py
+langport/data/conversation/settings/chatglm.py
 langport/data/conversation/settings/chatgpt.py
 langport/data/conversation/settings/claude.py
 langport/data/conversation/settings/dolly.py
 langport/data/conversation/settings/falcon.py
 langport/data/conversation/settings/h2ogpt.py
 langport/data/conversation/settings/koala.py
 langport/data/conversation/settings/mpt.py
@@ -32,21 +33,23 @@
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
 langport/data/conversation/settings/redpajama.py
 langport/data/conversation/settings/rwkv.py
 langport/data/conversation/settings/stablelm.py
 langport/data/conversation/settings/vicuna.py
+langport/data/conversation/settings/wizardlm.py
 langport/data/conversation/settings/zero_shot.py
 langport/model/__init__.py
 langport/model/compression.py
 langport/model/model_adapter.py
 langport/model/model_args.py
 langport/model/monkey_patch_non_inplace.py
 langport/model/adapters/__init__.py
+langport/model/adapters/baichuan.py
 langport/model/adapters/baize.py
 langport/model/adapters/bard.py
 langport/model/adapters/billa.py
 langport/model/adapters/chatglm.py
 langport/model/adapters/chatgpt.py
 langport/model/adapters/claude.py
 langport/model/adapters/codegen.py
@@ -58,24 +61,27 @@
 langport/model/adapters/phoenix.py
 langport/model/adapters/rwkv.py
 langport/model/adapters/stable_lm.py
 langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
 langport/model/adapters/text2vec.py
 langport/model/adapters/vicuna.py
+langport/model/adapters/wizardlm.py
 langport/model/executor/__init__.py
 langport/model/executor/base.py
 langport/model/executor/ggml.py
 langport/model/executor/huggingface.py
+langport/model/executor/optimum.py
 langport/model/executor/embedding/__init__.py
 langport/model/executor/embedding/huggingface.py
 langport/model/executor/generation/__init__.py
 langport/model/executor/generation/chatgpt.py
 langport/model/executor/generation/ggml.py
 langport/model/executor/generation/huggingface.py
+langport/model/executor/generation/optimum.py
 langport/model/models/__init__.py
 langport/model/models/rwkv_model.py
 langport/protocol/__init__.py
 langport/protocol/huggingface_api_protocol.py
 langport/protocol/openai_api_protocol.py
 langport/protocol/tabby_api_protocol.py
 langport/protocol/worker_protocol.py
@@ -98,14 +104,15 @@
 langport/service/gateway/tabby_api.py
 langport/service/server/__init__.py
 langport/service/server/chatgpt_generation_worker.py
 langport/service/server/dummy_worker.py
 langport/service/server/embedding_worker.py
 langport/service/server/generation_worker.py
 langport/service/server/ggml_generation_worker.py
+langport/service/server/optimum_generation_worker.py
 langport/utils/__init__.py
 langport/utils/cache_state.py
 langport/utils/evaluation.py
 langport/utils/http_pool.py
 langport/utils/interval_timer.py
 langport/workers/__init__.py
 langport/workers/embedding_worker.py
```

### Comparing `langport-0.2.1/pyproject.toml` & `langport-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.2.1"
+version = "0.3.0"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -18,14 +18,15 @@
     "shortuuid", "shortuuid", "tokenizers>=0.12.1", "torch",
     "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb", "tenacity>=8.2.2",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
 ggml = ["ctransformers"]
+optimum = ["onnx", "onnxruntime", "optimum"]
 
 [project.urls]
 "Homepage" = "https://github.com/vtuber-plan/langport"
 "Bug Tracker" = "https://github.com/vtuber-plan/langport/issues"
 
 [tool.setuptools.packages.find]
 exclude = ["assets*", "benchmark*", "docs", "dist*", "playground*", "scripts*", "tests*"]
```

