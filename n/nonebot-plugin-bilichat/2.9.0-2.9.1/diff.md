# Comparing `tmp/nonebot_plugin_bilichat-2.9.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.9.0.tar", last modified: Sun Jun 25 07:30:29 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.9.1.tar", last modified: Thu Jun 29 15:32:05 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.9.0.tar` & `nonebot_plugin_bilichat-2.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    34523 2023-06-25 07:30:21.054542 nonebot_plugin_bilichat-2.9.0/LICENSE
--rw-r--r--   0        0        0    12710 2023-06-25 07:30:21.054542 nonebot_plugin_bilichat-2.9.0/README.md
--rw-r--r--   0        0        0     9690 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     6614 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      844 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      871 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6502 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    16355 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     2773 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0     3638 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-25 07:30:21.074543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1187 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7534 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     2098 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    27644 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/newbing.png
--rw-r--r--   0        0        0    59199 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     1403 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0    24930 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing.py
--rw-r--r--   0        0        0     6711 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4932 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2200 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     3110 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-25 07:30:21.078543 nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1419 2023-06-25 07:30:29.750815 nonebot_plugin_bilichat-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    14096 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-29 15:31:57.361773 nonebot_plugin_bilichat-2.9.1/LICENSE
+-rw-r--r--   0        0        0    12647 2023-06-29 15:31:57.361773 nonebot_plugin_bilichat-2.9.1/README.md
+-rw-r--r--   0        0        0     9690 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     6614 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      844 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      871 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6502 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    16355 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     2773 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      569 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0     3638 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1187 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2023-06-29 15:31:57.381773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7534 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     2098 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    27644 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/newbing.png
+-rw-r--r--   0        0        0    59199 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     1403 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0    25238 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/newbing.py
+-rw-r--r--   0        0        0     6990 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4932 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2200 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     3118 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-29 15:31:57.385773 nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1419 2023-06-29 15:32:05.813687 nonebot_plugin_bilichat-2.9.1/pyproject.toml
+-rw-r--r--   0        0        0    14033 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.9.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.9.0/LICENSE` & `nonebot_plugin_bilichat-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/README.md` & `nonebot_plugin_bilichat-2.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 ## 📖 介绍
 
 视频链接解析，并根据其内容生成**基本信息**、**词云**和**内容总结**
 
 <details>
 <summary>手机端视图</summary>
-注: 此图片已过时，预期下个版本就会进行更换
 
 ![](docs/mobile.png)
 </details>
 
 <details>
 <summary>基本信息</summary>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
-ææºç«¯è§å¾ æ³¨: æ­¤å¾çå·²è¿æ¶ï¼é¢æä¸ä¸ªçæ¬å°±ä¼è¿è¡æ´æ¢
-![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/bbot_default.png) !
-[style_blue](docs/style_blue.png)   è¯äº ![](docs/wordcloud.png)
-è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨
-nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
-nb plugin install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/
+bbot_default.png) ![style_blue](docs/style_blue.png)   è¯äº ![](docs/
+wordcloud.png)   è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-
+cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat æ³¨:
+ç±äº nb-cli
 ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
 pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
 poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
 plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
```

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/newbing.png` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/newbing.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/newbing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from enum import Enum
 from typing import Literal, Optional, Union
 
 import aiohttp
 import certifi
 import httpx
 
-from ..model.exception import BaseBingChatException
+from ..model.exception import BaseBingChatException, BingCaptchaException
 
 ssl_context = ssl.create_default_context()
 ssl_context.load_verify_locations(certifi.where())
 
 
 DELIMITER = "\x1e"
 
@@ -591,14 +591,18 @@
                                 + "\n"
                             )
                     yield False, resp_txt
 
                 elif response.get("type") == 2:
                     if response["item"]["result"].get("error"):
                         await self.close()
+                        if response["item"]["result"]["value"] == "CaptchaChallenge":
+                            raise BingCaptchaException(
+                                f"{response['item']['result']['value']}: {response['item']['result']['message']}"
+                            )
                         raise BaseBingChatException(
                             f"{response['item']['result']['value']}: {response['item']['result']['message']}",
                         )
 
                     if response["item"]["messages"][-1]["contentOrigin"] == "Apology" and resp_txt:
                         response["item"]["messages"][-1]["text"] = resp_txt_no_link
                         response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0]["text"] = resp_txt
```

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from typing import List, Literal
 
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
-from ..model.exception import AbortError, BingChatResponseException
+from ..model.exception import AbortError, BingChatResponseException, BingCaptchaException
 from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
 from .newbing import Chatbot, ConversationStyle
 from .text_to_image import t2i
 
 cookies = (
     {}
@@ -142,14 +142,17 @@
         elif cache.episodes[cid].newbing == "Refusal to answer":
             return BING_APOLOGY.read_bytes(), False
         else:
             meaning = True
             logger.info("Using cached newbing summarization")
 
         return await t2i(cache.episodes[cid].newbing or "视频无法总结", "new Bing"), meaning
+    except BingCaptchaException as e:
+        logger.error(f"Video(Column) {cache.id} summary failed: {e}")
+        return "newbing 需要 captcha 验证，请在浏览器中随意提问并解决 captcha 后重新导出cookies.json以解决此问题", True
     except BingChatResponseException as e:
         logger.error(f"Video(Column) {cache.id} summary failed: {e}")
         cache.episodes[cid].newbing = "Refusal to answer"
         cache.save()
         return BING_APOLOGY.read_bytes(), False
     except AbortError as e:
         logger.exception(f"Video(Column) {cache.id} summary aborted: {e}")
```

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             type="png",
         )
     return img_raw
 
 
 async def t2i(data: str, src: str):
     try:
-        if len(data) < 30:
+        if len(data.strip()) < 30:
             return data
         if plugin_config.bilichat_use_browser:
             return await pw_text2image(data, src)
         return await rich_text2image(data, src)
     except Exception as e:
         logger.exception(e)
         return f"总结图片生成失败 {e}\n {data}"
```

### Comparing `nonebot_plugin_bilichat-2.9.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.9.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.9.0/pyproject.toml` & `nonebot_plugin_bilichat-2.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.9.0"
+version = "2.9.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.9.0/PKG-INFO` & `nonebot_plugin_bilichat-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.9.0
+Version: 2.9.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -84,15 +84,14 @@
 
 ## 📖 介绍
 
 视频链接解析，并根据其内容生成**基本信息**、**词云**和**内容总结**
 
 <details>
 <summary>手机端视图</summary>
-注: 此图片已过时，预期下个版本就会进行更换
 
 ![](docs/mobile.png)
 </details>
 
 <details>
 <summary>基本信息</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.9.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.9.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
@@ -21,20 +21,20 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
     # nonebot-plugin-bilichat _â¨ å¤åè½çBç«è§é¢è§£æå·¥å· â¨_
 [license] [PyPI_-_Downloads] [pypi] [python] [pdm-managed] [Code_style:_black]
                [onebot] [onebot] [QQ_Chat_Group] [QQ_Chat_Group]
 ## ð ä»ç»
 è§é¢é¾æ¥è§£æï¼å¹¶æ ¹æ®å¶åå®¹çæ**åºæ¬ä¿¡æ¯**ã**è¯äº**å**åå®¹æ»ç»**
-ææºç«¯è§å¾ æ³¨: æ­¤å¾çå·²è¿æ¶ï¼é¢æä¸ä¸ªçæ¬å°±ä¼è¿è¡æ´æ¢
-![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/bbot_default.png) !
-[style_blue](docs/style_blue.png)   è¯äº ![](docs/wordcloud.png)
-è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-cli å®è£ å¨
-nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£
-nb plugin install nonebot-plugin-bilichat æ³¨: ç±äº nb-cli
+ææºç«¯è§å¾ ![](docs/mobile.png)   åºæ¬ä¿¡æ¯ ![bbot_default](docs/
+bbot_default.png) ![style_blue](docs/style_blue.png)   è¯äº ![](docs/
+wordcloud.png)   è§é¢æ»ç» ![](docs/summary.png)  ## ð¿ å®è£  ä½¿ç¨ nb-
+cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-bilichat æ³¨:
+ç±äº nb-cli
 ä¸æ¯æä¾èµç»ï¼å æ­¤éè¦å¯ç¨è¯äºåAIæ»ç»çç¨æ·è¦éè¿å¶ä»çåç®¡çå¨å®è£é¢å¤çä¾èµ
 pip install nonebot-plugin-bilichat[all]   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip pip install
 nonebot-plugin-bilichat[all]   pdm pdm add nonebot-plugin-bilichat[all]
 poetry poetry add nonebot-plugin-bilichat[all]   conda conda install nonebot-
 plugin-bilichat[all]  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
```

