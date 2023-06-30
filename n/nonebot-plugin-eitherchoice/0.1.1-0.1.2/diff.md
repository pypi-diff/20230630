# Comparing `tmp/nonebot_plugin_eitherchoice-0.1.1.tar.gz` & `tmp/nonebot_plugin_eitherchoice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_eitherchoice-0.1.1.tar", last modified: Thu Jun 29 13:02:18 2023, max compression
+gzip compressed data, was "nonebot_plugin_eitherchoice-0.1.2.tar", last modified: Fri Jun 30 12:15:31 2023, max compression
```

## Comparing `nonebot_plugin_eitherchoice-0.1.1.tar` & `nonebot_plugin_eitherchoice-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/LICENSE
--rw-r--r--   0        0        0     4928 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/README.md
--rw-r--r--   0        0        0      949 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/__main__.py
--rw-r--r--   0        0        0     1247 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/config.py
--rw-r--r--   0        0        0     4015 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/data_source.py
--rw-r--r--   0        0        0     1941 2023-06-29 13:01:57.107592 nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/res/template.html.jinja
--rw-r--r--   0        0        0      818 2023-06-29 13:02:18.408802 nonebot_plugin_eitherchoice-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5573 1970-01-01 00:00:00.000000 nonebot_plugin_eitherchoice-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5313 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/README.md
+-rw-r--r--   0        0        0     1087 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/__init__.py
+-rw-r--r--   0        0        0     1619 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/__main__.py
+-rw-r--r--   0        0        0     1247 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/config.py
+-rw-r--r--   0        0        0     4015 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/data_source.py
+-rw-r--r--   0        0        0     1947 2023-06-30 12:15:15.931780 nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/res/template.html.jinja
+-rw-r--r--   0        0        0      818 2023-06-30 12:15:31.792032 nonebot_plugin_eitherchoice-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5958 1970-01-01 00:00:00.000000 nonebot_plugin_eitherchoice-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/LICENSE` & `nonebot_plugin_eitherchoice-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eitherchoice-0.1.1/README.md` & `nonebot_plugin_eitherchoice-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 </div>
 
 ## 📖 介绍
 
 ~~让 AI 帮你一本正经地胡说八道~~
 
+灵感来自 [koishi-plugin-eitherchoice](https://www.npmjs.com/package/koishi-plugin-eitherchoice) ~~（电子蝈蝈，电子博弈，在线观看）~~  
 服务来自 [EitherChoice](https://eitherchoice.com/)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
@@ -112,27 +113,28 @@
 |            配置项            | 必填 | 默认值  |                         说明                         |
 | :--------------------------: | :--: | :-----: | :--------------------------------------------------: |
 |           `PROXY`            |  否  |   无    |                  访问接口使用的代理                  |
 |   `EITHER_CHOICE_TIMEOUT`    |  否  |  `90`   |                 访问接口超时，单位秒                 |
 |    `EITHER_CHOICE_RETRY`     |  否  |   `2`   |                 访问接口最大重试次数                 |
 |     `EITHER_CHOICE_LANG`     |  否  | `zh-CN` |                       目标语言                       |
 | `EITHER_CHOICE_ALLOW_PUBLIC` |  否  | `True`  |             是否允许 AI 上网搜索相关信息             |
-|  `EITHER_CHOICE_PIC_WIDTH`   |  否  | `1280`  | 生成图片的宽度，单位像素（实际宽度可能是这里的一倍） |
+|  `EITHER_CHOICE_PIC_WIDTH`   |  否  | `1280`  | 生成图片的宽度，单位像素（实际宽度可能比这里大一倍） |
 |  `EITHER_CHOICE_MAIN_FONT`   |  否  |   ...   |           生成图片的主字体，使用 CSS 语法            |
 |  `EITHER_CHOICE_CODE_FONT`   |  否  |   ...   |          生成图片的代码字体，使用 CSS 语法           |
 
 ## 🎉 使用
 
 ### 指令
 
-- 指令：对比 要顶的事物 和 要踩的事物
-- 别名：比较、比较一下、锐评、如何评价
+- 指令：对比(下/一下) 要顶的事物 和 要踩的事物
+- 别名：比较、锐评、评价、如何评价
 - 例：
   - 对比 Python 和 JavaScript
-  - 比较一下 C# 和 Java
+  - 锐评一下 C# 和 Java
+  - 比较 “下北泽” 和 东京 (加上引号防止 `下` 或 `一下` 被当做指令的一部分去除)
 
 ### 效果图
 
 ![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/eitherchoice/example.png)
 
 ## 📞 联系
 
@@ -157,10 +159,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-## 0.1.1
+### 0.1.2
+
+- 修复由于 API 地址变动导致的显示 `[object Object]` 问题
+- 微调指令匹配方式
+
+### 0.1.1
 
 - 添加配置项 `EITHER_CHOICE_RETRY`，当访问接口出现问题时，将会自动重试
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-EitherChoice _â¨ è®© AI å¸®ä½ ~~éè¯~~å¯¹æ¯ä¸¤ä»¶äºç©
                     â¨_ [python] [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ~~è®© AI å¸®ä½ ä¸æ¬æ­£ç»å°è¡è¯´å«é~~ æå¡æ¥èª
+## ð ä»ç» ~~è®© AI å¸®ä½ ä¸æ¬æ­£ç»å°è¡è¯´å«é~~ çµææ¥èª
+[koishi-plugin-eitherchoice](https://www.npmjs.com/package/koishi-plugin-
+eitherchoice) ~~ï¼çµå­èèï¼çµå­åå¼ï¼å¨çº¿è§çï¼~~ æå¡æ¥èª
 [EitherChoice](https://eitherchoice.com/) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
 ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-eitherchoice ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-eitherchoice ```   pdm ```bash pdm add nonebot-plugin-
@@ -20,24 +22,28 @@
 é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :-----: | :-------
 -------------------------------------------: | | `PROXY` | å¦ | æ  |
 è®¿é®æ¥å£ä½¿ç¨çä»£ç | | `EITHER_CHOICE_TIMEOUT` | å¦ | `90` |
 è®¿é®æ¥å£è¶æ¶ï¼åä½ç§ | | `EITHER_CHOICE_RETRY` | å¦ | `2` |
 è®¿é®æ¥å£æå¤§éè¯æ¬¡æ° | | `EITHER_CHOICE_LANG` | å¦ | `zh-CN` |
 ç®æ è¯­è¨ | | `EITHER_CHOICE_ALLOW_PUBLIC` | å¦ | `True` | æ¯å¦åè®¸ AI
 ä¸ç½æç´¢ç¸å³ä¿¡æ¯ | | `EITHER_CHOICE_PIC_WIDTH` | å¦ | `1280` |
-çæå¾ççå®½åº¦ï¼åä½åç´ ï¼å®éå®½åº¦å¯è½æ¯è¿éçä¸åï¼
+çæå¾ççå®½åº¦ï¼åä½åç´ ï¼å®éå®½åº¦å¯è½æ¯è¿éå¤§ä¸åï¼
 | | `EITHER_CHOICE_MAIN_FONT` | å¦ | ... | çæå¾ççä¸»å­ä½ï¼ä½¿ç¨
 CSS è¯­æ³ | | `EITHER_CHOICE_CODE_FONT` | å¦ | ... |
 çæå¾ççä»£ç å­ä½ï¼ä½¿ç¨ CSS è¯­æ³ | ## ð ä½¿ç¨ ### æä»¤ -
-æä»¤ï¼å¯¹æ¯ è¦é¡¶çäºç© å è¦è¸©çäºç© -
-å«åï¼æ¯è¾ãæ¯è¾ä¸ä¸ãéè¯ãå¦ä½è¯ä»· - ä¾ï¼ - å¯¹æ¯ Python
-å JavaScript - æ¯è¾ä¸ä¸ C# å Java ### ææå¾ ![Alt text](https://
-raw.githubusercontent.com/lgc-NB2Dev/readme/main/eitherchoice/example.png) ##
-ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
-å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+æä»¤ï¼å¯¹æ¯(ä¸/ä¸ä¸) è¦é¡¶çäºç© å è¦è¸©çäºç© -
+å«åï¼æ¯è¾ãéè¯ãè¯ä»·ãå¦ä½è¯ä»· - ä¾ï¼ - å¯¹æ¯ Python å
+JavaScript - éè¯ä¸ä¸ C# å Java - æ¯è¾ âä¸åæ³½â å ä¸äº¬
+(å ä¸å¼å·é²æ­¢ `ä¸` æ `ä¸ä¸` è¢«å½åæä»¤çä¸é¨åå»é¤) ###
+ææå¾ ![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/
+eitherchoice/example.png) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
+(https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [EitherChoice](https://eitherchoice.com/) -
 æå¡æä¾ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ## 0.1.1 - æ·»å éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.2 - ä¿®å¤ç±äº API
+å°ååå¨å¯¼è´çæ¾ç¤º `[object Object]` é®é¢ - å¾®è°æä»¤å¹éæ¹å¼
+### 0.1.1 - æ·»å éç½®é¡¹
 `EITHER_CHOICE_RETRY`ï¼å½è®¿é®æ¥å£åºç°é®é¢æ¶ï¼å°ä¼èªå¨éè¯
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/__init__.py` & `nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 require("nonebot_plugin_htmlrender")
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __plugin_meta__ = PluginMetadata(
     name="EitherChoice",
     description="让 AI 帮你对比两件事物",
     usage=(
-        "指令：对比 要顶的事物 和 要踩的事物\n"
-        "别名：比较、比较一下、锐评、如何评价\n"
-        "\n"
-        "例：\n"
-        "- 对比 Python 和 JavaScript\n"
-        "- 比较一下 C# 和 Java"
+        "▶ 指令：对比(下/一下) 要顶的事物 和 要踩的事物"
+        "▶ 别名：比较、锐评、评价、如何评价"
+        "▶ 示例："
+        "    ▷ 对比 Python 和 JavaScript"
+        "    ▷ 锐评一下 C# 和 Java"
+        "    ▷ 比较 “下北泽” 和 东京 (加上引号防止 `下` 或 `一下` 被当做指令的一部分去除)"
     ),
     type="application",
     homepage="https://github.com/lgc-NB2Dev/nonebot-plugin-eitherchoice",
     config=ConfigModel,
     supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/__main__.py` & `nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,60 @@
+import string
 from typing import Tuple
 
 from nonebot import logger, on_command
 from nonebot.internal.adapter import Message
 from nonebot.internal.matcher import Matcher
 from nonebot.params import CommandArg
 from nonebot.typing import T_State
 from nonebot_plugin_saa import Image, MessageFactory
 
 from .data_source import get_choice_pic
 
+STRIP_CHARS = "'\"“”‘’"
+ARG_PREFIX = ("下", "一下")
+
+
+def strip_prefix(s: str) -> str:
+    for p in ARG_PREFIX:
+        if s.startswith(p):
+            return s[len(p) :]
+    return s
+
 
 async def check_rule(state: T_State, arg: Message = CommandArg()) -> bool:
     arg_str = arg.extract_plain_text()
 
     if arg_str.count("和") != 1:
         return False
 
     ta, tb = arg_str.split("和")
-    ta = ta.strip()
-    tb = tb.strip()
+    ta = strip_prefix(ta.strip()).strip(STRIP_CHARS)
+    tb = tb.strip(string.whitespace + STRIP_CHARS)
     if not (ta and tb):
         return False
 
     state["things"] = ta, tb
     return True
 
 
 cmd_choice = on_command(
     "对比",
     rule=check_rule,
-    aliases={"比较", "比较一下", "锐评", "如何评价"},
+    aliases={"比较", "锐评", "评价", "如何评价"},
 )
 
 
 @cmd_choice.handle()
 async def _(matcher: Matcher, state: T_State):
     things: Tuple[str, str] = state["things"]
+    # await matcher.finish(f"Things: {things}")
 
     await matcher.send("请稍等，AI 正在帮你评价...")
     try:
         pic = await get_choice_pic(*things)
     except Exception:
         logger.exception("发生错误")
+        logger.error("如果多次发生 Server disconnected 错误，请尝试增加 retry 次数")
         await matcher.finish("发生错误，请检查后台日志")
 
     await MessageFactory(Image(pic)).finish()
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/config.py` & `nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/data_source.py` & `nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         timeout=config.either_choice_timeout,
         proxies=config.proxy,
         http2=True,
         headers=headers,
     ) as client:
         async with client.stream(
             "POST",
-            "https://eitherchoice.com/api/prompt/dev",
+            "https://eitherchoice.com/api/prompt/ask",
             json=body,
         ) as stream:
             async for chunk in stream.aiter_text():
                 yield chunk
 
 
 async def get_choice_all(
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/nonebot_plugin_eitherchoice/res/template.html.jinja` & `nonebot_plugin_eitherchoice-0.1.2/nonebot_plugin_eitherchoice/res/template.html.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
       .title {
         background-image: linear-gradient(to right, #22c55e, #16a34a);
         -webkit-background-clip: text;
         background-clip: text;
         color: transparent;
         font-size: 2.25rem;
-        line-height: 2.5rem;
+        /* line-height: 2.5rem; */
         font-weight: 700;
         text-align: center;
         margin-bottom: 1rem;
       }
 
       th {
         padding-top: 12px;
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/pyproject.toml` & `nonebot_plugin_eitherchoice-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-eitherchoice"
-version = "0.1.1"
+version = "0.1.2"
 description = "Let AI help you compare two things."
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_eitherchoice-0.1.1/PKG-INFO` & `nonebot_plugin_eitherchoice-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-eitherchoice
-Version: 0.1.1
+Version: 0.1.2
 Summary: Let AI help you compare two things.
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-eitherchoice
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-eitherchoice
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0
@@ -53,14 +53,15 @@
 
 </div>
 
 ## 📖 介绍
 
 ~~让 AI 帮你一本正经地胡说八道~~
 
+灵感来自 [koishi-plugin-eitherchoice](https://www.npmjs.com/package/koishi-plugin-eitherchoice) ~~（电子蝈蝈，电子博弈，在线观看）~~  
 服务来自 [EitherChoice](https://eitherchoice.com/)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
@@ -129,27 +130,28 @@
 |            配置项            | 必填 | 默认值  |                         说明                         |
 | :--------------------------: | :--: | :-----: | :--------------------------------------------------: |
 |           `PROXY`            |  否  |   无    |                  访问接口使用的代理                  |
 |   `EITHER_CHOICE_TIMEOUT`    |  否  |  `90`   |                 访问接口超时，单位秒                 |
 |    `EITHER_CHOICE_RETRY`     |  否  |   `2`   |                 访问接口最大重试次数                 |
 |     `EITHER_CHOICE_LANG`     |  否  | `zh-CN` |                       目标语言                       |
 | `EITHER_CHOICE_ALLOW_PUBLIC` |  否  | `True`  |             是否允许 AI 上网搜索相关信息             |
-|  `EITHER_CHOICE_PIC_WIDTH`   |  否  | `1280`  | 生成图片的宽度，单位像素（实际宽度可能是这里的一倍） |
+|  `EITHER_CHOICE_PIC_WIDTH`   |  否  | `1280`  | 生成图片的宽度，单位像素（实际宽度可能比这里大一倍） |
 |  `EITHER_CHOICE_MAIN_FONT`   |  否  |   ...   |           生成图片的主字体，使用 CSS 语法            |
 |  `EITHER_CHOICE_CODE_FONT`   |  否  |   ...   |          生成图片的代码字体，使用 CSS 语法           |
 
 ## 🎉 使用
 
 ### 指令
 
-- 指令：对比 要顶的事物 和 要踩的事物
-- 别名：比较、比较一下、锐评、如何评价
+- 指令：对比(下/一下) 要顶的事物 和 要踩的事物
+- 别名：比较、锐评、评价、如何评价
 - 例：
   - 对比 Python 和 JavaScript
-  - 比较一下 C# 和 Java
+  - 锐评一下 C# 和 Java
+  - 比较 “下北泽” 和 东京 (加上引号防止 `下` 或 `一下` 被当做指令的一部分去除)
 
 ### 效果图
 
 ![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/eitherchoice/example.png)
 
 ## 📞 联系
 
@@ -174,10 +176,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-## 0.1.1
+### 0.1.2
+
+- 修复由于 API 地址变动导致的显示 `[object Object]` 问题
+- 微调指令匹配方式
+
+### 0.1.1
 
 - 添加配置项 `EITHER_CHOICE_RETRY`，当访问接口出现问题时，将会自动重试
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-eitherchoice Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-eitherchoice Version: 0.1.2 Summary:
 Let AI help you compare two things. Home-page: https://github.com/lgc-NB2Dev/
 nonebot-plugin-eitherchoice Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-eitherchoice Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-Dist:
 pydantic>=1.10.4 Requires-Dist: httpx[http2]>=0.24.1 Requires-Dist: nonebot-
 plugin-htmlrender>=0.2.1 Requires-Dist: nonebot-plugin-send-anything-
 anywhere>=0.2.7 Description-Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-EitherChoice _â¨ è®© AI å¸®ä½ ~~éè¯~~å¯¹æ¯ä¸¤ä»¶äºç©
                     â¨_ [python] [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» ~~è®© AI å¸®ä½ ä¸æ¬æ­£ç»å°è¡è¯´å«é~~ æå¡æ¥èª
+## ð ä»ç» ~~è®© AI å¸®ä½ ä¸æ¬æ­£ç»å°è¡è¯´å«é~~ çµææ¥èª
+[koishi-plugin-eitherchoice](https://www.npmjs.com/package/koishi-plugin-
+eitherchoice) ~~ï¼çµå­èèï¼çµå­åå¼ï¼å¨çº¿è§çï¼~~ æå¡æ¥èª
 [EitherChoice](https://eitherchoice.com/) ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
 ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-eitherchoice ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
 nonebot2 é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡,
 æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤  pip ```bash pip
 install nonebot-plugin-eitherchoice ```   pdm ```bash pdm add nonebot-plugin-
@@ -29,24 +31,28 @@
 é»è®¤å¼ | è¯´æ | | :--------------------------: | :--: | :-----: | :-------
 -------------------------------------------: | | `PROXY` | å¦ | æ  |
 è®¿é®æ¥å£ä½¿ç¨çä»£ç | | `EITHER_CHOICE_TIMEOUT` | å¦ | `90` |
 è®¿é®æ¥å£è¶æ¶ï¼åä½ç§ | | `EITHER_CHOICE_RETRY` | å¦ | `2` |
 è®¿é®æ¥å£æå¤§éè¯æ¬¡æ° | | `EITHER_CHOICE_LANG` | å¦ | `zh-CN` |
 ç®æ è¯­è¨ | | `EITHER_CHOICE_ALLOW_PUBLIC` | å¦ | `True` | æ¯å¦åè®¸ AI
 ä¸ç½æç´¢ç¸å³ä¿¡æ¯ | | `EITHER_CHOICE_PIC_WIDTH` | å¦ | `1280` |
-çæå¾ççå®½åº¦ï¼åä½åç´ ï¼å®éå®½åº¦å¯è½æ¯è¿éçä¸åï¼
+çæå¾ççå®½åº¦ï¼åä½åç´ ï¼å®éå®½åº¦å¯è½æ¯è¿éå¤§ä¸åï¼
 | | `EITHER_CHOICE_MAIN_FONT` | å¦ | ... | çæå¾ççä¸»å­ä½ï¼ä½¿ç¨
 CSS è¯­æ³ | | `EITHER_CHOICE_CODE_FONT` | å¦ | ... |
 çæå¾ççä»£ç å­ä½ï¼ä½¿ç¨ CSS è¯­æ³ | ## ð ä½¿ç¨ ### æä»¤ -
-æä»¤ï¼å¯¹æ¯ è¦é¡¶çäºç© å è¦è¸©çäºç© -
-å«åï¼æ¯è¾ãæ¯è¾ä¸ä¸ãéè¯ãå¦ä½è¯ä»· - ä¾ï¼ - å¯¹æ¯ Python
-å JavaScript - æ¯è¾ä¸ä¸ C# å Java ### ææå¾ ![Alt text](https://
-raw.githubusercontent.com/lgc-NB2Dev/readme/main/eitherchoice/example.png) ##
-ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333)
-å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+æä»¤ï¼å¯¹æ¯(ä¸/ä¸ä¸) è¦é¡¶çäºç© å è¦è¸©çäºç© -
+å«åï¼æ¯è¾ãéè¯ãè¯ä»·ãå¦ä½è¯ä»· - ä¾ï¼ - å¯¹æ¯ Python å
+JavaScript - éè¯ä¸ä¸ C# å Java - æ¯è¾ âä¸åæ³½â å ä¸äº¬
+(å ä¸å¼å·é²æ­¢ `ä¸` æ `ä¸ä¸` è¢«å½åæä»¤çä¸é¨åå»é¤) ###
+ææå¾ ![Alt text](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/
+eitherchoice/example.png) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
+(https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
+?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [EitherChoice](https://eitherchoice.com/) -
 æå¡æä¾ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ## 0.1.1 - æ·»å éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.2 - ä¿®å¤ç±äº API
+å°ååå¨å¯¼è´çæ¾ç¤º `[object Object]` é®é¢ - å¾®è°æä»¤å¹éæ¹å¼
+### 0.1.1 - æ·»å éç½®é¡¹
 `EITHER_CHOICE_RETRY`ï¼å½è®¿é®æ¥å£åºç°é®é¢æ¶ï¼å°ä¼èªå¨éè¯
```

