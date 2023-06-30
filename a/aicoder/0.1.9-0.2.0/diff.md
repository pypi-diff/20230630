# Comparing `tmp/aicoder-0.1.9-py3-none-any.whl.zip` & `tmp/aicoder-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 21412 bytes, number of entries: 12
--rw-r--r--  2.0 unx    12661 b- defN 23-Jun-30 11:34 aicoder/AICoder.py
--rw-r--r--  2.0 unx     8122 b- defN 23-Jun-30 11:34 aicoder/AICoderFull.py
--rw-r--r--  2.0 unx     5433 b- defN 23-Jun-30 12:00 aicoder/AICoderPartial.py
+Zip file size: 21432 bytes, number of entries: 12
+-rw-r--r--  2.0 unx    12669 b- defN 23-Jun-30 12:05 aicoder/AICoder.py
+-rw-r--r--  2.0 unx     8138 b- defN 23-Jun-30 12:04 aicoder/AICoderFull.py
+-rw-r--r--  2.0 unx     5449 b- defN 23-Jun-30 12:04 aicoder/AICoderPartial.py
 -rw-r--r--  2.0 unx     3481 b- defN 23-Jun-28 23:49 aicoder/AICoderPrompts.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 11:14 aicoder/__init__.py
--rw-r--r--  2.0 unx    14570 b- defN 23-Jun-30 12:01 aicoder/main.py
--rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/LICENSE
--rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 12:03 aicoder-0.1.9.dist-info/RECORD
-12 files, 64640 bytes uncompressed, 19832 bytes compressed:  69.3%
+-rw-r--r--  2.0 unx    14586 b- defN 23-Jun-30 12:04 aicoder/main.py
+-rw-r--r--  2.0 unx    18809 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-Jun-30 12:05 aicoder-0.2.0.dist-info/RECORD
+12 files, 64696 bytes uncompressed, 19852 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: aicoder/__init__.py
 Comment: 
 
 Filename: aicoder/main.py
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/LICENSE
+Filename: aicoder-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/METADATA
+Filename: aicoder-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/WHEEL
+Filename: aicoder-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/entry_points.txt
+Filename: aicoder-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/top_level.txt
+Filename: aicoder-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aicoder-0.1.9.dist-info/RECORD
+Filename: aicoder-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aicoder/AICoder.py

```diff
@@ -2,15 +2,15 @@
 import colorlog
 import openai
 import json
 import os
 import re
 import subprocess
 from threading import Lock
-from AICoderPrompts import PERSONALITY, PROGRAM_TO_GENERATE, FINAL_CLARIFICATIONS, GET_FILE_CONTENTS, ERROR_FIX, GET_ERRORS_JSON, COMPILATION_COMMAND
+from aicoder.AICoderPrompts import PERSONALITY, PROGRAM_TO_GENERATE, FINAL_CLARIFICATIONS, GET_FILE_CONTENTS, ERROR_FIX, GET_ERRORS_JSON, COMPILATION_COMMAND
 
 
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
```

## aicoder/AICoderFull.py

```diff
@@ -2,16 +2,16 @@
 import colorlog
 import json
 import os
 import concurrent.futures
 from concurrent.futures import ThreadPoolExecutor
 from tqdm import tqdm
 from time import sleep
-from AICoderPrompts import GET_ALL_FILES
-from AICoder import AICoder, ALL_IMPORTS, IMPORTS_LOCK
+from aicoder.AICoderPrompts import GET_ALL_FILES
+from aicoder.AICoder import AICoder, ALL_IMPORTS, IMPORTS_LOCK
 
 
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
```

## aicoder/AICoderPartial.py

```diff
@@ -1,16 +1,16 @@
 import logging
 from typing import List
 import colorlog
 import subprocess
 import os
 import urllib.parse
 from github import Github
-from AICoderPrompts import MODIFY_FILE, FILE_FROM_TEMPALTES
-from AICoder import AICoder
+from aicoder.AICoderPrompts import MODIFY_FILE, FILE_FROM_TEMPALTES
+from aicoder.AICoder import AICoder
 
 # Setting up logger
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
```

## aicoder/main.py

```diff
@@ -4,16 +4,16 @@
 import string
 import random
 import requests
 import logging
 import colorlog
 import subprocess
 from concurrent.futures import ThreadPoolExecutor
-from AICoderFull import AICoderFull
-from AICoderPartial import AICoderPartial
+from aicoder.AICoderFull import AICoderFull
+from aicoder.AICoderPartial import AICoderPartial
 
 # Logger setup
 handler = colorlog.StreamHandler()
 handler.setFormatter(colorlog.ColoredFormatter('%(log_color)s%(levelname)s:%(message)s'))
 logger = colorlog.getLogger('file_generator')
 if not logger.hasHandlers():
     logger.addHandler(handler)
```

## Comparing `aicoder-0.1.9.dist-info/LICENSE` & `aicoder-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aicoder-0.1.9.dist-info/RECORD` & `aicoder-0.2.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-aicoder/AICoder.py,sha256=URmNrQngdcJz2K7spT8Jg4n6yJ37GZHNE408zWyZe04,12661
-aicoder/AICoderFull.py,sha256=Z-_8Bh_wxGoNaTLVIC6JfeBMfCXCDqzknTkb-pYQODE,8122
-aicoder/AICoderPartial.py,sha256=_G5OYODc9HECa-T9JYHsHXIVfoT6ql6sF-uIdR6nmBU,5433
+aicoder/AICoder.py,sha256=JD6NVUiqbQH9yKxSCeoynQwcIWDrWJCuipwwoqFJ8sA,12669
+aicoder/AICoderFull.py,sha256=twZM0v57Zpa0S8nE9pmv-DWsncZcxDPVcXiOZgTWfzU,8138
+aicoder/AICoderPartial.py,sha256=_NadBlkGml2FSfK0gJPyN4zVUkQpe6e6nwAeywmJlEI,5449
 aicoder/AICoderPrompts.py,sha256=ZQGA2rNfSHzYdmc914960_HOJagGO_AuRXn_08sMeW4,3481
 aicoder/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aicoder/main.py,sha256=7MPU0RF0SMwTjKATgkN2CNhpmyu1KZ2TEHuDa4cxVXo,14570
-aicoder-0.1.9.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
-aicoder-0.1.9.dist-info/METADATA,sha256=cZQlKNBtGMtjz8O1tTvgE_ORHfznNMQcI56Fo5kmo9c,473
-aicoder-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aicoder-0.1.9.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
-aicoder-0.1.9.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
-aicoder-0.1.9.dist-info/RECORD,,
+aicoder/main.py,sha256=wXJXURSK7-H1_K33LHVhf_zh2OFmzvz389fgla7lDPc,14586
+aicoder-0.2.0.dist-info/LICENSE,sha256=nGKG3YDYTyar3KKwoaLPInTfnNQtuvh4aMwTADTd0L8,18809
+aicoder-0.2.0.dist-info/METADATA,sha256=DiiPdmkTBgNHPCQ1A7uA5_BREvECxdrAiXQoKC6xY1s,473
+aicoder-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aicoder-0.2.0.dist-info/entry_points.txt,sha256=m__okhQaM4kZ8CCfSA5VGUyQ0gf7TIGax6DhXdTnAeA,46
+aicoder-0.2.0.dist-info/top_level.txt,sha256=B8Pf-hhM5icZE_7vMCXD5mXWG0MAqt5ImotI1aNXdWQ,8
+aicoder-0.2.0.dist-info/RECORD,,
```

