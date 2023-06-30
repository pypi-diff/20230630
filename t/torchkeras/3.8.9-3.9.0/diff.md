# Comparing `tmp/torchkeras-3.8.9.tar.gz` & `tmp/torchkeras-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchkeras-3.8.9.tar", last modified: Thu Jun 29 13:43:04 2023, max compression
+gzip compressed data, was "dist/torchkeras-3.9.0.tar", last modified: Fri Jun 30 07:06:46 2023, max compression
```

## Comparing `torchkeras-3.8.9.tar` & `torchkeras-3.9.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.536709 torchkeras-3.8.9/
--rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.8.9/LICENSE
--rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.8.9/MANIFEST.in
--rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-29 13:43:04.536179 torchkeras-3.8.9/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)    12396 2023-06-25 16:00:42.000000 torchkeras-3.8.9/README.md
--rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-06-29 13:43:04.536936 torchkeras-3.8.9/setup.cfg
--rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-01 01:30:50.000000 torchkeras-3.8.9/setup.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.509811 torchkeras-3.8.9/torchkeras/
--rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-06-12 11:39:16.000000 torchkeras-3.8.9/torchkeras/__init__.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.530976 torchkeras-3.8.9/torchkeras/assets/
--rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/SimHei.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20)   487438 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/bus.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/park.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/zidane.jpg
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.532099 torchkeras-3.8.9/torchkeras/chatgpt/
--rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.8.9/torchkeras/chatgpt/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     8640 2023-06-09 14:44:53.000000 torchkeras-3.8.9/torchkeras/data.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.8.9/torchkeras/eda.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.8.9/torchkeras/email.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    11531 2023-06-25 03:42:54.000000 torchkeras-3.8.9/torchkeras/hugmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10468 2023-06-14 13:45:41.000000 torchkeras-3.8.9/torchkeras/kerascallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    12601 2023-06-29 09:06:38.000000 torchkeras-3.8.9/torchkeras/kerasmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.8.9/torchkeras/metrics.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.535769 torchkeras-3.8.9/torchkeras/models/
--rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.8.9/torchkeras/models/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.8.9/torchkeras/models/resnet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.8.9/torchkeras/models/ssd.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.8.9/torchkeras/models/unet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.8.9/torchkeras/pbar.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.8.9/torchkeras/plots.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.8.9/torchkeras/soup.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.8.9/torchkeras/summary.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3843 2023-06-12 11:38:27.000000 torchkeras-3.8.9/torchkeras/utils.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.512226 torchkeras-3.8.9/torchkeras.egg-info/
--rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)      737 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/SOURCES.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/dependency_links.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/requires.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       37 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/top_level.txt
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.888952 torchkeras-3.9.0/
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.9.0/LICENSE
+-rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.9.0/MANIFEST.in
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-30 07:06:46.888637 torchkeras-3.9.0/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)    12396 2023-06-25 16:00:42.000000 torchkeras-3.9.0/README.md
+-rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-06-30 07:06:46.889024 torchkeras-3.9.0/setup.cfg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-30 07:06:01.000000 torchkeras-3.9.0/setup.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.865748 torchkeras-3.9.0/torchkeras/
+-rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-06-30 07:05:32.000000 torchkeras-3.9.0/torchkeras/__init__.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.883980 torchkeras-3.9.0/torchkeras/assets/
+-rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/SimHei.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/park.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.9.0/torchkeras/assets/zidane.jpg
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.885511 torchkeras-3.9.0/torchkeras/chatgpt/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.9.0/torchkeras/chatgpt/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     8621 2023-06-30 01:34:56.000000 torchkeras-3.9.0/torchkeras/data.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.9.0/torchkeras/eda.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.9.0/torchkeras/email.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11531 2023-06-25 03:42:54.000000 torchkeras-3.9.0/torchkeras/hugmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10903 2023-06-29 23:05:25.000000 torchkeras-3.9.0/torchkeras/kerascallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    13855 2023-06-30 07:03:22.000000 torchkeras-3.9.0/torchkeras/kerasmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.9.0/torchkeras/metrics.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.888235 torchkeras-3.9.0/torchkeras/models/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.9.0/torchkeras/models/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.9.0/torchkeras/models/resnet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.9.0/torchkeras/models/ssd.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.9.0/torchkeras/models/unet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.9.0/torchkeras/pbar.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.9.0/torchkeras/plots.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.9.0/torchkeras/soup.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.9.0/torchkeras/summary.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3843 2023-06-12 11:38:27.000000 torchkeras-3.9.0/torchkeras/utils.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-30 07:06:46.868796 torchkeras-3.9.0/torchkeras.egg-info/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)      711 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/SOURCES.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/dependency_links.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/requires.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       26 2023-06-30 07:06:46.000000 torchkeras-3.9.0/torchkeras.egg-info/top_level.txt
```

### Comparing `torchkeras-3.8.9/LICENSE` & `torchkeras-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/PKG-INFO` & `torchkeras-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.9
+Version: 3.9.0
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.9 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.0 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
```

### Comparing `torchkeras-3.8.9/README.md` & `torchkeras-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/setup.py` & `torchkeras-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/assets/SimHei.ttf` & `torchkeras-3.9.0/torchkeras/assets/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/assets/park.jpg` & `torchkeras-3.9.0/torchkeras/assets/park.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/assets/zidane.jpg` & `torchkeras-3.9.0/torchkeras/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/chatgpt/__init__.py` & `torchkeras-3.9.0/torchkeras/chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/data.py` & `torchkeras-3.9.0/torchkeras/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
                 done_files.add(y)
     print('\nafter merge:')
     print(f'{to_folder}: {get_file_num(to_folder)} files')
     return to_folder 
 
 
 def get_example_image(img_name='park.jpg'):
-    'name can be bus.jpg / park.jpg / zidane.jpg'
+    'name can be park.jpg / zidane.jpg'
     img_path = str(path.parent/f"assets/{img_name}")
-    assert os.path.exists(img_path), 'img_name can only be bus.jpg / park.jpg / zidane.jpg'
+    assert os.path.exists(img_path), 'img_name can only be  park.jpg / zidane.jpg'
     return Image.open(img_path)
 
 def get_url_img(url):
     from skimage import io
     arr = io.imread(url)
     return Image.fromarray(arr)
```

### Comparing `torchkeras-3.8.9/torchkeras/eda.py` & `torchkeras-3.9.0/torchkeras/eda.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/email.py` & `torchkeras-3.9.0/torchkeras/email.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/hugmodel.py` & `torchkeras-3.9.0/torchkeras/hugmodel.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/kerascallbacks.py` & `torchkeras-3.9.0/torchkeras/kerascallbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,19 +175,24 @@
         
             
     def on_fit_end(self,  model:"KerasModel"):
         dfhistory = pd.DataFrame(model.history)
         title = self.get_title(model)
         self.update_graph(model, title = title)
         
-    def get_title(self,  model:'KerasModel'):
+    def get_best_score(self, model:'KerasModel'):
         dfhistory = pd.DataFrame(model.history)
         arr_scores = dfhistory[model.monitor]
         best_score = np.max(arr_scores) if model.mode=="max" else np.min(arr_scores)
-        title = f'best {model.monitor} = {best_score:.4f}'
+        best_epoch = dfhistory.loc[arr_scores==best_score,'epoch'].tolist()[0]
+        return (best_epoch, best_score)
+        
+    def get_title(self,  model:'KerasModel'):
+        best_epoch,best_score = self.get_best_score(model)
+        title = f'best {model.monitor} = {best_score:.4f} (@epoch {best_epoch})'
         return title
 
     def update_graph(self, model:'KerasModel', title=None, x_bounds=None, y_bounds=None):
         import matplotlib.pyplot as plt
         self.plt = plt
         if not hasattr(self, 'graph_fig'):
             self.graph_fig, self.graph_ax = plt.subplots(1, figsize=self.figsize)
@@ -201,26 +206,30 @@
         if  m1 in dfhistory.columns:
             train_metrics = dfhistory[m1]
             self.graph_ax.plot(epochs,train_metrics,'bo--',label= m1)
 
         m2 = 'val_'+self.metric
         if m2 in dfhistory.columns:
             val_metrics = dfhistory[m2]
-            self.graph_ax.plot(epochs,val_metrics,'ro-',label =m2)
+            self.graph_ax.plot(epochs,val_metrics,'co-',label =m2)
 
         if self.metric in dfhistory.columns:
             metric_values = dfhistory[self.metric]
-            self.graph_ax.plot(epochs, metric_values,'ro-', label = self.metric)
+            self.graph_ax.plot(epochs, metric_values,'co-', label = self.metric)
 
         self.graph_ax.set_xlabel("epoch")
         self.graph_ax.set_ylabel(self.metric)  
         if title:
              self.graph_ax.set_title(title)
         if m1 in dfhistory.columns or m2 in dfhistory.columns or self.metric in dfhistory.columns:
             self.graph_ax.legend(loc='best')
+            
+        if len(epochs)>0:
+            best_epoch, best_score = self.get_best_score(model)
+            self.graph_ax.plot(best_epoch,best_score,'r*',markersize=15)
 
         if x_bounds is not None: self.graph_ax.set_xlim(*x_bounds)
         if y_bounds is not None: self.graph_ax.set_ylim(*y_bounds)
         self.graph_out.update(self.graph_ax.figure)
         self.plt.close();
```

### Comparing `torchkeras-3.8.9/torchkeras/kerasmodel.py` & `torchkeras-3.9.0/torchkeras/kerasmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class StepRunner:
     def __init__(self, net, loss_fn, accelerator=None, stage = "train", metrics_dict = None, 
                  optimizer = None, lr_scheduler = None
                  ):
         self.net,self.loss_fn,self.metrics_dict,self.stage = net,loss_fn,metrics_dict,stage
         self.optimizer,self.lr_scheduler = optimizer,lr_scheduler
-        self.accelerator = accelerator if accelerator is not None else Accelerator() 
+        self.accelerator = accelerator
         if self.stage=='train':
             self.net.train() 
         else:
             self.net.eval()
     
     def __call__(self, batch):
         features,labels = batch 
@@ -67,14 +67,15 @@
         loop = tqdm(enumerate(dataloader,start=1), 
                     total=n,
                     file=sys.stdout,
                     disable=not self.accelerator.is_local_main_process or self.quiet,
                     ncols=100
                    )
         epoch_losses = {}
+        
         for step, batch in loop: 
             with self.accelerator.accumulate(self.net):
                 step_losses,step_metrics = self.steprunner(batch)   
                 step_log = dict(step_losses,**step_metrics)
                 for k,v in step_losses.items():
                     epoch_losses[k] = epoch_losses.get(k,0.0)+v
 
@@ -111,30 +112,30 @@
         super().__init__()
         self.net,self.loss_fn,self.metrics_dict = net, loss_fn, torch.nn.ModuleDict(metrics_dict) 
         self.optimizer = optimizer if optimizer is not None else torch.optim.Adam(
             self.net.parameters(), lr=3e-4)
         self.lr_scheduler = lr_scheduler
         self.from_scratch = True
         
-    def save_ckpt(self, ckpt_path='checkpoint.pt'):
-        net_dict = self.accelerator.get_state_dict(self.net)
-        self.accelerator.save(net_dict,ckpt_path)
+    def save_ckpt(self, ckpt_path='checkpoint.pt', accelerator= None):
+        accelerator = accelerator if accelerator is not None else self.accelerator
+        net_dict = accelerator.get_state_dict(self.net)
+        accelerator.save(net_dict,ckpt_path)
       
     def load_ckpt(self, ckpt_path='checkpoint.pt'):
-        self.net.load_state_dict(torch.load(ckpt_path))
+        self.net.load_state_dict(torch.load(ckpt_path,map_location='cpu'))
         self.from_scratch = False
 
     def forward(self, x):
         return self.net.forward(x)
     
     def fit(self, train_data, val_data=None, epochs=10, ckpt_path='checkpoint.pt',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True,  wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1):
-        
         from torchkeras.utils import colorful,is_jupyter
         
         self.__dict__.update(locals())
         self.accelerator = Accelerator(mixed_precision=mixed_precision,cpu=cpu,
             gradient_accumulation_steps=gradient_accumulation_steps)
         device = str(self.accelerator.device)
         device_type = '🐌'  if 'cpu' in device else ('⚡️' if 'cuda' in device else '🚀')
@@ -230,16 +231,16 @@
                  if hasattr(cb,'on_validation_epoch_end')]
 
             # 3，early-stopping -------------------------------------------------
             self.accelerator.wait_for_everyone()
             arr_scores = self.history[monitor]
             best_score_idx = np.argmax(arr_scores) if mode=="max" else np.argmin(arr_scores)
 
-            if best_score_idx==len(arr_scores)-1:
-                self.save_ckpt(ckpt_path)
+            if best_score_idx==len(arr_scores)-1 and self.accelerator.is_local_main_process:
+                self.save_ckpt(ckpt_path,accelerator = self.accelerator)
                 if not should_quiet:
                     self.accelerator.print(colorful("<<<<<< reach best {0} : {1} >>>>>>".format(
                         monitor,arr_scores[best_score_idx])))
 
             if len(arr_scores)-best_score_idx>patience:
                 self.accelerator.print(colorful(
                     "<<<<<< {} without improvement in {} epoch,""early stopping >>>>>>"
@@ -249,33 +250,57 @@
         if self.accelerator.is_local_main_process:   
             dfhistory = pd.DataFrame(self.history)
             [cb.on_fit_end(model = self) for cb in self.callbacks 
                  if hasattr(cb,'on_fit_end')]
             self.net = self.accelerator.unwrap_model(self.net)
             self.net.cpu()
             self.load_ckpt(ckpt_path)
+            torch.save(dfhistory,'dfhistory.pt')
             return dfhistory
-    
-    @torch.no_grad()
+        
     def evaluate(self, val_data, quiet=False):
         accelerator = Accelerator() if not hasattr(self,'accelerator') else self.accelerator
-        self.net,self.loss_fn,self.metrics_dict = accelerator.prepare(self.net,self.loss_fn,self.metrics_dict)
+        self.net,self.loss_fn,self.metrics_dict = accelerator.prepare(
+            self.net,self.loss_fn,self.metrics_dict)
         val_data = accelerator.prepare(val_data)
         val_step_runner = self.StepRunner(net = self.net,stage="val",
                     loss_fn = self.loss_fn,metrics_dict=deepcopy(self.metrics_dict),
                     accelerator = accelerator)
         val_epoch_runner = self.EpochRunner(val_step_runner,quiet=quiet)
-        val_metrics = val_epoch_runner(val_data)
+        with torch.no_grad():
+            val_metrics = val_epoch_runner(val_data)
+        if accelerator.is_local_main_process:
+            torch.save(val_metrics,'val_metrics.pt')
         return val_metrics
     
     def fit_ddp(self,num_processes,train_data,
             val_data=None, epochs=10, ckpt_path='checkpoint.pt',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True, wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1
            ):
+        from accelerate import notebook_launcher
+        train_size = train_data.size if hasattr(train_data,'size') else len(train_data)
+        train_data.size = train_size//num_processes
+        if val_data:
+            val_size = val_data.size if hasattr(val_data,'size') else len(val_data)
+            val_data.size = val_size//num_processes
+            
         args = (train_data,val_data,epochs,ckpt_path,patience,monitor,mode,
             callbacks,plot,wandb,quiet,mixed_precision,cpu,gradient_accumulation_steps)
+        notebook_launcher(self.fit, args, num_processes=num_processes)
+        dfhistory = torch.load('dfhistory.pt')
         
+        train_data.size = train_size 
+        if val_data:
+            val_data.size = val_size 
+        return dfhistory
+    
+    def evaluate_ddp(self, num_processes, val_data, quiet=False):
         from accelerate import notebook_launcher
-        notebook_launcher(self.fit, args, num_processes=num_processes)
-        
+        val_size = val_data.size if hasattr(val_data,'size') else len(val_data)
+        val_data.size = val_size//num_processes
+        args = (val_data,quiet)
+        notebook_launcher(self.evaluate, args, num_processes=num_processes)
+        val_metrics = torch.load('val_metrics.pt')
+        val_data.size = val_size
+        return val_metrics
```

### Comparing `torchkeras-3.8.9/torchkeras/metrics.py` & `torchkeras-3.9.0/torchkeras/metrics.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/models/resnet.py` & `torchkeras-3.9.0/torchkeras/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/models/ssd.py` & `torchkeras-3.9.0/torchkeras/models/ssd.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/models/unet.py` & `torchkeras-3.9.0/torchkeras/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/pbar.py` & `torchkeras-3.9.0/torchkeras/pbar.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/plots.py` & `torchkeras-3.9.0/torchkeras/plots.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/soup.py` & `torchkeras-3.9.0/torchkeras/soup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/summary.py` & `torchkeras-3.9.0/torchkeras/summary.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras/utils.py` & `torchkeras-3.9.0/torchkeras/utils.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.9/torchkeras.egg-info/PKG-INFO` & `torchkeras-3.9.0/torchkeras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.9
+Version: 3.9.0
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.9 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.9.0 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
```

### Comparing `torchkeras-3.8.9/torchkeras.egg-info/SOURCES.txt` & `torchkeras-3.9.0/torchkeras.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 torchkeras/utils.py
 torchkeras.egg-info/PKG-INFO
 torchkeras.egg-info/SOURCES.txt
 torchkeras.egg-info/dependency_links.txt
 torchkeras.egg-info/requires.txt
 torchkeras.egg-info/top_level.txt
 torchkeras/assets/SimHei.ttf
-torchkeras/assets/bus.jpg
 torchkeras/assets/park.jpg
 torchkeras/assets/zidane.jpg
 torchkeras/chatgpt/__init__.py
 torchkeras/models/__init__.py
 torchkeras/models/resnet.py
 torchkeras/models/ssd.py
 torchkeras/models/unet.py
```

