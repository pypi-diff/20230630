# Comparing `tmp/chatllm-2023.6.30.13.19.48.tar.gz` & `tmp/chatllm-2023.6.30.20.15.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatllm-2023.6.30.13.19.48.tar", last modified: Fri Jun 30 05:19:48 2023, max compression
+gzip compressed data, was "chatllm-2023.6.30.20.15.36.tar", last modified: Fri Jun 30 12:15:37 2023, max compression
```

## Comparing `chatllm-2023.6.30.13.19.48.tar` & `chatllm-2023.6.30.20.15.36.tar`

### file list

```diff
@@ -1,142 +1,153 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.846708 chatllm-2023.6.30.13.19.48/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.30.13.19.48/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      733 2023-06-29 01:47:04.000000 chatllm-2023.6.30.13.19.48/LLMS.md
--rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.30.13.19.48/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     6909 2023-06-30 05:19:48.846520 chatllm-2023.6.30.13.19.48/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     6178 2023-06-29 08:10:09.000000 chatllm-2023.6.30.13.19.48/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.30.13.19.48/README.md.bak
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-27 09:07:59.000000 chatllm-2023.6.30.13.19.48/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.791191 chatllm-2023.6.30.13.19.48/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.793374 chatllm-2023.6.30.13.19.48/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.30.13.19.48/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.793923 chatllm-2023.6.30.13.19.48/chatllm/aigc/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.30.13.19.48/chatllm/aigc/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.30.13.19.48/chatllm/aigc/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.796232 chatllm-2023.6.30.13.19.48/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.30.13.19.48/chatllm/api/TODO.md
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.30.13.19.48/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      659 2023-06-02 12:12:32.000000 chatllm-2023.6.30.13.19.48/chatllm/api/app.py
--rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2023.6.30.13.19.48/chatllm/api/config.py
--rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.30.13.19.48/chatllm/api/datamodels.py
--rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.30.13.19.48/chatllm/api/openai_client.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.797702 chatllm-2023.6.30.13.19.48/chatllm/api/routes/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/api.py
--rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     4928 2023-06-04 07:21:05.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/completions.py
--rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/embeddings.py
--rw-r--r--   0 betterme   (501) staff       (20)     3422 2023-06-26 05:20:07.000000 chatllm-2023.6.30.13.19.48/chatllm/api/routes/responses.py
--rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.30.13.19.48/chatllm/api/sse_api.py
--rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.30.13.19.48/chatllm/api/test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.801821 chatllm-2023.6.30.13.19.48/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/__chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.30.13.19.48/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.30.13.19.48/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.802341 chatllm-2023.6.30.13.19.48/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1087 2023-06-15 09:17:56.000000 chatllm-2023.6.30.13.19.48/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.30.13.19.48/chatllm/closeai.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.30.13.19.48/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.803753 chatllm-2023.6.30.13.19.48/chatllm/llms/
--rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2305 2023-06-29 01:00:10.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/chatglm.py
--rw-r--r--   0 betterme   (501) staff       (20)     1323 2023-06-29 02:49:42.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/chatgpt.py
--rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.30.13.19.48/chatllm/llms/llama.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.804255 chatllm-2023.6.30.13.19.48/chatllm/prompts/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2023.6.30.13.19.48/chatllm/prompts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-20 08:01:27.000000 chatllm-2023.6.30.13.19.48/chatllm/prompts/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.805662 chatllm-2023.6.30.13.19.48/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-06-02 10:18:35.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/gpu_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/nbce.py
--rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.30.13.19.48/chatllm/utils/nbce_test.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.808688 chatllm-2023.6.30.13.19.48/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/conf.yaml
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      221 2023-06-29 07:28:40.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/run.sh
--rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.30.13.19.48/chatllm/webui/visualglm_st.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.792404 chatllm-2023.6.30.13.19.48/chatllm.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     6909 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2837 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-30 05:19:48.000000 chatllm-2023.6.30.13.19.48/chatllm.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.815876 chatllm-2023.6.30.13.19.48/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.827421 chatllm-2023.6.30.13.19.48/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.30.13.19.48/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.30.13.19.48/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatbox.png
--rw-r--r--   0 betterme   (501) staff       (20)   141276 2023-06-29 08:09:29.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatmind.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.30.13.19.48/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.30.13.19.48/data/imgs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.30.13.19.48/data/imgs/img_1.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.30.13.19.48/data/imgs/role.png
--rw-r--r--   0 betterme   (501) staff       (20)     9900 2023-06-30 05:19:08.000000 chatllm-2023.6.30.13.19.48/data/imgs/群.png
--rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.30.13.19.48/data/openai_keys.md
--rw-r--r--   0 betterme   (501) staff       (20)   678357 2023-06-29 02:05:32.000000 chatllm-2023.6.30.13.19.48/data/中职职教高考政策解读.pdf
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.831174 chatllm-2023.6.30.13.19.48/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.30.13.19.48/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.30.13.19.48/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)   606941 2023-06-29 02:21:44.000000 chatllm-2023.6.30.13.19.48/data/孙子兵法.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.30.13.19.48/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.30.13.19.48/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.845081 chatllm-2023.6.30.13.19.48/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      342 2023-06-29 08:04:00.000000 chatllm-2023.6.30.13.19.48/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.30.13.19.48/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.30.13.19.48/requirements_ann.txt
--rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.30.13.19.48/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.30.13.19.48/requirements_openai.txt
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.30.13.19.48/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.30.13.19.48/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-30 05:19:48.846760 chatllm-2023.6.30.13.19.48/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-06-20 06:25:34.000000 chatllm-2023.6.30.13.19.48/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 05:19:48.845770 chatllm-2023.6.30.13.19.48/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.30.13.19.48/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.30.13.19.48/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.336650 chatllm-2023.6.30.20.15.36/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 chatllm-2023.6.30.20.15.36/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      733 2023-06-29 01:47:04.000000 chatllm-2023.6.30.20.15.36/LLMS.md
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-05-31 08:06:48.000000 chatllm-2023.6.30.20.15.36/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     6974 2023-06-30 12:15:37.336402 chatllm-2023.6.30.20.15.36/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     6243 2023-06-30 05:23:26.000000 chatllm-2023.6.30.20.15.36/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     5851 2023-05-29 06:46:23.000000 chatllm-2023.6.30.20.15.36/README.md.bak
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-27 09:07:59.000000 chatllm-2023.6.30.20.15.36/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.281053 chatllm-2023.6.30.20.15.36/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.282935 chatllm-2023.6.30.20.15.36/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 chatllm-2023.6.30.20.15.36/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 chatllm-2023.6.30.20.15.36/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 chatllm-2023.6.30.20.15.36/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 chatllm-2023.6.30.20.15.36/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.283414 chatllm-2023.6.30.20.15.36/chatllm/aigc/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-05-29 05:16:39.000000 chatllm-2023.6.30.20.15.36/chatllm/aigc/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      834 2023-05-29 05:17:00.000000 chatllm-2023.6.30.20.15.36/chatllm/aigc/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.285674 chatllm-2023.6.30.20.15.36/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-05-29 01:42:28.000000 chatllm-2023.6.30.20.15.36/chatllm/api/TODO.md
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 chatllm-2023.6.30.20.15.36/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      659 2023-06-02 12:12:32.000000 chatllm-2023.6.30.20.15.36/chatllm/api/app.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2192 2023-06-26 05:53:59.000000 chatllm-2023.6.30.20.15.36/chatllm/api/config.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1010 2023-05-31 00:47:03.000000 chatllm-2023.6.30.20.15.36/chatllm/api/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1749 2023-05-31 00:30:21.000000 chatllm-2023.6.30.20.15.36/chatllm/api/openai_client.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.287176 chatllm-2023.6.30.20.15.36/chatllm/api/routes/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      557 2023-05-29 01:39:47.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/api.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2200 2023-06-02 01:06:14.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5016 2023-06-30 12:15:34.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/completions.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1904 2023-06-04 06:52:41.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3301 2023-06-30 12:15:34.000000 chatllm-2023.6.30.20.15.36/chatllm/api/routes/responses.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11497 2023-05-25 09:59:48.000000 chatllm-2023.6.30.20.15.36/chatllm/api/sse_api.py
+-rw-r--r--   0 betterme   (501) staff       (20)      845 2023-05-26 07:01:26.000000 chatllm-2023.6.30.20.15.36/chatllm/api/test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.291020 chatllm-2023.6.30.20.15.36/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3937 2023-05-29 07:27:53.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/__chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2405 2023-06-27 08:56:59.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2420 2023-06-29 01:53:20.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)      944 2023-05-29 04:11:25.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1693 2023-06-29 07:30:13.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1350 2023-05-29 07:27:53.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1875 2023-05-25 06:54:08.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 chatllm-2023.6.30.20.15.36/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 chatllm-2023.6.30.20.15.36/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.291587 chatllm-2023.6.30.20.15.36/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1087 2023-06-15 09:17:56.000000 chatllm-2023.6.30.20.15.36/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      779 2023-05-25 08:42:08.000000 chatllm-2023.6.30.20.15.36/chatllm/closeai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 chatllm-2023.6.30.20.15.36/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.292777 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2023-06-30 09:18:14.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/Embeddings.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-06-30 09:14:59.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/LLMChat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      467 2023-06-30 10:31:04.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/Loader.py
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-06-30 08:37:28.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      474 2023-06-30 10:29:50.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/datamodels.py
+-rw-r--r--   0 betterme   (501) staff       (20)      420 2023-06-30 09:28:35.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.293016 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/document_loaders/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-06-30 11:05:38.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/document_loaders/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2101 2023-06-30 12:01:08.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/document_loaders/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      272 2023-06-30 10:14:54.000000 chatllm-2023.6.30.20.15.36/chatllm/langchain_mini/text_splitter.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.294216 chatllm-2023.6.30.20.15.36/chatllm/llms/
+-rw-r--r--   0 betterme   (501) staff       (20)     1526 2023-06-02 12:11:10.000000 chatllm-2023.6.30.20.15.36/chatllm/llms/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2305 2023-06-29 01:00:10.000000 chatllm-2023.6.30.20.15.36/chatllm/llms/chatglm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1323 2023-06-29 02:49:42.000000 chatllm-2023.6.30.20.15.36/chatllm/llms/chatgpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1559 2023-05-22 08:19:27.000000 chatllm-2023.6.30.20.15.36/chatllm/llms/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2083 2023-05-22 08:39:00.000000 chatllm-2023.6.30.20.15.36/chatllm/llms/llama.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.294722 chatllm-2023.6.30.20.15.36/chatllm/prompts/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-06-12 03:51:17.000000 chatllm-2023.6.30.20.15.36/chatllm/prompts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-06-20 08:01:27.000000 chatllm-2023.6.30.20.15.36/chatllm/prompts/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.296165 chatllm-2023.6.30.20.15.36/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-06-02 10:18:35.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2430 2023-05-19 09:28:43.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/gpu_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6342 2023-05-30 08:31:55.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/nbce.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5208 2023-05-30 08:22:36.000000 chatllm-2023.6.30.20.15.36/chatllm/utils/nbce_test.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.298768 chatllm-2023.6.30.20.15.36/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1457 2023-05-29 07:27:53.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-06-29 07:59:43.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3102 2023-06-01 03:54:54.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      134 2023-06-26 02:13:58.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/conf.yaml
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      221 2023-06-29 07:28:40.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/run.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     3506 2023-05-26 07:39:23.000000 chatllm-2023.6.30.20.15.36/chatllm/webui/visualglm_st.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.282096 chatllm-2023.6.30.20.15.36/chatllm.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     6974 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     3183 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-06-30 12:15:37.000000 chatllm-2023.6.30.20.15.36/chatllm.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.305550 chatllm-2023.6.30.20.15.36/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.319272 chatllm-2023.6.30.20.15.36/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 chatllm-2023.6.30.20.15.36/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 chatllm-2023.6.30.20.15.36/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)    80933 2023-05-31 01:13:52.000000 chatllm-2023.6.30.20.15.36/data/imgs/chatbox.png
+-rw-r--r--   0 betterme   (501) staff       (20)   141276 2023-06-29 08:09:29.000000 chatllm-2023.6.30.20.15.36/data/imgs/chatmind.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 chatllm-2023.6.30.20.15.36/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 chatllm-2023.6.30.20.15.36/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)   477462 2023-05-08 01:03:47.000000 chatllm-2023.6.30.20.15.36/data/imgs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)   333086 2023-05-08 01:03:52.000000 chatllm-2023.6.30.20.15.36/data/imgs/img_1.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 chatllm-2023.6.30.20.15.36/data/imgs/role.png
+-rw-r--r--   0 betterme   (501) staff       (20)     9900 2023-06-30 05:19:08.000000 chatllm-2023.6.30.20.15.36/data/imgs/群.png
+-rw-r--r--   0 betterme   (501) staff       (20)    31192 2023-05-29 00:57:03.000000 chatllm-2023.6.30.20.15.36/data/openai_keys.md
+-rw-r--r--   0 betterme   (501) staff       (20)   678357 2023-06-29 02:05:32.000000 chatllm-2023.6.30.20.15.36/data/中职职教高考政策解读.pdf
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.322967 chatllm-2023.6.30.20.15.36/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 chatllm-2023.6.30.20.15.36/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 chatllm-2023.6.30.20.15.36/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 chatllm-2023.6.30.20.15.36/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)   606941 2023-06-29 02:21:44.000000 chatllm-2023.6.30.20.15.36/data/孙子兵法.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 chatllm-2023.6.30.20.15.36/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 chatllm-2023.6.30.20.15.36/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 chatllm-2023.6.30.20.15.36/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 chatllm-2023.6.30.20.15.36/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.333563 chatllm-2023.6.30.20.15.36/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      342 2023-06-29 08:04:00.000000 chatllm-2023.6.30.20.15.36/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       90 2023-05-26 09:35:58.000000 chatllm-2023.6.30.20.15.36/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-05-19 09:53:16.000000 chatllm-2023.6.30.20.15.36/requirements_ann.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       30 2023-05-31 02:41:18.000000 chatllm-2023.6.30.20.15.36/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       29 2023-05-26 08:03:09.000000 chatllm-2023.6.30.20.15.36/requirements_openai.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-05-29 04:24:55.000000 chatllm-2023.6.30.20.15.36/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-05-29 04:24:55.000000 chatllm-2023.6.30.20.15.36/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-06-30 12:15:37.336699 chatllm-2023.6.30.20.15.36/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1706 2023-06-20 06:25:34.000000 chatllm-2023.6.30.20.15.36/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-06-30 12:15:37.334056 chatllm-2023.6.30.20.15.36/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 chatllm-2023.6.30.20.15.36/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 chatllm-2023.6.30.20.15.36/tox.ini
```

### Comparing `chatllm-2023.6.30.13.19.48/.gitignore` & `chatllm-2023.6.30.20.15.36/.gitignore`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/.travis.yml` & `chatllm-2023.6.30.20.15.36/.travis.yml`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/LICENSE` & `chatllm-2023.6.30.20.15.36/LICENSE`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/LLMS.md` & `chatllm-2023.6.30.20.15.36/LLMS.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/Makefile` & `chatllm-2023.6.30.20.15.36/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/PKG-INFO` & `chatllm-2023.6.30.20.15.36/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.30.13.19.48
+Version: 2023.6.30.20.15.36
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -89,14 +89,15 @@
 
 <details markdown="1">
   <summary>Click to ChatMind</summary>
 
 ```shell
 pip install "chatllm" && chatllm-run webui --name chatmind
 ```
+
 ![客户端](data/imgs/chatmind.png)
 
 </details>
 
 ## ChatPDF
 
 <details markdown="1">
@@ -130,15 +131,15 @@
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
   | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-        | -------------- | ------------------------- | --------------------------------- |
+          | -------------- | ------------------------- | --------------------------------- |
   | FP16（无量化） | 13 GB                     | 14 GB                             |
   | INT8           | 8 GB                     | 9 GB                             |
   | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
     - [安装指南](docs/INSTALL.md)
@@ -198,17 +199,17 @@
 - [ ] 增加 API 支持
     - [x] 利用 Fastapi/Flask/Grpc
       实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
     - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
-## 交流群
+## [交流群](http://wechat.yanyue.cloud/common/qun/redirect/?qid=449187)
 
 <div align=center>
-<img src="data/imgs/群.png" alt="群" width="250" height="400">
+<img src="data/imgs/群.png" alt="群" width="200" height="200">
 </div>
 
 > 若二维码失效加微信拉群 313303303
```

### Comparing `chatllm-2023.6.30.13.19.48/README.md` & `chatllm-2023.6.30.20.15.36/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 
 <details markdown="1">
   <summary>Click to ChatMind</summary>
 
 ```shell
 pip install "chatllm" && chatllm-run webui --name chatmind
 ```
+
 ![客户端](data/imgs/chatmind.png)
 
 </details>
 
 ## ChatPDF
 
 <details markdown="1">
@@ -105,15 +106,15 @@
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
   | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-        | -------------- | ------------------------- | --------------------------------- |
+          | -------------- | ------------------------- | --------------------------------- |
   | FP16（无量化） | 13 GB                     | 14 GB                             |
   | INT8           | 8 GB                     | 9 GB                             |
   | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
     - [安装指南](docs/INSTALL.md)
@@ -173,17 +174,17 @@
 - [ ] 增加 API 支持
     - [x] 利用 Fastapi/Flask/Grpc
       实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
     - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
-## 交流群
+## [交流群](http://wechat.yanyue.cloud/common/qun/redirect/?qid=449187)
 
 <div align=center>
-<img src="data/imgs/群.png" alt="群" width="250" height="400">
+<img src="data/imgs/群.png" alt="群" width="200" height="200">
 </div>
 
 > 若二维码失效加微信拉群 313303303
```

### Comparing `chatllm-2023.6.30.13.19.48/README.md.bak` & `chatllm-2023.6.30.20.15.36/README.md.bak`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/TODO.md` & `chatllm-2023.6.30.20.15.36/TODO.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/_his/FaissANN.py` & `chatllm-2023.6.30.20.15.36/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/_his/_chatllm.py` & `chatllm-2023.6.30.20.15.36/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/_his/_qa.py` & `chatllm-2023.6.30.20.15.36/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/aigc/common.py` & `chatllm-2023.6.30.20.15.36/chatllm/aigc/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/app.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/app.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/config.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/config.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/datamodels.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/datamodels.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/openai_client.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/openai_client.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/routes/api.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/routes/api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/routes/base.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/routes/base.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/routes/completions.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/routes/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 router = APIRouter()
 
 
 @router.post("/v1/chat/completions")
 async def chat_completions(body: ChatBody, request: Request, background_tasks: BackgroundTasks):
     background_tasks.add_task(torch_gc)
+    _id = uuid.uuid1()
 
     if request.headers.get("Authorization").split(" ")[1] not in tokens:
         raise HTTPException(status.HTTP_401_UNAUTHORIZED, "Token is wrong!")
 
     # if not llm_model: # 空模型
     #     raise HTTPException(status.HTTP_404_NOT_FOUND, "LLM model not found!")
 
@@ -60,45 +61,47 @@
         async def eval_llm():
             first = True
             response = ''  # 方便入库
             for _response in do_chat(question, history=history, **chat_kwargs):
                 response += _response
                 if first:
                     first = False
-                    yield json.dumps(generate_stream_response_start(), ensure_ascii=False)
-                _ = generate_stream_response(_response)
+                    yield json.dumps(generate_stream_response_start(_id), ensure_ascii=False)
+                _ = generate_stream_response(_id, _response)
                 yield json.dumps(_, ensure_ascii=False)
 
-            yield json.dumps(generate_stream_response_stop(), ensure_ascii=False)
+            yield json.dumps(generate_stream_response_stop(_id), ensure_ascii=False)
             yield "[DONE]"
 
-            content = generate_response(response)
+            content = generate_response(_id, response)
             content['user'] = body.user
             rprint(content)
             background_tasks.add_task(do_db, pd.DataFrame([content]), 'chatcmpl')
 
             if debug: logger.success(content)  # 日志
 
         return EventSourceResponse(eval_llm(), ping=10000)
     else:
         response = ''.join(do_chat(question, history=history, **chat_kwargs))
 
-        content = generate_response(response)
+        content = generate_response(_id, response)
         content['user'] = body.user
         background_tasks.add_task(do_db, pd.DataFrame([content]), 'chatcmpl')
 
         if debug: logger.success(content)  # 日志
 
         return JSONResponse(content)
 
 
 @router.post("/v1/completions")
 async def completions(body: CompletionBody, request: Request, background_tasks: BackgroundTasks):
     background_tasks.add_task(torch_gc)
 
+    _id = uuid.uuid1()
+
     if request.headers.get("Authorization").split(" ")[1] not in tokens:
         raise HTTPException(status.HTTP_401_UNAUTHORIZED, "Token is wrong!")
 
     # if not llm_model: # 空模型
     #     raise HTTPException(status.HTTP_404_NOT_FOUND, "LLM model not found!")
 
     question = body.prompt
@@ -109,30 +112,30 @@
         rprint('ChatBody:', body.dict())
 
     if body.stream:
         async def eval_llm():
             response = ''  # 方便入库
             for _response in do_chat(question, **chat_kwargs):
                 response += _response
-                _ = generate_stream_response(_response, chat=False)
+                _ = generate_stream_response(_id, _response, chat=False)
                 yield json.dumps(_, ensure_ascii=False)
 
-            yield json.dumps(generate_stream_response_stop(chat=False), ensure_ascii=False)
+            yield json.dumps(generate_stream_response_stop(_id, chat=False), ensure_ascii=False)
             yield "[DONE]"
 
-            content = generate_response(response, chat=False)
+            content = generate_response(_id, response, chat=False)
             content['user'] = body.user
             background_tasks.add_task(do_db, pd.DataFrame([content]), 'cmpl')
 
             if debug: logger.success(content)  # 日志
 
         return EventSourceResponse(eval_llm(), ping=10000)
     else:
         response = ''.join(do_chat(question, **chat_kwargs))  # 流式合成
 
-        content = generate_response(response, chat=False)
+        content = generate_response(_id, response, chat=False)
         content['user'] = body.user
         background_tasks.add_task(do_db, pd.DataFrame([content]), 'cmpl')
 
         if debug: logger.success(content)  # 日志
 
         return JSONResponse(content)
```

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/routes/embeddings.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/routes/responses.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/routes/responses.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 
 from meutils.pipe import *
 
 
-def generate_response(content: str, chat: bool = True):
+def generate_response(id, content: str, chat: bool = True):
     # 客户端会更新这些值
-    _id = uuid.uuid1()  # 内容id
     _time = int(time.time())
 
     if chat:
         return {
-            "id": f"chatcmpl-{_id}",
+            "id": f"chatcmpl-{id}",
             "object": "chat.completion",
             "created": _time,
             "model": "gpt-3.5-turbo-0301",
             "usage": {
                 "prompt_tokens": 0,
                 "completion_tokens": 0,
                 "total_tokens": 0,
@@ -30,15 +29,15 @@
             "choices": [{
                 "message": {"role": "assistant", "content": content},
                 "finish_reason": "stop", "index": 0}
             ]
         }
     else:
         return {
-            "id": f"cmpl-{_id}",
+            "id": f"cmpl-{id}",
             "object": "text_completion",
             "created": _time,
             "model": "text-davinci-003",
             "choices": [
                 {
                     "text": content,
                     "index": 0,
@@ -50,70 +49,68 @@
                 "prompt_tokens": 0,
                 "completion_tokens": 0,
                 "total_tokens": 0
             }
         }
 
 
-def generate_stream_response_start():
+def generate_stream_response_start(id):
     _time = int(time.time())
 
     return {
-        "id": "chatcmpl-77QWpn5cxFi9sVMw56DZReDiGKmcB",
+        "id": f"chatcmpl-{id}",
         "object": "chat.completion.chunk",
         "created": _time,
         "model": "gpt-3.5-turbo-0301",
         "choices": [{"delta": {"role": "assistant"}, "index": 0, "finish_reason": None}]
     }
 
 
-def generate_stream_response(content: str, chat: bool = True):
-    _id = uuid.uuid1()  # 内容id
+def generate_stream_response(id, content: str, chat: bool = True):
     _time = int(time.time())
 
     if chat:
         return {
-            "id": f"chatcmpl-{_id}",  # TODO
+            "id": f"chatcmpl-{id}",  # TODO
             "object": "chat.completion.chunk",
             "created": _time,
             "model": "gpt-3.5-turbo-0301",
             "choices": [{"delta": {"content": content}, "index": 0, "finish_reason": None}]
         }
     else:
         return {
-            "id": f"cmpl-{_id}",
+            "id": f"cmpl-{id}",
             "object": "text_completion",
             "created": _time,
             "choices": [
                 {
                     "text": content,
                     "index": 0,
                     "logprobs": None,
                     "finish_reason": None,
                 }
             ],
             "model": "text-davinci-003"
         }
 
 
-def generate_stream_response_stop(chat: bool = True):
-    _id = uuid.uuid1()  # 内容id
+def generate_stream_response_stop(id, chat: bool = True):
     _time = int(time.time())
 
     if chat:
         return {
-            "id": f"chatcmpl-{_id}",
+            "id": f"chatcmpl-{id}",
             "object": "chat.completion.chunk",
             "created": _time,
             "model": "gpt-3.5-turbo-0301",
             "choices": [{"delta": {}, "index": 0, "finish_reason": "stop"}]
         }
     else:
         return {
-            "id": f"cmpl-{_id}",
+            "id": f"cmpl-{id}",
             "object": "text_completion",
             "created": _time,
             "choices": [
                 {"text": "", "index": 0, "logprobs": None, "finish_reason": "stop"}],
             "model": "text-davinci-003",
         }
```

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/sse_api.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/sse_api.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/api/test.py` & `chatllm-2023.6.30.20.15.36/chatllm/api/test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/Question2Answer.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/__chatbase.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/__chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatann.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatbase.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatcrawler.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatmind.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatpdf.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/applications/chatwhoosh.py` & `chatllm-2023.6.30.20.15.36/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/chatyuan.py` & `chatllm-2023.6.30.20.15.36/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/clis/cli.py` & `chatllm-2023.6.30.20.15.36/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/closeai.py` & `chatllm-2023.6.30.20.15.36/chatllm/closeai.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/embedding.py` & `chatllm-2023.6.30.20.15.36/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/llms/__init__.py` & `chatllm-2023.6.30.20.15.36/chatllm/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/llms/chatglm.py` & `chatllm-2023.6.30.20.15.36/chatllm/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/llms/chatgpt.py` & `chatllm-2023.6.30.20.15.36/chatllm/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/llms/demo.py` & `chatllm-2023.6.30.20.15.36/chatllm/llms/demo.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/llms/llama.py` & `chatllm-2023.6.30.20.15.36/chatllm/llms/llama.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/prompts/common.py` & `chatllm-2023.6.30.20.15.36/chatllm/prompts/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/utils/common.py` & `chatllm-2023.6.30.20.15.36/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/utils/gpu_utils.py` & `chatllm-2023.6.30.20.15.36/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/utils/nbce.py` & `chatllm-2023.6.30.20.15.36/chatllm/utils/nbce.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/utils/nbce_test.py` & `chatllm-2023.6.30.20.15.36/chatllm/utils/nbce_test.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/chatbase.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/chatmind.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/chatmind.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/chatpdf.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/gradio_ui.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/nice_ui.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm/webui/visualglm_st.py` & `chatllm-2023.6.30.20.15.36/chatllm/webui/visualglm_st.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/chatllm.egg-info/PKG-INFO` & `chatllm-2023.6.30.20.15.36/chatllm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatllm
-Version: 2023.6.30.13.19.48
+Version: 2023.6.30.20.15.36
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -89,14 +89,15 @@
 
 <details markdown="1">
   <summary>Click to ChatMind</summary>
 
 ```shell
 pip install "chatllm" && chatllm-run webui --name chatmind
 ```
+
 ![客户端](data/imgs/chatmind.png)
 
 </details>
 
 ## ChatPDF
 
 <details markdown="1">
@@ -130,15 +131,15 @@
 
 <details markdown="1">
   <summary>Click to Deploy</summary>
 
 - ChatGLM-6B 模型硬件需求
 
   | **量化等级**   | **最低 GPU 显存**（推理） | **最低 GPU 显存**（高效参数微调） |
-        | -------------- | ------------------------- | --------------------------------- |
+          | -------------- | ------------------------- | --------------------------------- |
   | FP16（无量化） | 13 GB                     | 14 GB                             |
   | INT8           | 8 GB                     | 9 GB                             |
   | INT4           | 6 GB                      | 7 GB                              |
 
 
 - 从本地加载模型
     - [安装指南](docs/INSTALL.md)
@@ -198,17 +199,17 @@
 - [ ] 增加 API 支持
     - [x] 利用 Fastapi/Flask/Grpc
       实现流式接口 `chatllm-run openai <本地模型地址> --host 127.0.0.1 --port 8000`
     - [ ] 前后端分离，实现调用 API 的 Web UI Demo
 
 </details>
 
-## 交流群
+## [交流群](http://wechat.yanyue.cloud/common/qun/redirect/?qid=449187)
 
 <div align=center>
-<img src="data/imgs/群.png" alt="群" width="250" height="400">
+<img src="data/imgs/群.png" alt="群" width="200" height="200">
 </div>
 
 > 若二维码失效加微信拉群 313303303
```

### Comparing `chatllm-2023.6.30.13.19.48/chatllm.egg-info/SOURCES.txt` & `chatllm-2023.6.30.20.15.36/chatllm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -62,14 +62,23 @@
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
 chatllm/applications/chatwhoosh.py
 chatllm/applications/pipeline.py
 chatllm/clis/README.md
 chatllm/clis/__init__.py
 chatllm/clis/cli.py
+chatllm/langchain_mini/Embeddings.py
+chatllm/langchain_mini/LLMChat.py
+chatllm/langchain_mini/Loader.py
+chatllm/langchain_mini/__init__.py
+chatllm/langchain_mini/datamodels.py
+chatllm/langchain_mini/demo.py
+chatllm/langchain_mini/text_splitter.py
+chatllm/langchain_mini/document_loaders/__init__.py
+chatllm/langchain_mini/document_loaders/pdf.py
 chatllm/llms/__init__.py
 chatllm/llms/chatglm.py
 chatllm/llms/chatgpt.py
 chatllm/llms/demo.py
 chatllm/llms/llama.py
 chatllm/prompts/__init__.py
 chatllm/prompts/common.py
```

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/LLM.drawio.png` & `chatllm-2023.6.30.20.15.36/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/LLM.png` & `chatllm-2023.6.30.20.15.36/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/chatbox.png` & `chatllm-2023.6.30.20.15.36/data/imgs/chatbox.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/chatmind.png` & `chatllm-2023.6.30.20.15.36/data/imgs/chatmind.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/chatpdf.gif` & `chatllm-2023.6.30.20.15.36/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/chatpdf_ann_df.png` & `chatllm-2023.6.30.20.15.36/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/img.png` & `chatllm-2023.6.30.20.15.36/data/imgs/img.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/img_1.png` & `chatllm-2023.6.30.20.15.36/data/imgs/img_1.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/role.png` & `chatllm-2023.6.30.20.15.36/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/imgs/群.png` & `chatllm-2023.6.30.20.15.36/data/imgs/群.png`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/openai_keys.md` & `chatllm-2023.6.30.20.15.36/data/openai_keys.md`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/中职职教高考政策解读.pdf` & `chatllm-2023.6.30.20.15.36/data/中职职教高考政策解读.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/医/500种中药现代研究.txt` & `chatllm-2023.6.30.20.15.36/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/医/古今医统大全.txt` & `chatllm-2023.6.30.20.15.36/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/姚明.txt` & `chatllm-2023.6.30.20.15.36/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/孙子兵法.pdf` & `chatllm-2023.6.30.20.15.36/data/孙子兵法.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/王治郅.txt` & `chatllm-2023.6.30.20.15.36/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/科比.txt` & `chatllm-2023.6.30.20.15.36/data/科比.txt`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/data/财报.pdf` & `chatllm-2023.6.30.20.15.36/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/docs/Makefile` & `chatllm-2023.6.30.20.15.36/docs/Makefile`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/docs/conf.py` & `chatllm-2023.6.30.20.15.36/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/docs/make.bat` & `chatllm-2023.6.30.20.15.36/docs/make.bat`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/setup.py` & `chatllm-2023.6.30.20.15.36/setup.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/tests/test_llm4gpt.py` & `chatllm-2023.6.30.20.15.36/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `chatllm-2023.6.30.13.19.48/tests/内存型.ipynb` & `chatllm-2023.6.30.20.15.36/tests/内存型.ipynb`

 * *Files identical despite different names*

