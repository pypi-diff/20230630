# Comparing `tmp/chatllm-2023.6.29.9.57.33.tar.gz` & `tmp/chatllm-2023.6.30.13.19.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2023.6.29.9.57.33.tar", last modified: Thu Jun 29 01:57:33 2023, max compression
+gzip compressed data, was "chatllm-2023.6.30.13.19.48.tar", last modified: Fri Jun 30 05:19:48 2023, max compression
```

## Comparing `chatllm-2023.6.29.9.57.33.tar` & `chatllm-2023.6.30.13.19.48.tar`

### file list

```diff
@@ -1,139 +1,142 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.766459 chatllm-2023.6.29.9.57.33/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.29.9.57.33/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-06-29 01:47:04.000000 chatllm-2023.6.29.9.57.33/LLMS.md
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.29.9.57.33/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     6710 2023-06-29 01:57:33.766276 chatllm-2023.6.29.9.57.33/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     5980 2023-06-29 01:47:04.000000 chatllm-2023.6.29.9.57.33/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.29.9.57.33/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-27 09:07:59.000000 chatllm-2023.6.29.9.57.33/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.744710 chatllm-2023.6.29.9.57.33/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.746161 chatllm-2023.6.29.9.57.33/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.29.9.57.33/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.29.9.57.33/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.29.9.57.33/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.29.9.57.33/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.746535 chatllm-2023.6.29.9.57.33/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.29.9.57.33/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.29.9.57.33/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.747796 chatllm-2023.6.29.9.57.33/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.29.9.57.33/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.29.9.57.33/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      659 2023-06-02 12:12:32.000000 chatllm-2023.6.29.9.57.33/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2023.6.29.9.57.33/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.29.9.57.33/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.29.9.57.33/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.748514 chatllm-2023.6.29.9.57.33/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     4928 2023-06-04 07:21:05.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3422 2023-06-26 05:20:07.000000 chatllm-2023.6.29.9.57.33/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.29.9.57.33/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.29.9.57.33/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.750232 chatllm-2023.6.29.9.57.33/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.29.9.57.33/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.29.9.57.33/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.750594 chatllm-2023.6.29.9.57.33/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1087 2023-06-15 09:17:56.000000 chatllm-2023.6.29.9.57.33/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.29.9.57.33/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.29.9.57.33/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.751196 chatllm-2023.6.29.9.57.33/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2023.6.29.9.57.33/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2305 2023-06-29 01:00:10.000000 chatllm-2023.6.29.9.57.33/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1282 2023-06-29 01:56:12.000000 chatllm-2023.6.29.9.57.33/chatllm/llms/chatgpt.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.29.9.57.33/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.29.9.57.33/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.751444 chatllm-2023.6.29.9.57.33/chatllm/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2023.6.29.9.57.33/chatllm/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-20 08:01:27.000000 chatllm-2023.6.29.9.57.33/chatllm/prompts/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.752162 chatllm-2023.6.29.9.57.33/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-06-02 10:18:35.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.29.9.57.33/chatllm/utils/nbce_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.753169 chatllm-2023.6.29.9.57.33/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.29.9.57.33/chatllm/webui/visualglm_st.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.745628 chatllm-2023.6.29.9.57.33/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     6710 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2766 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-29 01:57:33.000000 chatllm-2023.6.29.9.57.33/chatllm.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.756119 chatllm-2023.6.29.9.57.33/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.759274 chatllm-2023.6.29.9.57.33/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.29.9.57.33/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.29.9.57.33/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.29.9.57.33/data/imgs/chatbox.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.29.9.57.33/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.29.9.57.33/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.29.9.57.33/data/imgs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.29.9.57.33/data/imgs/img_1.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.29.9.57.33/data/imgs/role.png
--rw-r--r--   0 betterme   (501) staff       (20)   484220 2023-06-06 10:32:35.000000 chatllm-2023.6.29.9.57.33/data/imgs/群.png
--rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.29.9.57.33/data/openai_keys.md
--rw-r--r--   0 betterme   (501) staff       (20)  1242960 2023-06-26 02:02:22.000000 chatllm-2023.6.29.9.57.33/data/中职职教高考政策解读.pdf
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.761863 chatllm-2023.6.29.9.57.33/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.29.9.57.33/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.29.9.57.33/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.29.9.57.33/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.29.9.57.33/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.29.9.57.33/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.29.9.57.33/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.29.9.57.33/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.765638 chatllm-2023.6.29.9.57.33/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      346 2023-06-29 01:47:04.000000 chatllm-2023.6.29.9.57.33/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.29.9.57.33/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.29.9.57.33/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.29.9.57.33/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.29.9.57.33/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.29.9.57.33/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.29.9.57.33/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-29 01:57:33.766509 chatllm-2023.6.29.9.57.33/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-06-20 06:25:34.000000 chatllm-2023.6.29.9.57.33/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-29 01:57:33.766015 chatllm-2023.6.29.9.57.33/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.29.9.57.33/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.29.9.57.33/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.846708 chatllm-2023.6.30.13.19.48/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.30.13.19.48/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-06-29 01:47:04.000000 chatllm-2023.6.30.13.19.48/LLMS.md
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.30.13.19.48/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6909 2023-06-30 05:19:48.846520 chatllm-2023.6.30.13.19.48/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     6178 2023-06-29 08:10:09.000000 chatllm-2023.6.30.13.19.48/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.30.13.19.48/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-27 09:07:59.000000 chatllm-2023.6.30.13.19.48/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.791191 chatllm-2023.6.30.13.19.48/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.793374 chatllm-2023.6.30.13.19.48/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.793923 chatllm-2023.6.30.13.19.48/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.30.13.19.48/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.30.13.19.48/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.796232 chatllm-2023.6.30.13.19.48/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.30.13.19.48/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.30.13.19.48/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      659 2023-06-02 12:12:32.000000 chatllm-2023.6.30.13.19.48/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2023.6.30.13.19.48/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.30.13.19.48/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.30.13.19.48/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.797702 chatllm-2023.6.30.13.19.48/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4928 2023-06-04 07:21:05.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3422 2023-06-26 05:20:07.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.30.13.19.48/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.30.13.19.48/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.801821 chatllm-2023.6.30.13.19.48/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.30.13.19.48/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.802341 chatllm-2023.6.30.13.19.48/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1087 2023-06-15 09:17:56.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.30.13.19.48/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.30.13.19.48/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.803753 chatllm-2023.6.30.13.19.48/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2305 2023-06-29 01:00:10.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1323 2023-06-29 02:49:42.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/chatgpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.804255 chatllm-2023.6.30.13.19.48/chatllm/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2023.6.30.13.19.48/chatllm/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-20 08:01:27.000000 chatllm-2023.6.30.13.19.48/chatllm/prompts/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.805662 chatllm-2023.6.30.13.19.48/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-06-02 10:18:35.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.808688 chatllm-2023.6.30.13.19.48/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      221 2023-06-29 07:28:40.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.792404 chatllm-2023.6.30.13.19.48/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6909 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2837 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.815876 chatllm-2023.6.30.13.19.48/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.827421 chatllm-2023.6.30.13.19.48/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.30.13.19.48/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.30.13.19.48/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)   141276 2023-06-29 08:09:29.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatmind.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.30.13.19.48/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.30.13.19.48/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.30.13.19.48/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)     9900 2023-06-30 05:19:08.000000 chatllm-2023.6.30.13.19.48/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.30.13.19.48/data/openai_keys.md
+-rw-r--r--   0 betterme   (501) staff       (20)   678357 2023-06-29 02:05:32.000000 chatllm-2023.6.30.13.19.48/data/中职职教高考政策解读.pdf
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.831174 chatllm-2023.6.30.13.19.48/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.30.13.19.48/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.30.13.19.48/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)   606941 2023-06-29 02:21:44.000000 chatllm-2023.6.30.13.19.48/data/孙子兵法.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.30.13.19.48/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.845081 chatllm-2023.6.30.13.19.48/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      342 2023-06-29 08:04:00.000000 chatllm-2023.6.30.13.19.48/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.30.13.19.48/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.30.13.19.48/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.30.13.19.48/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.30.13.19.48/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.30.13.19.48/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.30.13.19.48/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-30 05:19:48.846760 chatllm-2023.6.30.13.19.48/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-06-20 06:25:34.000000 chatllm-2023.6.30.13.19.48/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.845770 chatllm-2023.6.30.13.19.48/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.30.13.19.48/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tox.ini
```

### Comparing `chatllm-2023.6.29.9.57.33/.gitignore` & `chatllm-2023.6.30.13.19.48/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/.travis.yml` & `chatllm-2023.6.30.13.19.48/.travis.yml`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/LICENSE` & `chatllm-2023.6.30.13.19.48/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/LLMS.md` & `chatllm-2023.6.30.13.19.48/LLMS.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/Makefile` & `chatllm-2023.6.30.13.19.48/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/PKG-INFO` & `chatllm-2023.6.30.13.19.48/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.29.9.57.33
+Version: 2023.6.30.13.19.48
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -81,14 +81,26 @@
 - 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
   ![客户端](data/imgs/chatbox.png)
 
 ### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
 
 </details>
 
+## ChatMind
+
+<details markdown="1">
+  <summary>Click to ChatMind</summary>
+
+```shell
+pip install "chatllm" && chatllm-run webui --name chatmind
+```
+![客户端](data/imgs/chatmind.png)
+
+</details>
+
 ## ChatPDF
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
 ```shell
 pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
```

### Comparing `chatllm-2023.6.29.9.57.33/README.md` & `chatllm-2023.6.30.13.19.48/README.md.bak`

 * *Files 3% similar despite different names*

```diff
@@ -12,63 +12,57 @@
 pip install -U chatllm
 ```
 
 ## [Docs](https://yuanjie-ai.github.io/ChatLLM/)
 
 ## Usages
 
-### [目前适配的LLMs](LLMS.md)
-
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
 for i in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
     print(i, end='')
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 
-## OpenaiEcosystem
+- 支持角色扮演
+  ![img.png](data/imgs/role.png)
 
+## OpenaiEcosystem
 <details markdown="1">
   <summary>Click to 无缝对接openai生态</summary>
 
 ```shell
 # 服务端
 pip install "chatllm[openai]" && chatllm-run openai <本地模型地址>
 ```
-
-- SDK：`pip install openai`
-
 ```python
+# 客户端
 import openai
 
 openai.api_base = 'http://0.0.0.0:8000/v1'
 openai.api_key = 'chatllm'
 prompt = "你好"
 completion = openai.Completion.create(prompt=prompt, stream=True, model="text-davinci-003")
 for c in completion:
     print(c.choices[0].text, end='')
 # 你好👋!我是人工智能助手 ChatGLM-6B,很高兴见到你，欢迎问我任何问题。
 ```
-
-- 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
-  ![客户端](data/imgs/chatbox.png)
-
 ### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
-
 </details>
 
 ## ChatPDF
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
+
 ```shell
 pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
 ```
 
 - python交互
 
 ```python
@@ -93,15 +87,15 @@
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
   | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-        | -------------- | ------------------------- | --------------------------------- |
+      | -------------- | ------------------------- | --------------------------------- |
   | FP16（无量化） | 13 GB                     | 14 GB                             |
   | INT8           | 8 GB                     | 9 GB                             |
   | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
     - [安装指南](docs/INSTALL.md)
@@ -162,15 +156,14 @@
     - [x] 利用 Fastapi/Flask/Grpc
       实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
     - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
 ## 交流群
-
 <div align=center>
 <img src="data/imgs/群.png" alt="群" width="250" height="400">
 </div>
 
 > 若二维码失效加微信拉群 313303303
```

### Comparing `chatllm-2023.6.29.9.57.33/README.md.bak` & `chatllm-2023.6.30.13.19.48/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,57 +12,75 @@
 pip install -U chatllm
 ```
 
 ## [Docs](https://yuanjie-ai.github.io/ChatLLM/)
 
 ## Usages
 
+### [目前适配的LLMs](LLMS.md)
+
 ```python
 from chatllm.applications import ChatBase
 
 qa = ChatBase()
 qa.load_llm(model_name_or_path="THUDM/chatglm-6b")
 for i in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
     print(i, end='')
 # 根据已知信息无法回答该问题，因为周杰伦是中国内地流行歌手、演员、音乐制作人、导演，
 # 是具有一定的知名度和专业能力的人物，没有提供足够的信息无法判断他是傻子。
 ```
 
-- 支持角色扮演
-  ![img.png](data/imgs/role.png)
-
 ## OpenaiEcosystem
+
 <details markdown="1">
   <summary>Click to 无缝对接openai生态</summary>
 
 ```shell
 # 服务端
 pip install "chatllm[openai]" && chatllm-run openai <本地模型地址>
 ```
+
+- SDK：`pip install openai`
+
 ```python
-# 客户端
 import openai
 
 openai.api_base = 'http://0.0.0.0:8000/v1'
 openai.api_key = 'chatllm'
 prompt = "你好"
 completion = openai.Completion.create(prompt=prompt, stream=True, model="text-davinci-003")
 for c in completion:
     print(c.choices[0].text, end='')
 # 你好👋!我是人工智能助手 ChatGLM-6B,很高兴见到你，欢迎问我任何问题。
 ```
+
+- 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
+  ![客户端](data/imgs/chatbox.png)
+
 ### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
+
+</details>
+
+## ChatMind
+
+<details markdown="1">
+  <summary>Click to ChatMind</summary>
+
+```shell
+pip install "chatllm" && chatllm-run webui --name chatmind
+```
+![客户端](data/imgs/chatmind.png)
+
 </details>
 
 ## ChatPDF
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
-
 ```shell
 pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
 ```
 
 - python交互
 
 ```python
@@ -87,15 +105,15 @@
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
   | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-      | -------------- | ------------------------- | --------------------------------- |
+        | -------------- | ------------------------- | --------------------------------- |
   | FP16（无量化） | 13 GB                     | 14 GB                             |
   | INT8           | 8 GB                     | 9 GB                             |
   | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
     - [安装指南](docs/INSTALL.md)
@@ -156,14 +174,15 @@
     - [x] 利用 Fastapi/Flask/Grpc
       实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
     - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
 ## 交流群
+
 <div align=center>
 <img src="data/imgs/群.png" alt="群" width="250" height="400">
 </div>
 
 > 若二维码失效加微信拉群 313303303
```

### Comparing `chatllm-2023.6.29.9.57.33/TODO.md` & `chatllm-2023.6.30.13.19.48/TODO.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/_his/FaissANN.py` & `chatllm-2023.6.30.13.19.48/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/_his/_chatllm.py` & `chatllm-2023.6.30.13.19.48/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/_his/_qa.py` & `chatllm-2023.6.30.13.19.48/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/aigc/common.py` & `chatllm-2023.6.30.13.19.48/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/app.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/config.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/datamodels.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/openai_client.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/routes/api.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/routes/base.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/routes/completions.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/routes/completions.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/routes/embeddings.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/routes/responses.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/routes/responses.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/sse_api.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/api/test.py` & `chatllm-2023.6.30.13.19.48/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/__chatbase.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/chatann.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/chatbase.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/chatpdf.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.30.13.19.48/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/chatyuan.py` & `chatllm-2023.6.30.13.19.48/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/clis/cli.py` & `chatllm-2023.6.30.13.19.48/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/closeai.py` & `chatllm-2023.6.30.13.19.48/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/embedding.py` & `chatllm-2023.6.30.13.19.48/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/llms/__init__.py` & `chatllm-2023.6.30.13.19.48/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/llms/chatglm.py` & `chatllm-2023.6.30.13.19.48/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/llms/chatgpt.py` & `chatllm-2023.6.30.13.19.48/chatllm/llms/chatgpt.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 # @Project      : AI.  @by PyCharm
 # @File         : chatgpt
 # @Time         : 2023/6/29 08:52
 # @Author       : betterme
 # @WeChat       : meutils
 # @Software     : PyCharm
-# @Description  :
+# @Description  : https://api2d-doc.apifox.cn/api-84787447
 
 from meutils.pipe import *
 
 
 def load_llm4chat(**kwargs):
     import openai
```

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/llms/demo.py` & `chatllm-2023.6.30.13.19.48/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/llms/llama.py` & `chatllm-2023.6.30.13.19.48/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/prompts/common.py` & `chatllm-2023.6.30.13.19.48/chatllm/prompts/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/utils/common.py` & `chatllm-2023.6.30.13.19.48/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.30.13.19.48/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/utils/nbce.py` & `chatllm-2023.6.30.13.19.48/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/utils/nbce_test.py` & `chatllm-2023.6.30.13.19.48/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/webui/chatbase.py` & `chatllm-2023.6.30.13.19.48/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/webui/chatpdf.py` & `chatllm-2023.6.30.13.19.48/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.30.13.19.48/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/webui/nice_ui.py` & `chatllm-2023.6.30.13.19.48/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm/webui/visualglm_st.py` & `chatllm-2023.6.30.13.19.48/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/chatllm.egg-info/PKG-INFO` & `chatllm-2023.6.30.13.19.48/chatllm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.29.9.57.33
+Version: 2023.6.30.13.19.48
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -81,14 +81,26 @@
 - 客户端：[点击下载chatbox](https://chatboxapp.xyz/)，也可接入客户端
   ![客户端](data/imgs/chatbox.png)
 
 ### [openai_keys](./data/openai_keys.md): `不定期更新免费keys`
 
 </details>
 
+## ChatMind
+
+<details markdown="1">
+  <summary>Click to ChatMind</summary>
+
+```shell
+pip install "chatllm" && chatllm-run webui --name chatmind
+```
+![客户端](data/imgs/chatmind.png)
+
+</details>
+
 ## ChatPDF
 
 <details markdown="1">
   <summary>Click to ChatPDF</summary>
 
 ```shell
 pip install "chatllm[pdf]" && chatllm-run webui --name chatpdf
```

### Comparing `chatllm-2023.6.29.9.57.33/chatllm.egg-info/SOURCES.txt` & `chatllm-2023.6.30.13.19.48/chatllm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,30 +77,33 @@
 chatllm/utils/_textsplitter.py
 chatllm/utils/common.py
 chatllm/utils/gpu_utils.py
 chatllm/utils/nbce.py
 chatllm/utils/nbce_test.py
 chatllm/webui/__init__.py
 chatllm/webui/chatbase.py
+chatllm/webui/chatmind.py
 chatllm/webui/chatpdf.py
 chatllm/webui/conf.yaml
 chatllm/webui/gradio_ui.py
 chatllm/webui/nice_ui.py
 chatllm/webui/run.sh
 chatllm/webui/visualglm_st.py
 data/openai_keys.md
 data/中职职教高考政策解读.pdf
 data/姚明.txt
+data/孙子兵法.pdf
 data/王治郅.txt
 data/科比.txt
 data/财报.pdf
 data/马保国.txt
 data/imgs/LLM.drawio.png
 data/imgs/LLM.png
 data/imgs/chatbox.png
+data/imgs/chatmind.png
 data/imgs/chatpdf.gif
 data/imgs/chatpdf_ann_df.png
 data/imgs/img.png
 data/imgs/img_1.png
 data/imgs/role.png
 data/imgs/群.png
 data/医/500种中药现代研究.txt
```

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/LLM.drawio.png` & `chatllm-2023.6.30.13.19.48/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/LLM.png` & `chatllm-2023.6.30.13.19.48/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/chatbox.png` & `chatllm-2023.6.30.13.19.48/data/imgs/chatbox.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/chatpdf.gif` & `chatllm-2023.6.30.13.19.48/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.30.13.19.48/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/img.png` & `chatllm-2023.6.30.13.19.48/data/imgs/img.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/img_1.png` & `chatllm-2023.6.30.13.19.48/data/imgs/img_1.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/imgs/role.png` & `chatllm-2023.6.30.13.19.48/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/openai_keys.md` & `chatllm-2023.6.30.13.19.48/data/openai_keys.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/医/500种中药现代研究.txt` & `chatllm-2023.6.30.13.19.48/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/医/古今医统大全.txt` & `chatllm-2023.6.30.13.19.48/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/姚明.txt` & `chatllm-2023.6.30.13.19.48/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/王治郅.txt` & `chatllm-2023.6.30.13.19.48/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/科比.txt` & `chatllm-2023.6.30.13.19.48/data/科比.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/data/财报.pdf` & `chatllm-2023.6.30.13.19.48/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/docs/Makefile` & `chatllm-2023.6.30.13.19.48/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/docs/conf.py` & `chatllm-2023.6.30.13.19.48/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/docs/make.bat` & `chatllm-2023.6.30.13.19.48/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/setup.py` & `chatllm-2023.6.30.13.19.48/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/tests/test_llm4gpt.py` & `chatllm-2023.6.30.13.19.48/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.29.9.57.33/tests/内存型.ipynb` & `chatllm-2023.6.30.13.19.48/tests/内存型.ipynb`

 * *Files identical despite different names*

