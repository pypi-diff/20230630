# Comparing `tmp/mbapy-0.1.2.tar.gz` & `tmp/mbapy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.1.2.tar", last modified: Mon Jun 12 15:19:56 2023, max compression
+gzip compressed data, was "mbapy-0.1.3.tar", last modified: Fri Jun 30 13:37:37 2023, max compression
```

## Comparing `mbapy-0.1.2.tar` & `mbapy-0.1.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.699653 mbapy-0.1.2/
--rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6409 2023-06-12 15:19:56.698651 mbapy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5635 2023-06-02 01:55:22.000000 mbapy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.639455 mbapy-0.1.2/mbapy/
--rw-rw-rw-   0        0        0      590 2023-05-25 14:57:15.000000 mbapy-0.1.2/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2023-06-12 15:15:55.000000 mbapy-0.1.2/mbapy/__version__.py
--rw-rw-rw-   0        0        0     4503 2023-06-06 15:58:38.000000 mbapy-0.1.2/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.663456 mbapy-0.1.2/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.2/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.664456 mbapy-0.1.2/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.680647 mbapy-0.1.2/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.687649 mbapy-0.1.2/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.2/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.2/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.2/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     5036 2023-05-07 14:12:17.000000 mbapy-0.1.2/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.2/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.2/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.2/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.2/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.689649 mbapy-0.1.2/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.2/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.2/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0     9488 2023-06-06 15:58:32.000000 mbapy-0.1.2/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0     2825 2023-06-02 01:55:22.000000 mbapy-0.1.2/mbapy/file.py
--rw-rw-rw-   0        0        0    14671 2023-06-02 01:55:22.000000 mbapy-0.1.2/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.695651 mbapy-0.1.2/mbapy/stats/
--rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.2/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0     4459 2023-06-12 15:10:27.000000 mbapy-0.1.2/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.2/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0      754 2023-04-06 13:40:59.000000 mbapy-0.1.2/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0     9377 2023-05-25 14:57:15.000000 mbapy-0.1.2/mbapy/stats/test.py
--rw-rw-rw-   0        0        0     8922 2023-05-06 08:51:30.000000 mbapy-0.1.2/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2023-06-12 15:19:56.654451 mbapy-0.1.2/mbapy.egg-info/
--rw-rw-rw-   0        0        0     6409 2023-06-12 15:19:56.000000 mbapy-0.1.2/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1258 2023-06-12 15:19:56.000000 mbapy-0.1.2/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 15:19:56.000000 mbapy-0.1.2/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      393 2023-06-12 15:19:56.000000 mbapy-0.1.2/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0      122 2023-06-12 15:19:56.000000 mbapy-0.1.2/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 15:19:56.699653 mbapy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     3190 2023-06-12 15:19:52.000000 mbapy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.346296 mbapy-0.1.3/
+-rw-rw-rw-   0        0        0     1085 2022-10-19 14:16:22.000000 mbapy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2695 2023-06-30 13:37:37.346296 mbapy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1921 2023-06-29 14:51:48.000000 mbapy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.238641 mbapy-0.1.3/mbapy/
+-rw-rw-rw-   0        0        0      731 2023-06-30 04:21:54.000000 mbapy-0.1.3/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2023-06-30 13:36:51.000000 mbapy-0.1.3/mbapy/__version__.py
+-rw-rw-rw-   0        0        0     6204 2023-06-29 14:12:46.000000 mbapy-0.1.3/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.283713 mbapy-0.1.3/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      363 2023-05-25 14:57:15.000000 mbapy-0.1.3/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.286714 mbapy-0.1.3/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.301011 mbapy-0.1.3/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-06-06 15:50:53.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16561 2023-06-07 03:36:12.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2419 2023-06-07 03:14:56.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.308011 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-06-06 15:37:25.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:10.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:35:17.000000 mbapy-0.1.3/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-06-06 15:38:23.000000 mbapy-0.1.3/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    22606 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6379 2023-06-30 02:27:21.000000 mbapy-0.1.3/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1052 2023-05-01 12:18:06.000000 mbapy-0.1.3/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-03-20 16:36:17.000000 mbapy-0.1.3/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13193 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     3877 2023-06-02 01:55:22.000000 mbapy-0.1.3/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.312012 mbapy-0.1.3/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-05-04 14:59:39.000000 mbapy-0.1.3/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-05-25 14:57:15.000000 mbapy-0.1.3/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    11474 2023-06-15 14:59:22.000000 mbapy-0.1.3/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0     7865 2023-06-29 14:14:34.000000 mbapy-0.1.3/mbapy/file.py
+-rw-rw-rw-   0        0        0    14949 2023-06-30 13:01:18.000000 mbapy-0.1.3/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.332018 mbapy-0.1.3/mbapy/stats/
+-rw-rw-rw-   0        0        0      539 2023-04-19 11:56:16.000000 mbapy-0.1.3/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    10820 2023-06-30 10:49:15.000000 mbapy-0.1.3/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2022-12-05 10:10:18.000000 mbapy-0.1.3/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     1281 2023-06-15 15:01:10.000000 mbapy-0.1.3/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    12704 2023-06-30 13:33:59.000000 mbapy-0.1.3/mbapy/stats/test.py
+-rw-rw-rw-   0        0        0    16079 2023-06-15 15:05:25.000000 mbapy-0.1.3/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.246643 mbapy-0.1.3/mbapy.egg-info/
+-rw-rw-rw-   0        0        0     2695 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1488 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      393 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      122 2023-06-30 13:37:37.000000 mbapy-0.1.3/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 13:37:37.346296 mbapy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     3190 2023-06-30 13:37:03.000000 mbapy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 13:37:37.344292 mbapy-0.1.3/test/
+-rw-rw-rw-   0        0        0     1087 2023-06-30 04:25:46.000000 mbapy-0.1.3/test/test_base.py
```

### Comparing `mbapy-0.1.2/LICENSE` & `mbapy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/base.py` & `mbapy-0.1.3/mbapy/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-10-19 22:46:30
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-06-06 23:58:38
+LastEditTime: 2023-06-29 22:03:58
 Description: 
 '''
 import sys
 import time
 from functools import wraps
 
 import numpy as np
@@ -69,27 +69,61 @@
         # attach attributes to instance
         for arg in kwargs:
             setattr(self, arg, kwargs[arg])
         init(self, **kwargs)
     return wrapped_init
 
 def rand_choose_times(choices_range:list[int] = [0,10], times:int = 100):
+    """
+    Generates a random sequence of integers within a given range and 
+    counts the frequency of each number. Returns the most frequent number.
+    
+    :param choices_range: A list of two integers representing the lower and upper bounds of the range. Default is [0,10].
+    :type choices_range: list[int]
+    :param times: An integer representing the number of times the random sequence will be generated. Default is 100.
+    :type times: int
+    :return: An integer representing the most frequent number in the generated sequence.
+    :rtype: int
+    """
     randSeq = np.random.randint(low = choices_range[0], high = choices_range[1]+1, size = [times])
     count = [ np.sum(np.equal(randSeq,i)) for i in range(choices_range[0],choices_range[1]+1) ]
     return np.argmax(np.array(count))
 
+def rand_choose(lst:list, seed = None):
+    """
+    Selects a random element from the given list.
+
+    Parameters:
+        lst (list): The list from which to select a random element.
+        seed (int, optional): The seed value to use for random number generation. Defaults to None.
+
+    Returns:
+        Any: The randomly selected element from the list.
+    """
+    if seed is not None:
+        np.random.seed(seed)
+    return np.random.choice(lst)
+
 def put_err(info:str, ret = None):
     if not __NO_ERR__:
         print(f'\nERR : {sys._getframe().f_code.co_name:s} : {info:s}\n')
     return ret
 def put_log(info:str, head = "log", ret = None):
     print(f'\n{head:s} : {sys._getframe().f_code.co_name:s} : {info:s}\n')
     return ret
 
 def get_time(chr:str = ':')->str:
+    """
+    Returns the current time as a string with a given character replacing the standard colon separator.
+
+    :param chr: The character to replace the ':' separator. Default value is ':'.
+    :type chr: str
+    :return: A string that represents the current time with a given separator replacing the standard colon separator.
+    :rtype: str
+    """
     return time.asctime(time.localtime()).replace(':', chr)
 
 class MyArgs():
     def __init__(self, args:dict) -> None:
         self.args = dict()
         args = self.get_args(args)
     def get_args(self, args:dict, force_update = True, del_origin = False):
@@ -106,14 +140,24 @@
     def toDict(self):
         dic = {}
         for attr in vars(self):
             dic[attr] = getattr(self,attr)
         return dic   
 
 def get_default_for_None(x, deault):
+    """
+    Return the default value when the input value is None.
+
+    Args:
+        x (Any): The input value to be checked.
+        deault (Any): The default value to return if x is None.
+
+    Returns:
+        The input value if it is not None, otherwise the default value.
+    """
     return x if x is not None else deault
 
 def get_wanted_args(defalut_args:dict, kwargs:dict, del_kwargs = True):
     """
     wanted_args:dict with default value
     localVar = locals()
     """
```

### Comparing `mbapy-0.1.2/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.1.3/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.1.3/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/bb.py` & `mbapy-0.1.3/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/data.py` & `mbapy-0.1.3/mbapy/dl_torch/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2023-03-21 00:12:32
-LastEditors: BHM-Bob
-LastEditTime: 2023-05-07 22:12:17
+LastEditors: BHM-Bob 2262029386@qq.com
+LastEditTime: 2023-06-29 23:13:23
 Description: 
 '''
 import torch
 import torch.nn.functional as F
 from torch.utils.data import Dataset
 from torch.utils.data import DataLoader
 
 from .utils import GlobalSettings, Mprint
 
 def denarmalize_img(x, mean = [0.485, 0.456, 0.406], std = [0.229, 0.224, 0.225]):
+    """
+    Denormalizes an image given its pixel values, mean, and standard deviation.
+
+    Args:
+        x (torch.Tensor): The tensor of pixel values of the image.
+        mean (list of floats, optional): The mean pixel value for each channel.
+            Defaults to [0.485, 0.456, 0.406].
+        std (list of floats, optional): The standard deviation of pixel values
+            for each channel. Defaults to [0.229, 0.224, 0.225].
+
+    Returns:
+        torch.Tensor: The denormalized image tensor.
+    """
     mean = torch.tensor(mean).unsqueeze(1).unsqueeze(1)
     std = torch.tensor(std).unsqueeze(1).unsqueeze(1)
     return x * std + mean
 
 class RandomSeqGenerator(object):
     def __init__(self, seqs:torch.Tensor, lables:torch.Tensor, args:GlobalSettings,
                  multiLoads:int = 6, maskRatio:float = 0.3, device:str = 'cpu'):
@@ -56,14 +69,38 @@
         self.x_transformer, self.y_transformer = x_transformer, y_transformer
         
     def __getitem__(self, idx):
         return self.x_transformer(self.x[idx]), self.y_transformer(self.y[idx])
     def __len__(self):
         return self.size
 
+class SubDataSetR(Dataset):
+    """
+    继承Dataset，作为训练时\n
+    接受DataSetRAM分配的数据
+    transformer接受x[idx]和所有的x:list
+    """
+    def __init__(self, args:GlobalSettings, x:list, y:list,
+                 x_transformer:list = None, y_transformer:list = None):
+        super().__init__()
+        self.args = args
+        self.x = x
+        self.y = y
+        self.size = len(x)
+        if x_transformer is None:
+            x_transformer = lambda x : x
+        if y_transformer is None:
+            y_transformer = lambda y : y
+        self.x_transformer, self.y_transformer = x_transformer, y_transformer
+        
+    def __getitem__(self, idx):
+        return self.x_transformer(self.x[idx], self.x), self.y_transformer(self.y[idx], self.x)
+    def __len__(self):
+        return self.size
+
 class DataSetRAM():
     """
     将数据加载到RAM储存并按比例分配生成DataLoader\n
     可以传入各种transformer以满足加载不同数据的需求，亦可以继承该类，使用自定义代码加载self.x和self.labels\n
     Parameters
     ----------
     x: original x, suppose to be a list of paths and so on.
@@ -95,27 +132,25 @@
             
         self.size = len(self.x)
     
     def _check_list(self, x):
         return [x] if not isinstance(x, list) else x
 
     def split(self, divide:list[float],
-              x_transformer:list = None, y_transformer:list = None):
+              x_transformer:list = None, y_transformer:list = None, dataset = SubDataSet):
         """divide : [0, 0.7, 0.9, 1] => train_70% val_20% test_10%"""
         ret = []
         if len(self.y) == 0:
             self.y = [0] * self.size
         x_transformer = [None]*len(divide) if x_transformer is None else x_transformer
         y_transformer = [None]*len(divide) if y_transformer is None else y_transformer
         for idx in range(len(divide) - 1):
             index1 = int(divide[idx  ]*self.size)
             index2 = int(divide[idx+1]*self.size)
             ret.append(
                 DataLoader(
-                    SubDataSet(args = self.args,
-                               x = self.x[index1 : index2],
-                               y = self.y[index1 : index2],
-                               x_transformer = x_transformer[idx],
-                               y_transformer = y_transformer[idx])
+                    dataset(args = self.args,
+                            x = self.x[index1 : index2], y = self.y[index1 : index2],
+                            x_transformer = x_transformer[idx], y_transformer = y_transformer[idx])
                     ,batch_size = self.batch_size, shuffle = True, drop_last=True))
             self.args.mp.mprint(f'dataSet{idx:d} size:{index2-index1:d}')
         return ret
```

### Comparing `mbapy-0.1.2/mbapy/dl_torch/hyper_search.py` & `mbapy-0.1.3/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/loss.py` & `mbapy-0.1.3/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/m.py` & `mbapy-0.1.3/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/optim.py` & `mbapy-0.1.3/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/paper/bb.py` & `mbapy-0.1.3/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/dl_torch/utils.py` & `mbapy-0.1.3/mbapy/dl_torch/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -131,26 +131,42 @@
             if m.weight is not None:
                 nn.init.constant_(m.weight, 1)
             if m.bias is not None:
                 nn.init.constant_(m.bias, 0)
     return model
 
 def adjust_learning_rate(optimizer, now_epoch, args):
-    """Decay the learning rate based on schedule
-    args"""
+    """
+    Adjusts the learning rate of the given optimizer based on the current epoch and arguments.
+
+    Args:
+        optimizer (torch.optim.Optimizer): Optimizer to adjust the learning rate of.
+        now_epoch (int): Current epoch number.
+        args (argparse.Namespace): Parsed command-line arguments.
+
+    Returns:
+        None
+    """
     lr = args.lr
     if args.cos:  # cosine lr schedule
         lr *= 0.5 * (1. + math.cos(math.pi * now_epoch / args.epochs))
     else:  # stepwise lr schedule
         for milestone in args.schedule:
             lr *= 0.1 if now_epoch >= milestone else 1.
     for param_group in optimizer.param_groups:
         param_group['lr'] = lr
 
 def format_secs(sumSecs):
+    """
+    Formats a given number of seconds into hours, minutes, and seconds.
+
+    :param sumSecs: An integer representing the total number of seconds.
+    :return: A tuple containing three integers representing the number of hours,
+             minutes, and seconds respectively.
+    """
     sumHs = int(sumSecs//3600)
     sumMs = int((sumSecs-sumHs*3600)//60)
     sumSs = int(sumSecs-sumHs*3600-sumMs*60)
     return sumHs, sumMs, sumSs
 
 class AverageMeter(object):
     """
@@ -206,28 +222,54 @@
     def update(self, left_tasks:int, just_done_tasks:int = 1):
         used_time = time.time() - self.last_time
         self.last_time = time.time()
         sum_last_time = left_tasks * used_time / just_done_tasks
         return sum_last_time            
             
 def save_checkpoint(epoch, args:GlobalSettings, model, optimizer, loss, other:dict, tailName:str):
+    """
+    Saves a checkpoint of the model and optimizer state, along with other information 
+    such as epoch, loss, and arguments. The checkpoint file is named as 
+    "checkpoint_{tailName:s}_{time.asctime(time.localtime()).replace(':', '-'):s}.pth.tar" 
+    and saved in the directory specified by args.model_root.
+
+    :param epoch: An integer representing the current epoch number.
+    :param args: A GlobalSettings object containing various hyperparameters and settings.
+    :param model: The model whose state needs to be saved.
+    :param optimizer: The optimizer whose state needs to be saved.
+    :param loss: The current loss value.
+    :param other: A dictionary containing any other information that needs to be saved.
+    :param tailName: A string to be used in the checkpoint file name for better identification.
+
+    :return: None
+    """
     state = {
         "epoch": epoch + 1,
         "arch": args.arch,
         "state_dict": model.state_dict(),
         "optimizer": optimizer.state_dict(),
         "loss": loss,
         "args":args.toDict(),
     }
     state.update(other)
     filename = os.path.join(args.model_root,
                             f"checkpoint_{tailName:s}_{time.asctime(time.localtime()).replace(':', '-'):s}.pth.tar")
     torch.save(state, filename)
 
 def resume(args, model, optimizer, other:dict = {}):
+    """
+    Resumes the training from the last checkpoint if it exists, otherwise starts from scratch.
+
+    :param args: Namespace object containing parsed command-line arguments.
+    :param model: Model to be trained.
+    :param optimizer: Optimizer to be used for training.
+    :param other: Optional dictionary containing additional objects to be updated from checkpoint.
+
+    :return: Tuple of the model, optimizer, and old_losses if checkpoint exists, otherwise tuple of model, optimizer, and 0.
+    """
     if args.resume and os.path.isfile(args.resume):
         args.mp.mprint("=> loading checkpoint '{}'".format(args.resume))
         if args.gpu is None:
             checkpoint = torch.load(args.resume)
         else:
             # Map model to be loaded to specified single gpu.
             # loc = "cuda:{}".format(args.gpu)
```

### Comparing `mbapy-0.1.2/mbapy/plot.py` & `mbapy-0.1.3/mbapy/plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import itertools
+from itertools import combinations
 import sys
 from functools import wraps
 from typing import Union
 
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
@@ -10,179 +11,85 @@
 import pandas as pd
 import statsmodels.api as sm
 import seaborn as sns
 from mpl_toolkits import axisartist
 from mpl_toolkits.axes_grid1 import host_subplot
 
 from mbapy.base import get_wanted_args
+from mbapy.stats.df import pro_bar_data, pro_bar_data_R, sort_df_factors, get_df_data
+import mbapy.stats.test as mst
+from mbapy.stats.test import p_value_to_stars
 
 # plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文
 plt.rcParams["font.family"] = 'Times New Roman'
 plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
 colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
 
 def rgb2hex(r, g, b):
   return '#'+('{:02X}' * 3).format(r, g, b)
 def hex2rgb(hex:str):
   return [int(hex[i:i+2], 16) for i in (1, 3, 5)]
 def rgbs2hexs(rgbs:list[tuple[float]]):
+    """
+    Takes a list of RGB tuples and converts them to a list of hexadecimal color codes. 
+    Each RGB tuple must contain three floats between 0 and 1 representing the red, green, and blue 
+    components of the color. Returns a list of hexadecimal color codes as strings.
+    """
     return list(map(lambda x : rgb2hex(*[int(x[i]*255) for i in range(3)]),
                     rgbs))
     
-def get_palette(n:int = 10, mode:Union[None, str] = None) -> list[str]:
+def get_palette(n:int = 10, mode:Union[None, str] = None, return_n = True) -> list[str]:
     """get a seq of hex colors    
     Parameters
     ----------
     n: how many colors required
     mode: kind of colors
         - hls : [default] sns.color_palette('hls', n)
         - green : sum 5 grenns
         - pair : plt.get_cmap('tab20')
         - None : plt.get_cmap('Set1') for n<=9 or plt.get_cmap('Set3') for n<= 12
     """
     assert n >= 1, 'n < 1'
+    ret = None
     if mode == 'hls':
-        return rgbs2hexs(sns.color_palette('hls', n))
+        ret = rgbs2hexs(sns.color_palette('hls', n))
     if n <= 5 and mode == 'green':
-        return ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
+        ret = ['#80ab1c', '#405535', '#99b69b', '#92e4ce', '#72cb87'][0:n]
     elif n <= 9:
-        return rgbs2hexs(plt.get_cmap('Set1').colors)
+        ret = rgbs2hexs(plt.get_cmap('Set1').colors)
     elif n <= 12:
-        return rgbs2hexs(plt.get_cmap('Set3').colors)
+        ret = rgbs2hexs(plt.get_cmap('Set3').colors)
     elif n <= 20 and mode == 'pair':
-        return rgbs2hexs(plt.get_cmap('tab20').colors)
+        ret = rgbs2hexs(plt.get_cmap('tab20').colors)
+    if return_n and ret is not None:
+        ret = ret[:n]
+    return ret
     
-# TODO : not use itertools.product
-def pro_bar_data(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
-    """
-    cacu mean and SE for each combinations of facotors\n
-    data should be like this:\n
-    | factor1 | factor2 | y1 | y2 |...\n
-    |  f1_1   |   f2_1  |2.1 |-2  |...\n
-    after process\n
-    | factor1 | factor2 | y1(mean) | y1_SE(SE) | y1_N(sum_data) |...\n
-    |  f1_1   |   f2_1  |2.1       |   -2      |   32           |...\n
-    kwargs:
-        min_sample_N:int : min N threshold(>=)
-    """
-    # kwargs
-    min_sample_N = 1 if 'min_sample_N' not in kwargs else kwargs['min_sample_N']
-    assert min_sample_N > 0, 'min_sample_N <= 0'
-    # pro
-    if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]
-    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-    ndf = [factors.copy()]
-    for tag in tags:
-        ndf[0] += [tag, tag+'_SE', tag+'_N']
-    for factorCombi in itertools.product(*factor_contents):
-        factorMask = np.array(df[factors[0]] == factorCombi[0])
-        for i in range(1, len(factors)):
-            factorMask &= np.array(df[factors[i]] == factorCombi[i])
-        if factorMask.sum() >= min_sample_N:
-            line = []
-            for idx, tag in enumerate(tags):
-                values = np.array(df.loc[factorMask, [tag]])
-                line.append(values.mean())
-                if values.shape[0] > 1:
-                    line.append(values.std(ddof = 1)/np.sqrt(values.shape[0]))
-                else:
-                    line.append(np.NaN)
-                line.append(values.shape[0])
-            ndf.append(list(factorCombi) + line)
-    return pd.DataFrame(ndf[1:], columns=ndf[0])
-
-def pro_bar_data_R(factors:list[str], tags:list[str], df:pd.DataFrame, suffixs:list[str], **kwargs):
-    """
-    wrapper\n
-    @pro_bar_data_R(['solution', 'type'], ['root', 'leaf'], ndf)\n
-    def plot_func(values, **kwargs):
-        return produced vars in list format whose length equal to len(suffix)
-    """
-    def ret_wrapper(core_func):
-        def core_wrapper(**kwargs):
-            nonlocal tags
-            if len(tags) == 0:
-                tags = list(df.columns)[len(factors):]
-            factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-            ndf = [factors.copy()]
-            for tag in tags:
-                for suffix in suffixs:
-                    ndf[0] += [tag+suffix]
-            for factorCombi in itertools.product(*factor_contents):
-                factorMask = np.array(df[factors[0]] == factorCombi[0])
-                for i in range(1, len(factors)):
-                    factorMask &= np.array(df[factors[i]] == factorCombi[i])
-                if(factorMask.sum() > 0):
-                    line = []
-                    for idx, tag in enumerate(tags):
-                        values = np.array(df.loc[factorMask, [tag]])
-                        ret_line = core_func(values)
-                        assert len(ret_line) == len(suffixs), 'length of return value of core_func != len(suffixs)'
-                        line += ret_line
-                    ndf.append(list(factorCombi) + line)
-            return pd.DataFrame(ndf[1:], columns=ndf[0])
-        return core_wrapper
-    return ret_wrapper
-
-def get_df_data(factors:dict[str, list[str]], tags:list[str], df:pd.DataFrame,
-                include_factors:bool = True):
-    #sub_df = ndf.loc[(ndf['size'] == size1) & (ndf['light'] == light1), ['c', 'w', 'SE']]
-    #sub_df = get_df_data([{'size':[size1], 'light':[light1]}, ['c', 'w', 'SE'])
-    def update_mask(mask, other:np.ndarray, method:str = '&'):
-        return other if mask is None else (mask&other if method == '&' else mask|other)
-    if len(tags) == 0:
-        tags = list(set(df.columns.to_list())-set(factors.keys()))
-    if include_factors:
-        tags = list(factors.keys()) + tags
-    mask = None
-    for factor_name in factors:
-        sub_mask = None
-        if len(factors[factor_name]) == 0:
-            # factors[factor_name] asigned with [], get all sub factors
-            factors[factor_name] = df[factor_name].unique().tolist()
-        for sub_factor in factors[factor_name]:
-            sub_mask = update_mask(sub_mask, np.array(df[factor_name] == sub_factor), '|')
-        mask = update_mask(mask, sub_mask, '&')
-    return df.loc[mask, tags]
-
-def sort_df_factors(factors:list[str], tags:list[str], df:pd.DataFrame):
-    """UnTested
-    sort each combinations of facotors\n
-    data should be like this:\n
-    | factor1 | factor2 | y1 | y2 |...\n
-    |  f1_1   |   f2_1  |2.1 |-2  |...\n
-    |  f1_1   |   f2_2  |2.1 |-2  |...\n
-    ...\n
-    after sort if given facotors=['factor2', 'factor1']\n
-    | factor2 | factor1 | y1 | y2 |...\n
-    |  f2_1   |   f1_1  |2.1 |-2  |...\n
-    |  f2_1   |   f1_2  |2.1 |-2  |...\n
-    ...\n
-    """
-    if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]
-    factor_contents:list[list[str]] = [ df[f].unique().tolist() for f in factors ]
-    ndf = [factors.copy()]
-    ndf[0] += tags
-    for factorCombi in itertools.product(*factor_contents):
-        factorMask = df[factors[0]] == factorCombi[0]
-        for i in range(1, len(factors)):
-            factorMask &= df[factors[i]] == factorCombi[i]
-        ndf.append(list(factorCombi) + np.array(df.loc[factorMask, tags].values))
-    return pd.DataFrame(ndf[1:], columns=ndf[0])
-
 class AxisLable():
     def __init__(self, name:str, hold_space:int = 1) -> None:
         self.name = name
         self.hold_space = hold_space
     def add_space(self, space:int = 1):
         self.hold_space += space
 
 def pro_hue_pos(factors:list[str], df:pd.DataFrame, width:float, bar_space:float):
+    """
+    Returns the x-axis labels and positions of the bars for a plot with multiple categorical variables.
+    
+    :param factors: A list of column names in the DataFrame to group by.
+    :type factors: list[str]
+    :param df: The input DataFrame.
+    :type df: pd.DataFrame
+    :param width: The width of each bar.
+    :type width: float
+    :param bar_space: The space between bars.
+    :type bar_space: float
+    :return: A tuple containing a list of AxisLable objects for each axis and a list of positions for each bar.
+    :rtype: tuple(list[AxisLable], list[float])
+    """
     xlabels, fc_old, pos = [ [] for _ in range(len(factors))], '', []
     for f_i, f in enumerate(factors):
         for fc_i, fc in enumerate(df[f]):
             if fc != fc_old:
                 xlabels[f_i].append(AxisLable(fc))
                 fc_old = fc
             else:
@@ -211,43 +118,58 @@
     tags:[stack_low_y, stack_medium_y, ...] or just one
     df:df from pro_bar_data or sort_df_factors
         kwargs:
     width = 0.4
     bar_space = 0.2
     xrotations = [0]*len(factors)
     colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
+    hatchs:['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
+    labels:None,
+    font_size:None, 
     offset = [(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]
     """
     ax1 = host_subplot(111, axes_class=axisartist.Axes)
     
     if len(tags) == 0:
-        tags = list(df.columns)[len(factors):]    
+        tags = list(df.columns)[len(factors):]
     args = get_wanted_args({'width':0.4, 'bar_space':0.2, 'xrotations':[0]*len(factors),
                             'colors':plt.rcParams['axes.prop_cycle'].by_key()['color'],
-                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))]},
-                            kwargs, locals())
-    args.xrotations.append(0)    
+                            'hatchs':['-', '+', 'x', '\\', '*', 'o', 'O', '.'],
+                            'font_size':None,
+                            'labels':None,
+                            'offset':[(i+1)*(plt.rcParams['font.size']+8) for i in range(len(factors))],
+                            'edgecolor':'white'},
+                            kwargs)
+    args.xrotations.append(0)
     xlabels, pos = pro_hue_pos(factors, df, args.width, args.bar_space)
     bottom = kwargs['bottom'] if 'bottom' in kwargs else np.zeros(len(pos[0]))
     
     for yIdx, yName in enumerate(tags):
-        ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=yName,
-                edgecolor='white', color=args.colors[yIdx])
+        if args.labels is not None:
+            label = args.labels[yIdx]
+        else:
+            label = yName
+        ax1.bar(pos[0], df[yName], width = args.width, bottom = bottom, label=label,
+                edgecolor=args.edgecolor, color=args.colors[yIdx])
         bottom += df[yName]
     ax1.set_xlim(0, pos[0][-1]+args.bar_space+args.width/2)
     ax1.set_xticks(pos[0], [l.name for l in xlabels[0]])
     plt.setp(ax1.axis["bottom"].major_ticklabels, rotation=args.xrotations[0])
+    if args.font_size is not None:
+        plt.setp(ax1.axis["bottom"].major_ticklabels, fontsize=args.font_size[0])
     
     axs = []
     for idx, sub_pos in enumerate(pos[1:]):
         axs.append(ax1.twiny())
         axs[-1].set_xticks(sub_pos, [l.name for l in xlabels[idx+1]])
         new_axisline = axs[-1].get_grid_helper().new_fixed_axis
         axs[-1].axis["bottom"] = new_axisline(loc="bottom", axes=axs[-1], offset=(0, -args.offset[idx]))
         plt.setp(axs[-1].axis["bottom"].major_ticklabels, rotation=args.xrotations[idx+1])
+        if args.font_size is not None:
+            plt.setp(axs[-1].axis["bottom"].major_ticklabels, fontsize=args.font_size[idx+1])
         axs[-1].axis["top"].major_ticks.set_ticksize(0)
         # TODO : do not work
         axs[-1].axis["right"].major_ticks.set_ticksize(0)
     
     return np.array(pos[0]), ax1
 
 def plot_positional_hue(factors:list[str], tags:list[str], df:pd.DataFrame, **kwargs):
@@ -291,14 +213,33 @@
                 # TODO : do not work
                 axs[-1].axis["right"].major_ticks.set_ticksize(0)            
             return np.array(pos[0]), ax1
         return core_wrapper
     return ret_wrapper
 
 def qqplot(tags:list[str], df:pd.DataFrame, figsize = (12, 6), nrows = 1, ncols = 1, **kwargs):
+    """
+    Generates a QQPlot for each specified tag in the given DataFrame using statsmodels' qqplot function.
+    
+    :param tags: A list of strings containing the tags to be plotted.
+    :type tags: list[str]
+    :param df: A pandas DataFrame containing the data to be plotted.
+    :type df: pd.DataFrame
+    :param figsize: A tuple containing the size of the figure to be plotted, defaults to (12,6).
+    :type figsize: tuple(int, int)
+    :param nrows: The number of rows in the plot grid, defaults to 1.
+    :type nrows: int
+    :param ncols: The number of columns in the plot grid, defaults to 1.
+    :type ncols: int
+    :param **kwargs: Additional keyword arguments to be passed to the plot.
+    :type **kwargs: dict
+    
+    :return: None
+    :rtype: None
+    """
     axs = []
     fig = plt.figure(figsize = (12, 6))
     for fig_idx in range(1, ncols*nrows+1):
         axs.append(fig.add_subplot(nrows, ncols, fig_idx))
         if 'xlim' in kwargs:
             axs[-1].set_xlim(kwargs['xlim'])
         if 'ylim' in kwargs:
@@ -310,10 +251,73 @@
         if 'tick_size' in kwargs:
             axs[-1].tick_params(labelsize = kwargs['tick_size'])
         if 'label_size' in kwargs:
             axs[-1].set_xlabel('Theoretical Quantiles', fontsize = kwargs['label_size'])
             axs[-1].set_ylabel('Sample Quantiles', fontsize = kwargs['label_size'])
             
 def save_show(path:str, dpi = 300, bbox_inches = 'tight'):
+    """
+    Saves and shows the current figure.
+
+    :param path: A string representing the file path to save the figure.
+    :param dpi: An integer representing the resolution in dots per inch of the saved figure. Default is 300.
+    :param bbox_inches: A string or a Bbox object representing the portion of the figure to be saved in inches. Default is 'tight'.
+    """
     plt.tight_layout()
     plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
-    plt.show()
+    plt.show()
+    
+def plot_turkey(means, std_errs, tukey_results):
+    """
+    Plot a bar chart showing the means of different groups along with the standard errors.
+
+    Parameters:
+    - means: A list of mean values for each group.
+    - std_errs: A list of standard errors for each group.
+    - tukey_results: The Tukey's test results object.
+
+    Returns:
+    - The current `Axes` instance.
+
+    This function plots a bar chart using the given mean values and standard errors. It also marks the groups with significant differences based on the Tukey's test results.
+    For each combination of groups, the function checks if the corresponding Tukey's test result indicates a significant difference. If so, it plots a horizontal line at the maximum height, vertical lines at the endpoints, and places a text label with stars indicating the p-value of the difference.
+    """
+    x = np.arange(len(means))
+    plt.bar(x, means, yerr=std_errs, capsize=5)
+
+    combins = np.array(list(combinations(range(len(means)), 2)))
+    height = max(means) + max(std_errs)
+    min_height = 0.05 * height
+    endpoint_height = [height - 0.05 * min_height, height + 0.05 * min_height]
+    for i, combination in enumerate(combins):
+        if tukey_results.reject[i]:
+            plt.plot(combination, [height, height], color='black')
+            plt.plot([combination[0], combination[0]], endpoint_height, color='black')
+            plt.plot([combination[1], combination[1]], endpoint_height, color='black')
+            plt.text(np.mean(combination), height,
+                     p_value_to_stars(tukey_results.pvalues[i]), ha='center')
+            height += min_height
+
+    plt.xticks(x, tukey_results.groupsunique)
+    return plt.gca()
+
+if __name__ == '__main__':
+    """dev code"""
+    df = pd.read_excel('./data/plot.xlsx', sheet_name='MWM')
+    df['Animal Type'] = df['Animal Type'].astype('str')
+    model = mst.multicomp_turkeyHSD({'Animal Type':[]}, 'Duration', df)
+    result = mst.turkey_to_table(model)
+    print(result)
+    sub_df = get_df_data({'Animal Type':[]}, ['Duration'], df)
+    sub_df = pro_bar_data(['Animal Type'], ['Duration'], sub_df)
+    plot_turkey(sub_df['Duration'], sub_df['Duration_SE'], model)
+    plt.show()
+    
+    df = pd.DataFrame({'Month': [5, 5, 6, 6, 7, 7, 8, 8, 9, 9],
+                       'Ozone': [23.61538, 22.22445, 29.44444, 18.20790, 59.11538, 31.63584, 59.96154, 39.68121, 31.44828, 24.14182]})
+    model = mst.multicomp_turkeyHSD({'Month':[]}, 'Ozone', df)
+    result = mst.turkey_to_table(model)
+    print(result)
+    sub_df = pro_bar_data(['Month'], ['Ozone'], df)
+    plot_turkey(sub_df['Ozone'], sub_df['Ozone_SE'], model)
+    plt.show()
+
```

### Comparing `mbapy-0.1.2/mbapy/stats/__init__.py` & `mbapy-0.1.3/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy/stats/geography.py` & `mbapy-0.1.3/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.1.2/mbapy.egg-info/SOURCES.txt` & `mbapy-0.1.3/mbapy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,21 @@
 mbapy/dl_torch/data.py
 mbapy/dl_torch/hyper_search.py
 mbapy/dl_torch/loss.py
 mbapy/dl_torch/m.py
 mbapy/dl_torch/optim.py
 mbapy/dl_torch/utils.py
 mbapy/dl_torch/arch/__init__.py
+mbapy/dl_torch/arch/CL/__init__.py
+mbapy/dl_torch/arch/CL/builder.py
+mbapy/dl_torch/arch/CL/trainer.py
+mbapy/dl_torch/arch/CLIP/__init__.py
+mbapy/dl_torch/arch/CLIP/builder.py
+mbapy/dl_torch/arch/CLIP/trainer.py
 mbapy/dl_torch/paper/__init__.py
 mbapy/dl_torch/paper/bb.py
 mbapy/stats/__init__.py
 mbapy/stats/df.py
 mbapy/stats/geography.py
 mbapy/stats/reg.py
-mbapy/stats/test.py
+mbapy/stats/test.py
+test/test_base.py
```

### Comparing `mbapy-0.1.2/setup.py` & `mbapy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-06-12 23:19:32
+LastEditTime: 2023-06-30 21:37:03
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 """
 
@@ -106,8 +106,8 @@
     install_requires=requires,
 )
 
 # pip install .
 
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.1.1.tar.gz
+# twine upload dist/mbapy-0.1.3.tar.gz
```

