# Comparing `tmp/ailingbot-0.0.5.tar.gz` & `tmp/ailingbot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailingbot-0.0.5.tar", max compression
+gzip compressed data, was "ailingbot-0.0.6.tar", max compression
```

## Comparing `ailingbot-0.0.5.tar` & `ailingbot-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.5/LICENSE
--rw-r--r--   0        0        0    22820 2023-06-29 08:11:26.468239 ailingbot-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.5/ailingbot/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.5/ailingbot/channels/__init__.py
--rw-r--r--   0        0        0     3128 2023-06-29 06:24:43.085356 ailingbot-0.0.5/ailingbot/channels/channel.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.5/ailingbot/channels/dingtalk/__init__.py
--rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.5/ailingbot/channels/dingtalk/agent.py
--rw-r--r--   0        0        0      799 2023-06-29 04:26:54.854394 ailingbot-0.0.5/ailingbot/channels/dingtalk/render.py
--rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.5/ailingbot/channels/dingtalk/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.5/ailingbot/channels/feishu/__init__.py
--rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.5/ailingbot/channels/feishu/agent.py
--rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.5/ailingbot/channels/feishu/render.py
--rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.5/ailingbot/channels/feishu/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.5/ailingbot/channels/slack/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.5/ailingbot/channels/wechatwork/__init__.py
--rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.5/ailingbot/channels/wechatwork/agent.py
--rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.5/ailingbot/channels/wechatwork/encrypt.py
--rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.5/ailingbot/channels/wechatwork/render.py
--rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.5/ailingbot/channels/wechatwork/webhook.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.5/ailingbot/chat/__init__.py
--rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.5/ailingbot/chat/chatbot.py
--rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.5/ailingbot/chat/messages.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.5/ailingbot/chat/policies/__init__.py
--rw-r--r--   0        0        0     5436 2023-06-29 06:24:43.133890 ailingbot-0.0.5/ailingbot/chat/policies/langchain.py
--rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.5/ailingbot/chat/policy.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.5/ailingbot/cli/__init__.py
--rw-r--r--   0        0        0     9511 2023-06-29 08:06:11.693659 ailingbot-0.0.5/ailingbot/cli/cli.py
--rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.5/ailingbot/cli/options.py
--rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.5/ailingbot/cli/render.py
--rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.5/ailingbot/config.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.5/ailingbot/endpoint/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.5/ailingbot/shared/__init__.py
--rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.5/ailingbot/shared/abc.py
--rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.5/ailingbot/shared/errors.py
--rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.5/ailingbot/shared/misc.py
--rw-r--r--   0        0        0     1115 2023-06-29 08:10:51.524952 ailingbot-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    24388 1970-01-01 00:00:00.000000 ailingbot-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-13 09:39:02.779654 ailingbot-0.0.6/LICENSE
+-rw-r--r--   0        0        0    25129 2023-06-30 10:12:59.159678 ailingbot-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.021431 ailingbot-0.0.6/ailingbot/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.023123 ailingbot-0.0.6/ailingbot/channels/__init__.py
+-rw-r--r--   0        0        0     3343 2023-06-30 08:53:14.045465 ailingbot-0.0.6/ailingbot/channels/channel.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024057 ailingbot-0.0.6/ailingbot/channels/dingtalk/__init__.py
+-rw-r--r--   0        0        0     6335 2023-06-29 07:16:47.029744 ailingbot-0.0.6/ailingbot/channels/dingtalk/agent.py
+-rw-r--r--   0        0        0      799 2023-06-29 04:26:54.854394 ailingbot-0.0.6/ailingbot/channels/dingtalk/render.py
+-rw-r--r--   0        0        0     4273 2023-06-29 07:16:46.998937 ailingbot-0.0.6/ailingbot/channels/dingtalk/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024362 ailingbot-0.0.6/ailingbot/channels/feishu/__init__.py
+-rw-r--r--   0        0        0     5760 2023-06-29 04:10:57.580967 ailingbot-0.0.6/ailingbot/channels/feishu/agent.py
+-rw-r--r--   0        0        0     1398 2023-06-27 07:03:48.368295 ailingbot-0.0.6/ailingbot/channels/feishu/render.py
+-rw-r--r--   0        0        0     7052 2023-06-29 04:26:54.855074 ailingbot-0.0.6/ailingbot/channels/feishu/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024673 ailingbot-0.0.6/ailingbot/channels/slack/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-30 09:13:29.198690 ailingbot-0.0.6/ailingbot/channels/slack/agent.py
+-rw-r--r--   0        0        0     4299 2023-06-30 09:45:05.574135 ailingbot-0.0.6/ailingbot/channels/slack/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.024883 ailingbot-0.0.6/ailingbot/channels/wechatwork/__init__.py
+-rw-r--r--   0        0        0     4245 2023-06-26 06:57:43.400029 ailingbot-0.0.6/ailingbot/channels/wechatwork/agent.py
+-rw-r--r--   0        0        0     1588 2023-06-13 11:45:22.920053 ailingbot-0.0.6/ailingbot/channels/wechatwork/encrypt.py
+-rw-r--r--   0        0        0     2408 2023-06-19 04:30:43.452309 ailingbot-0.0.6/ailingbot/channels/wechatwork/render.py
+-rw-r--r--   0        0        0     5942 2023-06-26 06:57:43.400763 ailingbot-0.0.6/ailingbot/channels/wechatwork/webhook.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.027040 ailingbot-0.0.6/ailingbot/chat/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-29 05:19:20.215510 ailingbot-0.0.6/ailingbot/chat/chatbot.py
+-rw-r--r--   0        0        0     3487 2023-06-25 06:38:56.364334 ailingbot-0.0.6/ailingbot/chat/messages.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.028722 ailingbot-0.0.6/ailingbot/chat/policies/__init__.py
+-rw-r--r--   0        0        0     5436 2023-06-29 06:24:43.133890 ailingbot-0.0.6/ailingbot/chat/policies/langchain.py
+-rw-r--r--   0        0        0     1678 2023-06-25 07:39:16.611374 ailingbot-0.0.6/ailingbot/chat/policy.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.030016 ailingbot-0.0.6/ailingbot/cli/__init__.py
+-rw-r--r--   0        0        0     9511 2023-06-29 08:39:29.182555 ailingbot-0.0.6/ailingbot/cli/cli.py
+-rw-r--r--   0        0        0     1753 2023-06-21 04:13:29.688817 ailingbot-0.0.6/ailingbot/cli/options.py
+-rw-r--r--   0        0        0     5347 2023-06-18 13:01:00.251299 ailingbot-0.0.6/ailingbot/cli/render.py
+-rw-r--r--   0        0        0     1539 2023-06-20 11:18:39.452072 ailingbot-0.0.6/ailingbot/config.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.033047 ailingbot-0.0.6/ailingbot/endpoint/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:48:58.034006 ailingbot-0.0.6/ailingbot/shared/__init__.py
+-rw-r--r--   0        0        0     3953 2023-06-27 05:30:31.536603 ailingbot-0.0.6/ailingbot/shared/abc.py
+-rw-r--r--   0        0        0     1635 2023-06-14 09:09:34.338358 ailingbot-0.0.6/ailingbot/shared/errors.py
+-rw-r--r--   0        0        0      746 2023-06-13 06:48:58.036240 ailingbot-0.0.6/ailingbot/shared/misc.py
+-rw-r--r--   0        0        0     1115 2023-06-30 10:13:19.023174 ailingbot-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    26697 1970-01-01 00:00:00.000000 ailingbot-0.0.6/PKG-INFO
```

### Comparing `ailingbot-0.0.5/LICENSE` & `ailingbot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/README.md` & `ailingbot-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 
 最后我们需要去飞书的管理后台，将webhook地址配置好。
 飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/feishu/event/`
 
 完成以上配置后，就可以在飞书中找到机器人，进行对话了：
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="企业微信机器人" width="1000"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="飞书机器人" width="1000"/>
 </p>
 
 ## 接入钉钉
 
 下面演示如何快速将上面的机器人接入钉钉。
 
 ### 通过Docker
@@ -301,15 +301,97 @@
 
 最后我们需要去钉钉的管理后台，将webhook地址配置好。
 钉钉Webhook的URL为：`http(s)://你的公网IP:8080/webhook/dingtalk/event/`
 
 完成以上配置后，就可以在钉钉中找到机器人，进行对话了：
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="企业微信机器人" />
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="钉钉机器人" />
+</p>
+
+## 接入Slack
+
+下面演示如何快速将上面的机器人接入Slack，并启用文档知识问答策略。
+
+### 通过Docker
+
+```shell
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -d \
+  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
+  -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
+  -e AILINGBOT_CHANNEL__NAME=slack \
+  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的Slack App webhook verification token} \
+  -e AILINGBOT_CHANNEL__OAUTH_TOKEN={你的Slack App oauth token} \
+  -p 8080:8080
+  ailingbot poetry run ailingbot serve
+```
+
+### 通过PIP
+
+#### 安装
+
+```shell
+pip install ailingbot
+```
+
+#### 生成配置文件
+
+```shell
+ailingbot init --silence --overwrite
+```
+
+#### 修改配置文件
+
+打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+
+```toml
+[channel]
+name = "slack"
+verification_token = "" # 填写真实信息
+oauth_token = "" # 填写真实信息
+```
+
+将policy部分替换为文档问答策略：
+
+```toml
+[policy]
+name = "lc_document_qa"
+chunk_size = 1000
+chunk_overlap = 5
+```
+
+最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
+
+```toml
+[policy.llm]
+_type = "openai"
+model_name = "gpt-3.5-turbo-16k" # 这里改为gpt-3.5-turbo-16k
+openai_api_key = "" # 填写真实信息
+temperature = 0
+```
+
+#### 启动服务
+
+```shell
+ailingbot serve
+```
+
+最后我们需要去Slack的管理后台，将webhook地址配置好。
+飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/slack/event/`
+
+完成以上配置后，就可以在飞书中找到机器人，进行对话了：
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack机器人" width="1000"/>
 </p>
 
 # 📖使用指南
 
 ## 主要流程
 
 AilingBot的主要处理流程如下图：
@@ -430,15 +512,15 @@
 | 文档切重叠   | 对应LangChain Splitter的chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
 
 配置示例：
 
 ```toml
 # 使用lc_document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
 [policy]
-name = "lc_conversation"
+name = "lc_document_qa"
 chunk_size = 1000
 chunk_overlap = 0
 ```
 
 #### 模型配置
 
 模型配置与LangChain保持一致，下面给出示例。
@@ -625,15 +707,20 @@
 
 TBD
 
 ## 开发Channel
 
 TBD
 
-# 发展计划
+# 🤔常见问题
+
+- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的lc_document_qa策略
+- 各个IM的webhook需要公网IP，如果你暂时没有，可以考虑通过"内网穿透"方案在本地测试，具体方法请参考网上资料
+
+# 🎯发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
 - [ ] 支持更多的Channel
     - [x] 企业微信
     - [x] 飞书
     - [x] 钉钉
     - [ ] Slack
```

### Comparing `ailingbot-0.0.5/ailingbot/channels/channel.py` & `ailingbot-0.0.6/ailingbot/channels/channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,11 +92,17 @@
 
         elif name.lower() == 'dingtalk':
             from ailingbot.channels.dingtalk.webhook import (
                 DingtalkWebhookFactory,
             )
 
             factory = DingtalkWebhookFactory(debug=debug)
+        elif name.lower() == 'slack':
+            from ailingbot.channels.slack.webhook import (
+                SlackWebhookFactory,
+            )
+
+            factory = SlackWebhookFactory(debug=debug)
         else:
-            factory = get_class_dynamically(full_class_path)()
+            factory = get_class_dynamically(full_class_path)(debug=debug)
 
         return await factory.create_webhook_app()
```

### Comparing `ailingbot-0.0.5/ailingbot/channels/dingtalk/agent.py` & `ailingbot-0.0.6/ailingbot/channels/dingtalk/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/dingtalk/render.py` & `ailingbot-0.0.6/ailingbot/channels/dingtalk/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/dingtalk/webhook.py` & `ailingbot-0.0.6/ailingbot/channels/dingtalk/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/feishu/agent.py` & `ailingbot-0.0.6/ailingbot/channels/feishu/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/feishu/render.py` & `ailingbot-0.0.6/ailingbot/channels/feishu/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/feishu/webhook.py` & `ailingbot-0.0.6/ailingbot/channels/feishu/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/wechatwork/agent.py` & `ailingbot-0.0.6/ailingbot/channels/wechatwork/agent.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/wechatwork/encrypt.py` & `ailingbot-0.0.6/ailingbot/channels/wechatwork/encrypt.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/wechatwork/render.py` & `ailingbot-0.0.6/ailingbot/channels/wechatwork/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/channels/wechatwork/webhook.py` & `ailingbot-0.0.6/ailingbot/channels/wechatwork/webhook.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/chat/chatbot.py` & `ailingbot-0.0.6/ailingbot/chat/chatbot.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/chat/messages.py` & `ailingbot-0.0.6/ailingbot/chat/messages.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/chat/policies/langchain.py` & `ailingbot-0.0.6/ailingbot/chat/policies/langchain.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/chat/policy.py` & `ailingbot-0.0.6/ailingbot/chat/policy.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/cli/cli.py` & `ailingbot-0.0.6/ailingbot/cli/cli.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/cli/options.py` & `ailingbot-0.0.6/ailingbot/cli/options.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/cli/render.py` & `ailingbot-0.0.6/ailingbot/cli/render.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/config.py` & `ailingbot-0.0.6/ailingbot/config.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/shared/abc.py` & `ailingbot-0.0.6/ailingbot/shared/abc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/shared/errors.py` & `ailingbot-0.0.6/ailingbot/shared/errors.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/ailingbot/shared/misc.py` & `ailingbot-0.0.6/ailingbot/shared/misc.py`

 * *Files identical despite different names*

### Comparing `ailingbot-0.0.5/pyproject.toml` & `ailingbot-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ailingbot"
-version = "0.0.5"
+version = "0.0.6"
 description = "An all-in-one solution to empower your IM bot with AI."
 authors = ["ericzhang-cn <ericzhang.buaa@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `ailingbot-0.0.5/PKG-INFO` & `ailingbot-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ailingbot
-Version: 0.0.5
+Version: 0.0.6
 Summary: An all-in-one solution to empower your IM bot with AI.
 License: MIT
 Author: ericzhang-cn
 Author-email: ericzhang.buaa@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -278,15 +278,15 @@
 
 最后我们需要去飞书的管理后台，将webhook地址配置好。
 飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/feishu/event/`
 
 完成以上配置后，就可以在飞书中找到机器人，进行对话了：
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="企业微信机器人" width="1000"/>
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/feishu-screenshot.png" alt="飞书机器人" width="1000"/>
 </p>
 
 ## 接入钉钉
 
 下面演示如何快速将上面的机器人接入钉钉。
 
 ### 通过Docker
@@ -341,15 +341,97 @@
 
 最后我们需要去钉钉的管理后台，将webhook地址配置好。
 钉钉Webhook的URL为：`http(s)://你的公网IP:8080/webhook/dingtalk/event/`
 
 完成以上配置后，就可以在钉钉中找到机器人，进行对话了：
 
 <p align="center">
-    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="企业微信机器人" />
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/dingtalk-screenshot.png" alt="钉钉机器人" />
+</p>
+
+## 接入Slack
+
+下面演示如何快速将上面的机器人接入Slack，并启用文档知识问答策略。
+
+### 通过Docker
+
+```shell
+git clone https://github.com/ericzhang-cn/ailingbot.git ailingbot
+cd ailingbot
+docker build -t ailingbot .
+docker run -d \
+  -e AILINGBOT_POLICY__NAME=lc_document_qa \
+  -e AILINGBOT_POLICY__CHUNK_SIZE=1000 \
+  -e AILINGBOT_POLICY__CHUNK_OVERLAP=0 \
+  -e AILINGBOT_POLICY__LLM__OPENAI_API_KEY={你的OpenAI API key} \
+  -e AILINGBOT_POLICY__LLM__MODEL_NAME=gpt-3.5-turbo-16k \
+  -e AILINGBOT_CHANNEL__NAME=slack \
+  -e AILINGBOT_CHANNEL__VERIFICATION_TOKEN={你的Slack App webhook verification token} \
+  -e AILINGBOT_CHANNEL__OAUTH_TOKEN={你的Slack App oauth token} \
+  -p 8080:8080
+  ailingbot poetry run ailingbot serve
+```
+
+### 通过PIP
+
+#### 安装
+
+```shell
+pip install ailingbot
+```
+
+#### 生成配置文件
+
+```shell
+ailingbot init --silence --overwrite
+```
+
+#### 修改配置文件
+
+打开`settings.toml`，将其中的channel部分改为如下，并填入你的飞书真实信息：
+
+```toml
+[channel]
+name = "slack"
+verification_token = "" # 填写真实信息
+oauth_token = "" # 填写真实信息
+```
+
+将policy部分替换为文档问答策略：
+
+```toml
+[policy]
+name = "lc_document_qa"
+chunk_size = 1000
+chunk_overlap = 5
+```
+
+最后建议在使用文档问答策略时，使用16k模型，因此将`policy.llm.model_name`修改为如下配置：
+
+```toml
+[policy.llm]
+_type = "openai"
+model_name = "gpt-3.5-turbo-16k" # 这里改为gpt-3.5-turbo-16k
+openai_api_key = "" # 填写真实信息
+temperature = 0
+```
+
+#### 启动服务
+
+```shell
+ailingbot serve
+```
+
+最后我们需要去Slack的管理后台，将webhook地址配置好。
+飞书Webhook的URL为：`http(s)://你的公网IP:8080/webhook/slack/event/`
+
+完成以上配置后，就可以在飞书中找到机器人，进行对话了：
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/ericzhang-cn/ailingbot/main/img/slack-screenshot.png" alt="Slack机器人" width="1000"/>
 </p>
 
 # 📖使用指南
 
 ## 主要流程
 
 AilingBot的主要处理流程如下图：
@@ -470,15 +552,15 @@
 | 文档切重叠   | 对应LangChain Splitter的chunk_overlap | policy.chunk_overlap | AILINGBOT_POLICY__CHUNK_OVERLAP |
 
 配置示例：
 
 ```toml
 # 使用lc_document_qa策略，chunk_size和chunk_overlap分别配置为1000和0
 [policy]
-name = "lc_conversation"
+name = "lc_document_qa"
 chunk_size = 1000
 chunk_overlap = 0
 ```
 
 #### 模型配置
 
 模型配置与LangChain保持一致，下面给出示例。
@@ -665,15 +747,20 @@
 
 TBD
 
 ## 开发Channel
 
 TBD
 
-# 发展计划
+# 🤔常见问题
+
+- 由于企业微信不支持上传文件事件的回调，因此企业微信暂时不能使用内置的lc_document_qa策略
+- 各个IM的webhook需要公网IP，如果你暂时没有，可以考虑通过"内网穿透"方案在本地测试，具体方法请参考网上资料
+
+# 🎯发展计划
 
 - [ ] 提供完善的使用文档和开发者文档
 - [ ] 支持更多的Channel
     - [x] 企业微信
     - [x] 飞书
     - [x] 钉钉
     - [ ] Slack
```

