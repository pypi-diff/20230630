# Comparing `tmp/cns-1.0.38-py3-none-any.whl.zip` & `tmp/cns-1.0.39-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,23 @@
-Zip file size: 485201 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-29 09:38 cns/DataX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-29 09:38 cns/DataX.cp39-win_amd64.pyd
+Zip file size: 655715 bytes, number of entries: 21
+-rw-rw-rw-  2.0 fat   140288 b- defN 23-Jun-30 03:48 cns/DataX.cp36-win32.pyd
+-rw-rw-rw-  2.0 fat   178176 b- defN 23-Jun-30 03:48 cns/DataX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-30 03:48 cns/DataX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    82944 b- defN 23-Jun-02 15:12 cns/DateTimeX.cp36-win32.pyd
 -rw-rw-rw-  2.0 fat    99840 b- defN 23-Jun-02 15:11 cns/DateTimeX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    88576 b- defN 23-Jun-02 15:13 cns/DateTimeX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    88064 b- defN 23-Jun-30 02:07 cns/OTPX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-30 02:07 cns/OTPX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    84992 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    74240 b- defN 23-Jun-16 07:35 cns/SQLstrX.cp39-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    77312 b- defN 23-Jun-23 11:03 cns/TextX.cp36-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    65536 b- defN 23-Jun-23 11:02 cns/TextX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      417 b- defN 23-Jun-26 05:16 cns/__init__.py
--rw-rw-rw-  2.0 fat   101888 b- defN 23-Jun-26 14:00 cns/cmdX.cp36-win_amd64.pyd
--rw-rw-rw-  2.0 fat    87040 b- defN 23-Jun-26 14:00 cns/cmdX.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2001 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1399 b- defN 23-Jun-29 09:40 cns-1.0.38.dist-info/RECORD
-17 files, 1098535 bytes uncompressed, 482933 bytes compressed:  56.0%
+-rw-rw-rw-  2.0 fat      428 b- defN 23-Jun-30 02:08 cns/__init__.py
+-rw-rw-rw-  2.0 fat    79360 b- defN 23-Jun-30 02:21 cns/cmdX.cp36-win32.pyd
+-rw-rw-rw-  2.0 fat   101888 b- defN 23-Jun-30 02:22 cns/cmdX.cp36-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    87040 b- defN 23-Jun-30 02:22 cns/cmdX.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-30 04:34 cns-1.0.39.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2001 b- defN 23-Jun-30 04:34 cns-1.0.39.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-30 04:34 cns-1.0.39.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-30 04:34 cns-1.0.39.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1733 b- defN 23-Jun-30 04:34 cns-1.0.39.dist-info/RECORD
+21 files, 1480832 bytes uncompressed, 652941 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: cns/DataX.cp36-win32.pyd
+Comment: 
+
 Filename: cns/DataX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/DataX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/DateTimeX.cp36-win32.pyd
@@ -9,14 +12,20 @@
 
 Filename: cns/DateTimeX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/DateTimeX.cp39-win_amd64.pyd
 Comment: 
 
+Filename: cns/OTPX.cp36-win_amd64.pyd
+Comment: 
+
+Filename: cns/OTPX.cp39-win_amd64.pyd
+Comment: 
+
 Filename: cns/SQLstrX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/SQLstrX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/TextX.cp36-win_amd64.pyd
@@ -24,29 +33,32 @@
 
 Filename: cns/TextX.cp39-win_amd64.pyd
 Comment: 
 
 Filename: cns/__init__.py
 Comment: 
 
+Filename: cns/cmdX.cp36-win32.pyd
+Comment: 
+
 Filename: cns/cmdX.cp36-win_amd64.pyd
 Comment: 
 
 Filename: cns/cmdX.cp39-win_amd64.pyd
 Comment: 
 
-Filename: cns-1.0.38.dist-info/LICENSE
+Filename: cns-1.0.39.dist-info/LICENSE
 Comment: 
 
-Filename: cns-1.0.38.dist-info/METADATA
+Filename: cns-1.0.39.dist-info/METADATA
 Comment: 
 
-Filename: cns-1.0.38.dist-info/WHEEL
+Filename: cns-1.0.39.dist-info/WHEEL
 Comment: 
 
-Filename: cns-1.0.38.dist-info/top_level.txt
+Filename: cns-1.0.39.dist-info/top_level.txt
 Comment: 
 
-Filename: cns-1.0.38.dist-info/RECORD
+Filename: cns-1.0.39.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cns/__init__.py

```diff
@@ -1,10 +1,10 @@
-# 定义当使用“from my_package import *”时导入的内容
+# -*- coding: UTF-8 -*-
 #__all__ = ["DateTimeX"]  # *导入类时限制在此范围
 
 from .DateTimeX import DateTimeX     # 日期获取
 from .DataX import DataX             # 数据处理
 from .TextX import TextX             # 文本处理
 from .SQLstrX import SQLstrX         # RPASQL处理
-from .cmdX import cmdX             # 路径处理(修改文件名等)
-
+from .cmdX import cmdX               # 路径处理(修改文件名等)
+from .OTPX import OTPX               # 动态口令
```

## Comparing `cns-1.0.38.dist-info/METADATA` & `cns-1.0.39.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cns
-Version: 1.0.38
+Version: 1.0.39
 Summary: cns工具包
 Home-page: https://cns.ink/example
 Author: Rambo
 Author-email: 6566666@qq.com
 License: Copyright (C) 2023 CNS. All Rights Reserved. See LICENSE for license.
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `cns-1.0.38.dist-info/RECORD` & `cns-1.0.39.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-cns/DataX.cp36-win_amd64.pyd,sha256=tfeVxdEgqCDZd_uS9CEBbH3vk_cZLtcee_hB_ZeNE0o,178176
-cns/DataX.cp39-win_amd64.pyd,sha256=uuL22X4jAKstGC5Utsvdt7_ccDC7GjFAO7zZ3NRKcz4,153600
+cns/DataX.cp36-win32.pyd,sha256=jPEQdDmq8RwH1dhKCf7YzJA3GNpDzXi9e4Eq6MiBbG0,140288
+cns/DataX.cp36-win_amd64.pyd,sha256=QPojpbys5qhboJ9yu7RqFKyQCRQODDuA6zYwy1gHfkQ,178176
+cns/DataX.cp39-win_amd64.pyd,sha256=lJQ1PUox-nGluq9OD7cJrMQhlfCSitVj8x2E3CQDKdk,153600
 cns/DateTimeX.cp36-win32.pyd,sha256=X6jjFZbOMmTTqnw0r3SfmiTRG9RFEpRdfVyU6AiFvCk,82944
 cns/DateTimeX.cp36-win_amd64.pyd,sha256=w-g6QPTK_U3il2bFu7PcucBGixhSX2Gm4M54ItAYMTk,99840
 cns/DateTimeX.cp39-win_amd64.pyd,sha256=bp9N6_ettlJ1odtrHJ3qU_yTBAsvULggzIyfz-eJuEk,88576
+cns/OTPX.cp36-win_amd64.pyd,sha256=cmWUVENEYKVmv6gFHPuuDQ85qARuXDYE8QJa5-qob7M,88064
+cns/OTPX.cp39-win_amd64.pyd,sha256=gifLhBrujnmf-O0ha6QK3lW9bK3SQFZheF8KJqFmFUg,74240
 cns/SQLstrX.cp36-win_amd64.pyd,sha256=3NLRKJa7q2Dl1sKlzVBbScgYjcgoSgMOClS2BuxDIzI,84992
 cns/SQLstrX.cp39-win_amd64.pyd,sha256=B0wq2UBpInSyGEq6aGOvKiqwAov8_ynHtlkPnaYav8k,74240
 cns/TextX.cp36-win_amd64.pyd,sha256=cbQwr_FGkhhWoyyq3i43Tj11YSa-8r_3ZSN5JpXTcWk,77312
 cns/TextX.cp39-win_amd64.pyd,sha256=tJkutc00Vya2KBtXFWGcCm0wOSt9vvAm_7cZBsB1DgE,65536
-cns/__init__.py,sha256=t6RixBCw_0B4wUVAo2KTIOea-6tMeUneUQs6hXOS2ao,417
-cns/cmdX.cp36-win_amd64.pyd,sha256=-saULFU8EL3nYz7hBAYhKrg81qdSsLYVepV3QmHaz4g,101888
-cns/cmdX.cp39-win_amd64.pyd,sha256=jangzLwhz4_0gTB2rTdKsogUe01conQguA3LJKLgGNE,87040
-cns-1.0.38.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
-cns-1.0.38.dist-info/METADATA,sha256=e0jaElhwS1jdMAHZbrfhQ1Z8uQxiJmNv7KzT9X8pnq0,2001
-cns-1.0.38.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-cns-1.0.38.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
-cns-1.0.38.dist-info/RECORD,,
+cns/__init__.py,sha256=OkiLZaBAE60ryksXe3OeD0hLTmnSGmNMGIJzYPC82nM,428
+cns/cmdX.cp36-win32.pyd,sha256=L0QTCztAz3VZ17x8Nf3cSHIIDOCFVWHNNHD_31ywnTc,79360
+cns/cmdX.cp36-win_amd64.pyd,sha256=yxEASvpFt4I7BOFafrgLZ1Yu42BBFr-TMLfhFH1OptM,101888
+cns/cmdX.cp39-win_amd64.pyd,sha256=J95o5AivVbnnlV7W9fse7tJ6My6q_PLaa33f_jS1IEg,87040
+cns-1.0.39.dist-info/LICENSE,sha256=OCcV9iTKhNBVidknwiPS8X-OLMdgbpsuUL9EzN6Q5zI,473
+cns-1.0.39.dist-info/METADATA,sha256=ThTz45XOYLm14icdLKN4ozLSdzKudIvDVc8UWoYmKS8,2001
+cns-1.0.39.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+cns-1.0.39.dist-info/top_level.txt,sha256=oA9qczli9LkRhNJ77Ah4syjSkuiqmSaR2pTif57e9pM,4
+cns-1.0.39.dist-info/RECORD,,
```

