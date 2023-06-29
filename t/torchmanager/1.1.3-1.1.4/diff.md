# Comparing `tmp/torchmanager-1.1.3.tar.gz` & `tmp/torchmanager-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager-1.1.3.tar", max compression
+gzip compressed data, was "torchmanager-1.1.4.tar", max compression
```

## Comparing `torchmanager-1.1.3.tar` & `torchmanager-1.1.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1318 2023-04-21 19:45:23.217167 torchmanager-1.1.3/LICENSE
--rw-r--r--   0        0        0      616 2023-05-26 14:45:47.094692 torchmanager-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      281 2023-05-26 13:57:53.914350 torchmanager-1.1.3/torchmanager/__init__.py
--rw-r--r--   0        0        0    11052 2023-05-26 13:57:53.914710 torchmanager-1.1.3/torchmanager/basic.py
--rw-r--r--   0        0        0      658 2023-05-26 13:57:53.915031 torchmanager-1.1.3/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4255 2023-05-26 13:57:53.915310 torchmanager-1.1.3/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-05-26 13:57:23.129146 torchmanager-1.1.3/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-05-26 13:57:23.129390 torchmanager-1.1.3/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-05-26 13:57:23.129552 torchmanager-1.1.3/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4846 2023-05-26 13:57:53.915619 torchmanager-1.1.3/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-05-26 13:57:23.129973 torchmanager-1.1.3/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2440 2023-05-26 13:57:53.915840 torchmanager-1.1.3/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      963 2023-05-26 13:57:53.916340 torchmanager-1.1.3/torchmanager/compatibility.py
--rw-r--r--   0        0        0       85 2023-05-26 13:57:23.131070 torchmanager-1.1.3/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-26 13:57:53.916733 torchmanager-1.1.3/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2236 2023-05-26 13:57:53.917130 torchmanager-1.1.3/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      171 2023-05-26 13:57:53.917364 torchmanager-1.1.3/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5386 2023-05-26 13:57:23.132661 torchmanager-1.1.3/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1044 2023-05-26 13:57:53.917665 torchmanager-1.1.3/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     7061 2023-05-26 13:57:53.917950 torchmanager-1.1.3/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     2381 2023-05-26 13:57:53.918243 torchmanager-1.1.3/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      234 2023-05-26 13:57:53.918541 torchmanager-1.1.3/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     3272 2023-05-26 13:57:53.918835 torchmanager-1.1.3/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     2546 2023-05-26 13:57:53.919126 torchmanager-1.1.3/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     2440 2023-05-26 13:57:53.919427 torchmanager-1.1.3/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     4000 2023-05-26 13:57:53.919829 torchmanager-1.1.3/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     9401 2023-05-26 13:57:53.920555 torchmanager-1.1.3/torchmanager/testing.py
--rw-r--r--   0        0        0      191 2023-05-26 13:57:53.920853 torchmanager-1.1.3/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-05-26 13:57:23.135892 torchmanager-1.1.3/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0     2037 2023-05-26 13:57:53.922149 torchmanager-1.1.3/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    14893 2023-05-26 13:57:53.922553 torchmanager-1.1.3/torchmanager/training.py
--rw-r--r--   0        0        0      443 2023-05-26 13:57:53.922922 torchmanager-1.1.3/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      114 2023-05-26 13:57:53.923187 torchmanager-1.1.3/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     5587 2023-05-26 13:57:53.923476 torchmanager-1.1.3/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-05-26 13:57:23.137865 torchmanager-1.1.3/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-05-26 13:57:23.138096 torchmanager-1.1.3/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-05-26 13:57:23.138227 torchmanager-1.1.3/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-05-26 13:57:23.138467 torchmanager-1.1.3/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     2728 2023-05-26 13:57:53.923701 torchmanager-1.1.3/torchmanager_core/protocols.py
--rw-r--r--   0        0        0      204 2023-05-26 13:57:23.138928 torchmanager-1.1.3/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5253 2023-05-26 13:57:53.924003 torchmanager-1.1.3/torchmanager_core/version.py
--rw-r--r--   0        0        0      126 2023-05-26 13:57:53.924253 torchmanager-1.1.3/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-05-26 13:57:23.140532 torchmanager-1.1.3/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-06-12 21:40:08.180158 torchmanager-1.1.4/LICENSE
+-rw-r--r--   0        0        0      616 2023-06-29 21:59:25.541911 torchmanager-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-06-29 21:58:18.783925 torchmanager-1.1.4/torchmanager/__init__.py
+-rw-r--r--   0        0        0    11076 2023-06-29 21:59:25.543096 torchmanager-1.1.4/torchmanager/basic.py
+-rw-r--r--   0        0        0      659 2023-06-29 21:59:25.543478 torchmanager-1.1.4/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4248 2023-06-29 21:59:25.543792 torchmanager-1.1.4/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4686 2023-06-29 21:59:25.544093 torchmanager-1.1.4/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3522 2023-06-29 21:59:25.548795 torchmanager-1.1.4/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1984 2023-06-29 21:59:25.549314 torchmanager-1.1.4/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4854 2023-06-29 21:59:25.549619 torchmanager-1.1.4/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2238 2023-06-29 21:59:25.549956 torchmanager-1.1.4/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2454 2023-06-29 21:59:25.550248 torchmanager-1.1.4/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      963 2023-06-29 21:58:18.786227 torchmanager-1.1.4/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       85 2023-06-28 18:44:00.539650 torchmanager-1.1.4/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6962 2023-06-29 21:58:18.786430 torchmanager-1.1.4/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2236 2023-06-29 21:58:18.786607 torchmanager-1.1.4/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      171 2023-06-29 21:58:18.786797 torchmanager-1.1.4/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5386 2023-06-29 21:58:18.786993 torchmanager-1.1.4/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1044 2023-06-29 21:58:18.787165 torchmanager-1.1.4/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     7061 2023-06-29 21:58:18.787416 torchmanager-1.1.4/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     2381 2023-06-29 21:58:18.787572 torchmanager-1.1.4/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      234 2023-06-29 21:58:18.787736 torchmanager-1.1.4/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     3272 2023-06-29 21:58:18.787899 torchmanager-1.1.4/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     2546 2023-06-29 21:58:18.788079 torchmanager-1.1.4/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     2633 2023-06-29 21:59:25.550538 torchmanager-1.1.4/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     4000 2023-06-29 21:58:18.788645 torchmanager-1.1.4/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     9401 2023-06-29 21:58:18.789063 torchmanager-1.1.4/torchmanager/testing.py
+-rw-r--r--   0        0        0      191 2023-06-29 21:58:18.789324 torchmanager-1.1.4/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4986 2023-06-29 21:58:18.789722 torchmanager-1.1.4/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0     2037 2023-06-29 21:58:18.789979 torchmanager-1.1.4/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    14893 2023-06-29 21:58:18.790239 torchmanager-1.1.4/torchmanager/training.py
+-rw-r--r--   0        0        0      443 2023-06-29 21:58:18.790431 torchmanager-1.1.4/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      114 2023-06-29 21:58:18.790649 torchmanager-1.1.4/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     5587 2023-06-29 21:58:18.790848 torchmanager-1.1.4/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-06-28 18:44:00.542743 torchmanager-1.1.4/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-06-28 18:44:00.542862 torchmanager-1.1.4/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-29 21:58:18.791030 torchmanager-1.1.4/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-06-28 18:44:00.543066 torchmanager-1.1.4/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     2728 2023-06-29 21:58:18.791203 torchmanager-1.1.4/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0      204 2023-06-28 18:44:00.543293 torchmanager-1.1.4/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     7356 2023-06-29 21:59:25.550792 torchmanager-1.1.4/torchmanager_core/version.py
+-rw-r--r--   0        0        0      163 2023-06-29 21:59:25.551054 torchmanager-1.1.4/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-28 18:44:00.543729 torchmanager-1.1.4/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 torchmanager-1.1.4/PKG-INFO
```

### Comparing `torchmanager-1.1.3/LICENSE` & `torchmanager-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/pyproject.toml` & `torchmanager-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "torchmanager"
-version = "1.1.3"
-description = "PyTorch Training Manager v1.1.3"
+version = "1.1.4"
+description = "PyTorch Training Manager v1.1.4"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
```

### Comparing `torchmanager-1.1.3/torchmanager/basic.py` & `torchmanager-1.1.4/torchmanager/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,19 +215,19 @@
         Convert the current manager to a checkpoint
 
         - Returns: A `Checkpoint` with its model as the current manager
         """
         ckpt = Checkpoint(self)
         return ckpt
 
-    def unpack_data(self, data: Collection) -> Tuple[Any, Any]:
+    def unpack_data(self, data: Collection[Any]) -> Tuple[Any, Any]:
         """
         Unpacks data to input and target
 
         - Parameters:
-            - data: `Any` kind of data object
+            - data: A `Collection` of `Any` kind of data objects
         - Returns: A `tuple` of `Any` kind of input and `Any` kind of target
         """
         if len(data) >= 2:
             return tuple(data)
         else:
             return NotImplemented
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/__init__.py` & `torchmanager-1.1.4/torchmanager/callbacks/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     from .tensorboard import TensorBoard
 except:
     from torchmanager_core import view
     view.warnings.warn("Tensorboard dependency is not installed, install it to use `Experiment` and `TensorBoard` callbacks.", ImportWarning)
 
     Experiment = NotImplemented
     TensorBoard = NotImplemented
-    pass
+    pass
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/callback.py` & `torchmanager-1.1.4/torchmanager/callbacks/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from torchmanager_core import abc, torch
 from torchmanager_core.protocols import Frequency
 from torchmanager_core.typing import Any, Dict, Optional
 
+
 class Callback:
     """An empty basic training callback"""
 
     def on_batch_end(self, batch: int, summary: Dict[str, float] = {}) -> None:
         """
         The callback when batch ends
 
@@ -124,14 +125,14 @@
             self._update(result)
             self.current_step += 1
 
     @abc.abstractmethod
     def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Any:
         """
         Abstract method to step the callback
-        
+
         - Parameters:
             - summary: A `dict` of training summary with name in `str` and value in `float`
             - val_summary: An optional `dict` of validation summary with name in `str` and value in `float`
         - Returns: An `Any` type of result for the new step
         """
         return NotImplemented
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/ckpt.py` & `torchmanager-1.1.4/torchmanager/callbacks/ckpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
 from ..train import Checkpoint as Ckpt
 from .callback import Callback
 
 T = TypeVar('T', bound=StateDictLoadable)
 
+
 class _Checkpoint(Callback, Generic[T]):
     """
     The callback to save the last checkpoint during training
 
     * extends: `.Callback
 
     - Properties:
@@ -43,40 +44,43 @@
         super().__init__()
         self.__checkpoint = Ckpt(model, **kwargs)
         self.ckpt_path = os.path.normpath(ckpt_path)
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
         self.checkpoint.save(epoch, self.ckpt_path)
 
+
 class LastCheckpoint(_Checkpoint[T]):
     """
     Last checkpoint with frequency control support
 
     * extends: `_Checkpoint`
-    
+
     - Properties:
         - freq: An `int` of checkpoint epoch frequency
     """
     __freq: int
 
     @property
     def freq(self) -> int:
         return self.__freq
-    
+
     @freq.setter
     def freq(self, f: int) -> None:
         assert f > 0, _raise(ValueError(f"Frequency must be a positive number, got {f}. "))
         self.__freq = f
 
     def __init__(self, model: T, ckpt_path: str, freq: int = 1, **kwargs: Any) -> None:
         super().__init__(model, ckpt_path, **kwargs)
         self.freq = freq
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = ...) -> None:
-        if epoch % self.freq == 0: super().on_epoch_end(epoch, summary, val_summary)
+        if epoch % self.freq == 0:
+            super().on_epoch_end(epoch, summary, val_summary)
+
 
 class BestCheckpoint(_Checkpoint[T]):
     """
     The callback to save the latest checkpoint for each epoch
 
     * extends: `_Checkpoint`
 
@@ -87,15 +91,15 @@
     """
     # properties
     best_score: float
     load_best: bool
     monitor: str
     monitor_type: MonitorType
 
-    def __init__(self, monitor: str, model: T, ckpt_path: str, load_best: bool = False, monitor_type: MonitorType=MonitorType.MAX, **kwargs: Any) -> None:
+    def __init__(self, monitor: str, model: T, ckpt_path: str, load_best: bool = False, monitor_type: MonitorType = MonitorType.MAX, **kwargs: Any) -> None:
         """
         Constructor
 
         - Parameters:
             - monitor: A `str` of monitored metric
             - monitor_type: A `MonitorType` of either `MIN` of `MAX` mode for the best model
         """
@@ -122,10 +126,13 @@
         if self.load_best:
             # load checkpoint
             best_ckpt: Ckpt[StateDictLoadable] = Ckpt.from_saved(self.ckpt_path)
 
             # load to model
             if isinstance(best_ckpt.model, ModelContainer):
                 ckpt_model = best_ckpt.model.model
-            else: ckpt_model = best_ckpt.model
-            try: model.load_state_dict(ckpt_model.state_dict())
-            except: raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
+            else:
+                ckpt_model = best_ckpt.model
+            try:
+                model.load_state_dict(ckpt_model.state_dict())
+            except:
+                raise TypeError(f"Reload best checkpoint to model failed: supposed to have {type(model)} in checkpoint, got {type(ckpt_model)}.")
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/dynamic.py` & `torchmanager-1.1.4/torchmanager/callbacks/dynamic.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from torchmanager_core.protocols import Frequency, SummaryWriteble, Weighted
 from torchmanager_core.typing import Any, Callable, Generic, Optional, SupportsFloat, TypeVar
 
 from .callback import FrequencyCallback
 
 W = TypeVar('W', bound=Weighted)
 
+
 class DynamicWeight(FrequencyCallback, abc.ABC, Generic[W]):
     '''
     An abstract dynamic weight callback that set weight dynamically
 
     * extends: `.callback.FrequencyCallback`
     * abstract class that needs implementation of `step` method
     '''
@@ -54,18 +55,19 @@
             w = self._weighted.weight
             result = {'train': w}
             self._writer.add_scalars(self._key, result, epoch)
 
         # update
         super().on_epoch_end(epoch, *args, **kwargs)
 
+
 class LambdaDynamicWeight(DynamicWeight[W], Generic[W]):
     '''
     A dynamic weight callback that set weight dynamically with lambda function
-    
+
     * extends: `DynamicWeight`
 
     Targeting to any object that performs to `.protocol.Weighted` protocol:
     >>> from torchmanager import losses
     >>> loss_fn = losses.Loss(...) # where `torchmanager.losses.Loss` performs to `.protocols.Weighted` protocol
 
     Passing defined functions into the `DynamicWeight` callback:
@@ -87,8 +89,8 @@
     def _lambda_fn(self) -> Callable[[int], Any]: return self.__lambda_fn
 
     def __init__(self, fn: Callable[[int], Any], weighted: W, freq: Frequency = Frequency.EPOCH, writer: Optional[SummaryWriteble] = None, name: Optional[str] = None) -> None:
         super().__init__(weighted, freq, writer, name)
         self.__lambda_fn = fn
 
     def step(self, *args: Any, **kwargs: Any) -> Any:
-        return self._lambda_fn(self.current_step)
+        return self._lambda_fn(self.current_step)
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/early_stop.py` & `torchmanager-1.1.4/torchmanager/callbacks/early_stop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from torchmanager_core import errors, sys
 from torchmanager_core.typing import Dict, List, Optional
 
 from .ckpt import Callback, MonitorType
 
+
 class EarlyStop(Callback):
     '''
     The early stop callback that raises `StopTraining` error during the training if monitored metric not improved for several steps
 
     - Properties:
         - monitor: A `str` of monitored metric
         - monitor_type: A `MonitorType` of either `MIN` of `MAX` mode for the best model
@@ -26,15 +27,21 @@
         self.__metrics = [sys.float_info.min if monitor_type == MonitorType.MAX else sys.float_info.max]
         self.monitor = monitor
         self.monitor_type = monitor_type
         self.steps = steps
 
     def on_epoch_end(self, epoch: int, summary: Dict[str, float] = ..., val_summary: Optional[Dict[str, float]] = None) -> None:
         # load monitoring value
-        if val_summary is not None: summary = val_summary
+        summary = val_summary if val_summary is not None else summary
         monitoring_value = summary[self.monitor]
 
         # compare with recorded metrics
-        max_value = max(self.__metrics)
-        if monitoring_value < max_value and len(self._metrics) >= self.steps: raise errors.StopTraining(epoch)
-        elif len(self._metrics) >= self.steps: self._metrics.pop()
-        self._metrics.insert(0, monitoring_value)
+        value = self._metrics[0]
+        if self.monitor_type == MonitorType.MAX and monitoring_value <= value and len(self._metrics) > self.steps:
+            raise errors.StopTraining(epoch)
+        elif self.monitor_type == MonitorType.MAX and monitoring_value > value:
+            self._metrics.clear()
+        elif self.monitor_type == MonitorType.MIN and monitoring_value >= value and len(self._metrics) > self.steps:
+            raise errors.StopTraining(epoch)
+        elif self.monitor_type == MonitorType.MIN and monitoring_value < value:
+            self._metrics.clear()
+        self._metrics.append(monitoring_value)
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/experiment.py` & `torchmanager-1.1.4/torchmanager/callbacks/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .callback import Callback
 from .ckpt import BestCheckpoint, LastCheckpoint
 from .tensorboard import TensorBoard
 
 T = TypeVar('T', bound=StateDictLoadable)
 
+
 class Experiment(Callback, Generic[T]):
     """
     The tensorboard callback that wraps last and best checkpoints in `checkpoints` folder by `last.model` and `best_*.model` with tensorboard logs in `data` folder together into a wrapped *.exp file
 
     * extends: `.callback.Callback`
     * requires: `tensorboard` package
 
@@ -21,32 +22,33 @@
         - last_ckpt: A `.ckpt.LastCheckpoint` callback that records the last checkpoint
         - tensorboard: A `.ckpt.TensorBoard` callback that records data to tensorboard
     """
     best_ckpts: List[BestCheckpoint[T]]
     last_ckpt: LastCheckpoint[T]
     tensorboard: TensorBoard
 
-    def __init__(self, experiment: str, model: T, monitors: Union[Dict[str, MonitorType], List[str]]={}, show_verbose: bool = True) -> None:
+    def __init__(self, experiment: str, model: T, monitors: Union[Dict[str, MonitorType], List[str]] = {}, show_verbose: bool = True) -> None:
         """
         Constructor
 
         - Parameters:
             - experiment: A `str` of target folder for the experiment
             - model: A target model to be tracked during experiment in `T`
             - monitors: A `list` of metric name if all monitors are using `MonitorType.MAX` to track, or `dict` of metric name to be tracked for the best checkpoint in `str` and the `.ckpt.MonitorType` to track as values
             - show_verbose: A `bool` flag of if showing loggins in console
         """
         # call super constructor
         experiment = os.path.normpath(experiment)
-        if not experiment.endswith(".exp"): experiment += ".exp"
+        if not experiment.endswith(".exp"):
+            experiment += ".exp"
         experiment_dir = os.path.join("experiments", experiment)
         os.makedirs(experiment_dir, exist_ok=True)
         log_dir = os.path.join(experiment_dir, "data")
         ckpt_path = os.path.join(experiment_dir, "checkpoints")
-        
+
         # initial checkpoints
         self.best_ckpts = []
         last_ckpt_path = os.path.join(ckpt_path, "last.model")
         self.last_ckpt = LastCheckpoint(model, last_ckpt_path)
         self.tensorboard = TensorBoard(log_dir)
 
         # initialize best checkpoints according to monitors
@@ -98,8 +100,8 @@
         self.last_ckpt.on_epoch_end(*args, **kwargs)
         self.tensorboard.on_epoch_end(*args, **kwargs)
 
     def on_epoch_start(self, *args: Any, **kwargs: Any) -> None:
         for best_ckpt in self.best_ckpts:
             best_ckpt.on_epoch_start(*args, **kwargs)
         self.last_ckpt.on_epoch_start(*args, **kwargs)
-        self.tensorboard.on_epoch_start(*args, **kwargs)
+        self.tensorboard.on_epoch_start(*args, **kwargs)
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/lr.py` & `torchmanager-1.1.4/torchmanager/callbacks/lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from torchmanager_core.typing import Any, Dict, Generic, Optional, TypeVar
 
 from .callback import FrequencyCallback
 
 Scheduler = TypeVar("Scheduler", bound=torch.optim.lr_scheduler._LRScheduler)
 Writer = TypeVar("Writer", bound=SummaryWriteble)
 
+
 class LrSchedueler(FrequencyCallback, Generic[Scheduler]):
     """
     The callback to step learning rate scheduler
 
     * extends: `FrequencyCallback`
 
     - Parameters:
@@ -44,23 +45,24 @@
     def on_epoch_end(self, epoch: int, summary: Dict[str, float], val_summary: Optional[Dict[str, Any]] = None) -> None:
         # get lr summary
         lr_summary = {}
         lr_list = self._scheduler.get_last_lr()
         if len(lr_list) > 1:
             for i, lr in enumerate(lr_list):
                 lr_summary[f'{self._name}_{i}'] = lr
-        else: lr_summary[self._name] = lr_list[0]
+        else:
+            lr_summary[self._name] = lr_list[0]
 
         # write results to Tensorboard
         if self._writer is not None:
             # record summary
             for key in lr_summary.keys():
                 result: Dict[str, float] = {}
                 result["train"] = lr_summary[key]
                 self._writer.add_scalars(key, result, epoch)
 
         # update lr scheduler
         summary.update(lr_summary)
         super().on_epoch_end(epoch, summary, val_summary)
 
     def step(self, *args: Any, **kwargs: Any) -> Any:
-        self._scheduler.step()
+        self._scheduler.step()
```

### Comparing `torchmanager-1.1.3/torchmanager/callbacks/tensorboard.py` & `torchmanager-1.1.4/torchmanager/callbacks/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from torchmanager_core import tensorboard, torch
 from torchmanager_core.typing import Dict, Optional, Set, Tuple
 from torchmanager_core.protocols import Frequency
 
 from .callback import FrequencyCallback
 
+
 class TensorBoard(FrequencyCallback):
     """
     The callback to record summary to tensorboard for each epoch
 
     * extends: `.callback.FrequencyCallback`
     * requires: `tensorboard` package
 
@@ -55,10 +56,11 @@
             if val_summary is not None and key in val_summary:
                 r["val"] = val_summary[key]
             self.writer.add_scalars(key, r, self.current_step + 1)
 
     def step(self, summary: Dict[str, float], val_summary: Optional[Dict[str, float]] = None) -> Tuple[Set[str], Dict[str, float], Optional[Dict[str, float]]]:
         # fetch keys
         keys = list(summary.keys())
-        if val_summary is not None: keys += list(val_summary.keys())
+        if val_summary is not None:
+            keys += list(val_summary.keys())
         keys = set(keys)
-        return keys, summary, val_summary
+        return keys, summary, val_summary
```

### Comparing `torchmanager-1.1.3/torchmanager/compatibility.py` & `torchmanager-1.1.4/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/data/dataset.py` & `torchmanager-1.1.4/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/data/sliding.py` & `torchmanager-1.1.4/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/losses/cross_entropy.py` & `torchmanager-1.1.4/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/losses/dice.py` & `torchmanager-1.1.4/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/losses/loss.py` & `torchmanager-1.1.4/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/losses/mse.py` & `torchmanager-1.1.4/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/metrics/accuracy.py` & `torchmanager-1.1.4/torchmanager/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/metrics/conf_met.py` & `torchmanager-1.1.4/torchmanager/metrics/conf_met.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/metrics/iou.py` & `torchmanager-1.1.4/torchmanager/metrics/iou.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,24 +36,26 @@
     def __init__(self, dim: int = 1, smooth: float = 1e-4, threshold: float = 0, target: Optional[str] = None) -> None:
         """
         Constructor
 
         - Parameters:
             - dim: An `int` of class dimension
             - smooth: A `float` of smooth value to avoid zero devision
+            - threshold: A `float` of min mIoU threshold
+            - target: A `str` of target name in `input` and `target` during direct calling
         """
         super().__init__(target=target)
         assert dim > 0, _raise(ValueError(f"The dimension must be a positive number, got {dim}."))
         assert threshold >= 0 and threshold <= 1, _raise(ValueError(f"The threshold must be in range [0,1], got {threshold}."))
         self._dim = dim
         self._smooth = smooth
         self._threshold = threshold
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
-        input = input.argmax(self._dim)
+        input = input.argmax(self._dim) if input.shape[self._dim] > 1 else input > 0
         intersection = (input & target).float().sum()
         union = (input | target).float().sum()
         iou = (intersection + self._smooth) / (union + self._smooth)
         thresholded = torch.clamp(10 / (1 - self._threshold) * (iou - self._threshold), 0, 10).ceil() / 10
         return thresholded
```

### Comparing `torchmanager-1.1.3/torchmanager/metrics/metric.py` & `torchmanager-1.1.4/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/testing.py` & `torchmanager-1.1.4/torchmanager/testing.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/train/checkpoint.py` & `torchmanager-1.1.4/torchmanager/train/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,25 +56,25 @@
         # load checkpint dictionary
         ckpt: Dict[str, Any] = torch.load(ckpt_path, map_location=map_location)
 
         # load model
         if ckpt["save_weights_only"] is True:
             assert model is not None, _raise(TypeError("Model must be given to load this checkpoint because `save_weights_only` was set to be `True`."))
             state_dict: OrderedDict[str, Any] = ckpt["model"]
-            model.load_state_dict(state_dict)
+            model.load_state_dict(state_dict=state_dict)
             ckpt["model"] = model
         else:
             # remove data parallel wrap
             if isinstance(ckpt["model"], torch.nn.parallel.DataParallel):
                 ckpt["model"] = ckpt["model"].module
 
             # load model structure with checkpoint weights
             if model is not None:
                 saved_model: StateDictLoadable = ckpt["model"]  # type: ignore
-                model.load_state_dict(OrderedDict(saved_model.state_dict()))
+                model.load_state_dict(state_dict=OrderedDict(saved_model.state_dict()))
                 ckpt["model"] = model
         return cls(**ckpt)
 
     def save(self, epoch: int, ckpt_path: str) -> None:
         """
         Saves current checkpoint
```

### Comparing `torchmanager-1.1.3/torchmanager/train/learning_rate.py` & `torchmanager-1.1.4/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager/training.py` & `torchmanager-1.1.4/torchmanager/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager_core/devices/device.py` & `torchmanager-1.1.4/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager_core/errors/train.py` & `torchmanager-1.1.4/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager_core/protocols.py` & `torchmanager-1.1.4/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager-1.1.3/torchmanager_core/version.py` & `torchmanager-1.1.4/torchmanager_core/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,155 @@
 import functools
 
-from .typing import Any, Optional
+from .typing import Any, Enum, Optional
 from .view import warnings
 
 
+class PreRelease(Enum):
+    ALPHA = 'a'
+    BETA = 'b'
+    RELEASE_CANDIDATE = "rc"
+
+    def __gt__(self, pre_release: Any) -> bool:
+        # convert pre release
+        if not isinstance(pre_release, PreRelease):
+            pre_release = PreRelease(pre_release)
+
+        # check pre release version
+        if self == pre_release:
+            return False
+        elif self == PreRelease.RELEASE_CANDIDATE:
+            return True
+        elif self == PreRelease.BETA and pre_release == PreRelease.ALPHA:
+            return True
+        else:
+            return False
+
+    def __lt__(self, pre_release: Any) -> bool:
+        # convert pre release
+        if not isinstance(pre_release, PreRelease):
+            pre_release = PreRelease(pre_release)
+
+        # check pre release version
+        if self == pre_release:
+            return False
+        elif pre_release == PreRelease.RELEASE_CANDIDATE:
+            return True
+        elif pre_release == PreRelease.BETA and self == PreRelease.ALPHA:
+            return True
+        else:
+            return False
+
+    def __le__(self, other: Any) -> bool:
+        return self == other or self < other
+
+    def __ge__(self, other: Any) -> bool:
+        return self == other or self > other
+
+
 class Version:
     main_version: int
     minor_version: int
-    pre_release: Optional[str]
+    pre_release: Optional[PreRelease]
+    pre_release_version: int
     sub_version: int
 
     def __init__(self, v: Any, /) -> None:
         # convert to string
         version_str = str(v)
 
         # format version
         if version_str.startswith('v'):
             version_str = version_str[1:]
 
         # split pre-release version
-        pre_release_parts = version_str.split('a')
-        if len(pre_release_parts) > 1:
-            self.pre_release = 'a' + pre_release_parts[1]
-            version_str = pre_release_parts[0]
-        else:
+        if 'a' in version_str:
+            pre_release_parts = version_str.split('a')
+            self.pre_release = PreRelease.ALPHA
+        elif 'b' in version_str:
             pre_release_parts = version_str.split('b')
-            if len(pre_release_parts) > 1:
-                self.pre_release = 'b' + pre_release_parts[1]
-                version_str = pre_release_parts[0]
-            else:
-                self.pre_release = "0"
+            self.pre_release = PreRelease.BETA
+        elif 'rc' in version_str:
+            pre_release_parts = version_str.split('rc')
+            self.pre_release = PreRelease.RELEASE_CANDIDATE
+        else:
+            pre_release_parts = [version_str, "0"]
+            self.pre_release = None
+        version_str = pre_release_parts[0]
+        self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 1
 
         # split version
         version_parts = version_str.split('.')
         self.main_version = int(version_parts[0])
         self.minor_version = int(version_parts[1])
         self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
 
     def __repr__(self) -> str:
         version_str = f"v{self.main_version}"
         if self.minor_version > 0 or self.sub_version > 0:
             version_str += f".{self.minor_version}"
         if self.sub_version > 0:
             version_str += f".{self.sub_version}"
         if self.pre_release is not None:
-            version_str += self.pre_release
+            version_str += f"{self.pre_release.value}{self.pre_release_version}"
         return version_str
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Version):
-            return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release
+            return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release and self.pre_release_version == other.pre_release_version
         else:
             other = Version(str(other))
             return self.__eq__(other)
 
     def __lt__(self, other: Any) -> bool:
-        if isinstance(other, Version):
-            if self.main_version < other.main_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version < other.minor_version:
-                    return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version < other.sub_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
-                return self.sub_version < other.sub_version
-            return False
-        else:
+        # convert to version
+        if not isinstance(other, Version):
             other = Version(str(other))
-            return self.__lt__(other)
 
-    def __gt__(self, other: Any) -> bool:
-        if isinstance(other, Version):
-            if self.main_version > other.main_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version > other.minor_version:
+        # check version
+        if self.main_version < other.main_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version < other.minor_version:
                 return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version > other.sub_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
-                return self.sub_version > other.sub_version
-            return False
-        else:
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version < other.sub_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
+            return self.pre_release < other.pre_release or (self.pre_release == other.pre_release and self.pre_release_version < other.pre_release_version)
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None:
+            return True
+        return False
+
+    def __gt__(self, other: Any) -> bool:
+        # convert to version
+        if not isinstance(other, Version):
             other = Version(str(other))
-            return self.__gt__(other)
+
+        # check version
+        if self.main_version > other.main_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version > other.minor_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version > other.sub_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
+            return self.pre_release > other.pre_release or (self.pre_release == other.pre_release and self.pre_release_version > other.pre_release_version)
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and other.pre_release is not None:
+            return True
+        return False
 
     def __le__(self, other: Any) -> bool:
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.1")
-CURRENT = Version("v1.1.3")
-DESCRIPTION: str = "PyTorch Training Manager v1.1.3"
+CURRENT = Version("v1.1.4")
+DESCRIPTION: str = "PyTorch Training Manager v1.1.4"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager-1.1.3/PKG-INFO` & `torchmanager-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torchmanager
-Version: 1.1.3
-Summary: PyTorch Training Manager v1.1.3
+Version: 1.1.4
+Summary: PyTorch Training Manager v1.1.4
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

