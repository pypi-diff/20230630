# Comparing `tmp/vios-1.0.2-py3-none-any.whl.zip` & `tmp/vios-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 33236 bytes, number of entries: 23
+Zip file size: 33360 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat      781 b- defN 23-Jun-26 13:01 vios/__init__.py
 -rw-rw-rw-  2.0 fat     4936 b- defN 23-Jun-26 13:00 vios/collection/__init__.py
 -rw-rw-rw-  2.0 fat     3515 b- defN 23-Jun-26 11:28 vios/collection/support.py
 -rw-rw-rw-  2.0 fat    11254 b- defN 23-Jun-19 15:11 vios/collection/tasks.py
--rw-rw-rw-  2.0 fat    10235 b- defN 23-Jun-26 11:28 vios/collection/uapi.py
+-rw-rw-rw-  2.0 fat    10198 b- defN 23-Jun-28 07:10 vios/collection/uapi.py
 -rw-rw-rw-  2.0 fat     4756 b- defN 23-Jun-19 15:11 vios/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat     2962 b- defN 23-Jun-19 15:11 vios/driver/__init__.py
 -rw-rw-rw-  2.0 fat      209 b- defN 23-Jun-26 11:28 vios/driver/common/__init__.py
--rw-rw-rw-  2.0 fat     4199 b- defN 23-Jun-26 13:04 vios/driver/common/basedriver.py
+-rw-rw-rw-  2.0 fat     4192 b- defN 23-Jun-28 07:10 vios/driver/common/basedriver.py
 -rw-rw-rw-  2.0 fat     4666 b- defN 23-Jun-19 15:11 vios/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5546 b- defN 23-Jun-19 15:11 vios/driver/common/visadriver.py
--rw-rw-rw-  2.0 fat      784 b- defN 23-Jun-21 12:45 vios/envelope/__init__.py
--rw-rw-rw-  2.0 fat    12840 b- defN 23-Jun-26 11:28 vios/envelope/assembler.py
+-rw-rw-rw-  2.0 fat      784 b- defN 23-Jun-30 06:18 vios/envelope/__init__.py
+-rw-rw-rw-  2.0 fat    13293 b- defN 23-Jun-30 05:21 vios/envelope/assembler.py
 -rw-rw-rw-  2.0 fat    10541 b- defN 23-Jun-26 11:28 vios/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-19 15:11 vios/envelope/device.py
 -rw-rw-rw-  2.0 fat     1719 b- defN 23-Jun-26 11:28 vios/envelope/processor.py
 -rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-26 12:50 vios/envelope/rule.py
 -rw-rw-rw-  2.0 fat      522 b- defN 23-Jun-26 11:28 vios/tools/__init__.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-27 03:36 vios-1.0.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1000 b- defN 23-Jun-27 03:36 vios-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-27 03:36 vios-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jun-27 03:36 vios-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1857 b- defN 23-Jun-27 03:36 vios-1.0.2.dist-info/RECORD
-23 files, 87535 bytes uncompressed, 30256 bytes compressed:  65.4%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1000 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1857 b- defN 23-Jun-30 06:18 vios-1.0.3.dist-info/RECORD
+23 files, 87944 bytes uncompressed, 30380 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: vios/envelope/rule.py
 Comment: 
 
 Filename: vios/tools/__init__.py
 Comment: 
 
-Filename: vios-1.0.2.dist-info/LICENSE
+Filename: vios-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: vios-1.0.2.dist-info/METADATA
+Filename: vios-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: vios-1.0.2.dist-info/WHEEL
+Filename: vios-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: vios-1.0.2.dist-info/top_level.txt
+Filename: vios-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-1.0.2.dist-info/RECORD
+Filename: vios-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vios/collection/uapi.py

```diff
@@ -1,10 +1,9 @@
 import random
 import time
-from collections import OrderedDict
 from datetime import datetime
 from pathlib import Path
 
 import matplotlib.image as mim
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib import colors
```

## vios/driver/common/basedriver.py

```diff
@@ -1,11 +1,11 @@
 import re
 from abc import ABC, abstractmethod
 from copy import deepcopy
-from typing import Any, Union
+from typing import Any
 
 from .quantity import newcfg
 
 PATTERN = r'^192\.168\.({seg})\.((2(5[0-5]|[0-4]\d))|[0-1]?\d{{1,2}})'
 
 
 class BaseDriver(ABC):
```

## vios/envelope/assembler.py

```diff
@@ -17,26 +17,29 @@
 
 
 #region context
 class CompilerContext(QuarkLocalConfig):
     def __init__(self, data) -> None:
         super().__init__(data)
         self.reset(data)
+        self.initial = {}
+        self.bypass = {}
+        self._keys = []
 
     def reset(self, snapshot):
         if isinstance(snapshot, dict):
             self._QuarkLocalConfig__driver = DictDriver(deepcopy(snapshot))
         else:
             self._QuarkLocalConfig__driver = snapshot
 
 
 cfg = CompilerContext({})  # cfg (QuarkLocalConfig): 线路编绎所需配置
 
 
-def initialize(snapshot):
+def initialize(snapshot, **kwds):
     """初始化编译上下文环境，即每个线路对应的当前的cfg表
 
     Args:
         snapshot (_type_): 当前的cfg表
 
     Returns:
         QuarkLocalConfig: 用于编译的上下文环境
@@ -46,14 +49,17 @@
     #     if isinstance(snapshot, dict):
     #         self.__driver = DictDriver(deepcopy(snapshot))
     #     else:
     #         super().reset(snapshot)
 
     """
     cfg.reset(snapshot)
+    cfg.initial = kwds.get('initial', {'restore': [('WAIT', 'T', 0.01, 's')]})
+    cfg.bypass = kwds.get('bypass', {})
+    cfg._keys = kwds.get('keys', [])
     return cfg
 #endregion context
 
 
 #region compile
 def _form_signal(sig):
     """signal类型
@@ -82,15 +88,15 @@
             pass
     elif isinstance(sig, Signal):
         return sig
     raise ValueError(f'unknow type of signal "{sig}".'
                      f" optional signal types: {list(sig_tab.keys())}")
 
 
-def ccompile(sid: int, circuit: list, **kwds):
+def ccompile(sid: int, steps: dict, circuit: list, **kwds):
     """编绎线路，生成可执行的指令，包括波形生成、采集卡参数、触发设置等
 
     Args:
         sid (int): 任务步数
         circuit (list): 用户定义的线路(@HK)
 
     Returns:
@@ -98,15 +104,14 @@
 
     >>> from quark import connect
     >>> s = connect('QuarkServer')
     >>> cfg = initialize(s.snapshot())
     >>> circuit = [(('Measure',0),'Q0503')]
     >>> instruction, datamap =ccompile(0,circuit,signal='iq')
     >>> instruction
-    where instruction is:
     {'main': [('WRITE', 'Q0503.waveform.DDS', <waveforms.waveform.Waveform at 0x291381b6c80>, ''),
               ('WRITE', 'M5.waveform.DDS', <waveforms.waveform.Waveform at 0x291381b7f40>, ''),
               ('WRITE', 'ADx86_159.CH5.Shot', 1024, ''),
               ('WRITE', 'ADx86_159.CH5.Coefficient', {'start': 2.4000000000000003e-08,
                                                       'stop': 4.0299999999999995e-06,
                                                       'wList': [{'Delta': 6932860000.0,
                                                                   'phase': 0,
@@ -138,38 +143,48 @@
                 'signal': 2,
                 'arch': 'baqis'}}
 
     """
     kwds['signal'] = _form_signal(kwds.get('signal'))
     kwds['lib'] = stdlib
 
+    ctx = kwds.get('ctx', cfg)
+
     # print('Compiling', circuit)
-    code = _compile(circuit, cfg=cfg, **kwds)
+    code = _compile(circuit, cfg=ctx, **kwds)
     cmds, datamap = assembly_code(code)
     # print('Compiled', cmds)
     instruction = {}
     for cmd in cmds:
         ctype = type(cmd).__name__  # WRITE,TRIG,READ
         if ctype == 'WRITE':
             step = 'main'
         else:
             step = ctype
         op = (ctype, cmd.address, cmd.value, '')
         if step in instruction:
             instruction[step].append(op)
         else:
             instruction[step] = [op]
-    return instruction, {'dataMap': datamap}
+
+    # merge loop body with compiled result
+    for step, _cmds in instruction.items():
+        if step in steps:
+            steps[step].extend(_cmds)
+        else:
+            steps[step] = _cmds
+
+    return steps, {'dataMap': datamap} | kwds
 
 #endregion compile
 
 
 #region assemble
 
-def assemble(sid: int, instruction: dict[str, list[str, str, Any, str]], bypass: dict = {}, initial: list = []):
+def assemble(sid: int, instruction: dict[str, list[str, str, Any, str]]):
     """重组编译(ccompile)生成的指令集合(见cccompile), 并生成相应的硬件操作指令
 
     Args:
         sid (int): 任务步数
         instruction (dict[str, list[str, str, Any, str]]): 编译生成的指令集合(见ccompile)，可能包括额外的操作
         bypass (dict, optional): 缓存已有指令，避免重复设置. Defaults to {}.
         initial (list, optional): 初始值，用于任务结束时恢复设置. Defaults to [].
@@ -192,23 +207,23 @@
                     kwds.update({"context": context, 'cached': ccmd})
                 except (ValueError, KeyError) as e:
                     ccmd[target] = value
                     continue
 
                 if sid == 0:
                     init = cfg.query(target.removesuffix('.Q').removesuffix('.Q'))
-                    initial.append((ctype, target, init, unit))
+                    cfg.initial['restore'].append((ctype, target, init, unit))
 
             if ctype != 'WAIT':
                 dev = _target.split('.', 1)[0]
                 kwds['srate'] = cfg.query(f'dev.{dev}.srate')
             _wrval = [ctype, value, unit, kwds]
 
             try:
-                preprocess(_target, _wrval, scmd, bypass)
+                preprocess(_target, _wrval, scmd, cfg.bypass)
             except Exception as e:
                 print(f'Failed to preprocess {target}!')
                 scmd[_target] = _wrval
         instruction[step] = scmd
 
 
 # 设备通道与config表中字段的映射关系
```

## Comparing `vios-1.0.2.dist-info/LICENSE` & `vios-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-1.0.2.dist-info/METADATA` & `vios-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 1.0.2
+Version: 1.0.3
 Summary: runtime requirements for systemq
 Author-email: YL <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-1.0.2.dist-info/RECORD` & `vios-1.0.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 vios/__init__.py,sha256=pQ_BUjQ_ZCki4pI_wid9yJbQi_YK2uWG3rixAEbC670,781
 vios/collection/__init__.py,sha256=jVv6Lv-ByJWhXnXT1fSnuz6rCMqSnGCT-Z4NNu9xiH8,4936
 vios/collection/support.py,sha256=78G1G0vyDInEfW4j4RGdt7uM8gt_M3_Ucm_3_zm7jB0,3515
 vios/collection/tasks.py,sha256=FUAGla2yjy4apdM5PLZ7yJP0YsbMajat1gm8bt7y7QI,11254
-vios/collection/uapi.py,sha256=VfNmww9-p2x7JyOsWS_I9GGxvWTQmeBYFuB0Muo9xc4,10235
+vios/collection/uapi.py,sha256=bmjnw6XokSU-0Zkt7XTldjAY0kF48RbHuFVVnE-EkSI,10198
 vios/driver/VirtualDevice.py,sha256=sf87LAcRvJIVZW-OyP8Hw-CWu7isonbr2-TjFGZHYSk,4756
 vios/driver/__init__.py,sha256=rvTlhtDHO_l1rHNsgb3PA9LnEirl4TIm0bvlgRseRnY,2962
 vios/driver/common/__init__.py,sha256=rwnAg6V2hY1vinIHlvGwKTXn34SRQHX8bnIleycTM6k,209
-vios/driver/common/basedriver.py,sha256=Ap7WBhRI2sGSRrYhFCDUuchMdi-OixUUvyRn6pW28nI,4199
+vios/driver/common/basedriver.py,sha256=jQ3svU_t1v0Zt8lRX8ij8MhwilmIwziozwuTFeRxRnE,4192
 vios/driver/common/quantity.py,sha256=70feNhld2lF04KHQ3zWDliS_cmD1q97Yi0oFqlwYijs,4666
 vios/driver/common/visadriver.py,sha256=WY6TqGmow_K5ePAYIYkG12IxjHfAczuxYTvPk4VmVG4,5546
 vios/envelope/__init__.py,sha256=97kXED9oaUd56J2OoVCTQpctkQZDcAZWxpEQakTxCRM,784
-vios/envelope/assembler.py,sha256=ARxCK_PeURJmW7uaVnDuJ5Q2MOukqoVlLRhWrWyZ-nI,12840
+vios/envelope/assembler.py,sha256=9UcTDB-hL3EA8B0QUA7luD22gCipzJrn-VRRu7VA9ZM,13293
 vios/envelope/calculator.py,sha256=eE7730YFzArrukuDh0dI0JabG2PiEz3eo3N4Czqgk88,10541
 vios/envelope/device.py,sha256=rQeLe_Y9MTwLZfJsSK9MhvZxdOnrtJNcOZriS6Rm1Io,1047
 vios/envelope/processor.py,sha256=4py3AwLurBTrhXXJCvdfHrMeKGzOFl-gICQTNjpoyQM,1719
 vios/envelope/rule.py,sha256=ANiUVCtozVP6B6m8En55VLqOHWdeMkuA7KqiAiFyAnQ,2980
 vios/tools/__init__.py,sha256=vq-1N9Zjm_ZYcD9_lwX9fKlcMT9Rx7Kd3BDRqmKhMT0,522
-vios-1.0.2.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
-vios-1.0.2.dist-info/METADATA,sha256=ZRC62rAPesQcwmtc24ydYs-_8N4tfasdmLWFl8SarA4,1000
-vios-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-1.0.2.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
-vios-1.0.2.dist-info/RECORD,,
+vios-1.0.3.dist-info/LICENSE,sha256=N0ypn_97IUjlPVBH8az2Wt02D-9ROQafRq1D6tcqorE,1089
+vios-1.0.3.dist-info/METADATA,sha256=QGh6SLu3E1TVTsVMXl7euSmxhUZrikrLMqTIJavIm20,1000
+vios-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-1.0.3.dist-info/top_level.txt,sha256=4DHqoaYuzp4X6-_w1r1lk0039QUzXe7OVi76KeUqjZM,5
+vios-1.0.3.dist-info/RECORD,,
```

