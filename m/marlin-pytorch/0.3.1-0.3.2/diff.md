# Comparing `tmp/marlin_pytorch-0.3.1.tar.gz` & `tmp/marlin_pytorch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marlin_pytorch-0.3.1.tar", last modified: Tue Mar  7 09:26:22 2023, max compression
+gzip compressed data, was "marlin_pytorch-0.3.2.tar", last modified: Fri Jun 30 11:09:30 2023, max compression
```

## Comparing `marlin_pytorch-0.3.1.tar` & `marlin_pytorch-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.307659 marlin_pytorch-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-03-07 09:26:22.307659 marlin_pytorch-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8763 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-07 09:26:22.307659 marlin_pytorch-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.291659 marlin_pytorch-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.295659 marlin_pytorch-0.3.1/src/marlin_pytorch/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4048 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/face_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.303659 marlin_pytorch-0.3.1/src/marlin_pytorch/model/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     9856 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/marlin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8329 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/modules.py
--rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/model/positional_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/util.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.299659 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-07 09:26:22.000000 marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-07 09:26:22.303659 marlin_pytorch-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/test/test_marlin_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/test/test_marlin_vit_base.py
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/test/test_marlin_vit_large.py
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/test/test_marlin_vit_small.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-03-07 09:24:53.000000 marlin_pytorch-0.3.1/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.091638 marlin_pytorch-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-06-30 11:09:30.091638 marlin_pytorch-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-30 11:09:30.091638 marlin_pytorch-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1733 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.083638 marlin_pytorch-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.087638 marlin_pytorch-0.3.2/src/marlin_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4048 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6062 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/face_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.087638 marlin_pytorch-0.3.2/src/marlin_pytorch/model/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3420 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10094 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/marlin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8329 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/modules.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1675 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/model/positional_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3514 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-30 11:09:29.000000 marlin_pytorch-0.3.2/src/marlin_pytorch/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.087638 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-06-30 11:09:30.000000 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-06-30 11:09:30.000000 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-30 11:09:30.000000 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-06-30 11:09:30.000000 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-30 11:09:30.000000 marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-30 11:09:30.091638 marlin_pytorch-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3173 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/test/test_marlin_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/test/test_marlin_vit_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      469 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/test/test_marlin_vit_large.py
+-rw-r--r--   0 runner    (1001) docker     (122)      468 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/test/test_marlin_vit_small.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-06-30 11:07:11.000000 marlin_pytorch-0.3.2/test/test_version.py
```

### Comparing `marlin_pytorch-0.3.1/LICENSE` & `marlin_pytorch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/PKG-INFO` & `marlin_pytorch-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin_pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Official pytorch implementation for MARLIN.
 Home-page: https://github.com/ControlNet/MARLIN
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/MARLIN/issues
 Project-URL: Source Code, https://github.com/ControlNet/MARLIN
@@ -58,21 +58,21 @@
         <img src="https://img.shields.io/pypi/dm/marlin-pytorch?style=flat-square">
     </a>
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/release.yaml?branch=master&label=release&style=flat-square"></a>
     <a href="https://coveralls.io/github/ControlNet/MARLIN"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square"></a>
 </div>
 
 This repo is the official PyTorch implementation for the paper 
-[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/2211.06627) (CVPR 2023).
+[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://openaccess.thecvf.com/content/CVPR2023/html/Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper) (CVPR 2023).
 
 ## Repository Structure
 
 The repository contains 2 parts:
  - `marlin-pytorch`: The PyPI package for MARLIN used for inference.
  - The implementation for the paper including training and evaluation scripts.
 
@@ -251,21 +251,23 @@
 from marlin_pytorch.config import register_model_from_yaml
 
 register_model_from_yaml("my_marlin_model", "path/to/config.yaml")
 model = Marlin.from_file("my_marlin_model", "path/to/marlin.ckpt")
 ```
 
 ## References
-If you find this work useful in your research, please cite it.
+If you find this work useful for your research, please consider citing it.
 ```bibtex
-@article{cai2022marlin,
+@inproceedings{cai2022marlin,
   title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
   author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-  journal = {arXiv preprint arXiv:2211.06627},
-  year = {2022},
+  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
+  year = {2023},
+  month = {June},
+  pages = {1493-1504}
 }
 ```
 
 ## Acknowledgements
 
 Some code about model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The code related to preprocessing
 is borrowed from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marlin_pytorch Version: 0.3.1 Summary: Official
+Metadata-Version: 2.1 Name: marlin_pytorch Version: 0.3.2 Summary: Official
 pytorch implementation for MARLIN. Home-page: https://github.com/ControlNet/
 MARLIN Author: ControlNet Author-email: smczx@hotmail.com License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/MARLIN/issues Project-
 URL: Source Code, https://github.com/ControlNet/MARLIN Keywords: deep
 learning,pytorch,AI Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -20,24 +20,26 @@
  [https://img.shields.io/github/license/ControlNet/MARLIN?style=flat-square]
  [https://img.shields.io/badge/arXiv-2211.06627-b31b1b.svg?style=flat-square]
   [https://img.shields.io/pypi/v/marlin-pytorch?style=flat-square] [https://
       img.shields.io/pypi/dm/marlin-pytorch?style=flat-square] [https://
   img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square] [https://
 img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch]
    [https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
-      unittest.yaml?branch=dev&label=release&style=flat-square] [https://
+     unittest.yaml?branch=dev&label=unittest&style=flat-square] [https://
        img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
      release.yaml?branch=master&label=release&style=flat-square] [https://
  img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square]
 This repo is the official PyTorch implementation for the paper [MARLIN: Masked
-Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/
-2211.06627) (CVPR 2023). ## Repository Structure The repository contains 2
-parts: - `marlin-pytorch`: The PyPI package for MARLIN used for inference. -
-The implementation for the paper including training and evaluation scripts. ```
-. âââ assets # Images for README.md âââ LICENSE âââ README.md
+Autoencoder for facial video Representation LearnINg](https://
+openaccess.thecvf.com/content/CVPR2023/html/
+Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper)
+(CVPR 2023). ## Repository Structure The repository contains 2 parts: -
+`marlin-pytorch`: The PyPI package for MARLIN used for inference. - The
+implementation for the paper including training and evaluation scripts. ``` .
+âââ assets # Images for README.md âââ LICENSE âââ README.md
 âââ MODEL_ZOO.md âââ CITATION.cff âââ .gitignore âââ
 .github # below is for the PyPI package marlin-pytorch âââ src # Source
 code for marlin-pytorch âââ tests # Unittest âââ
 requirements.lib.txt âââ setup.py âââ init.py âââ version.txt
 # below is for the paper implementation âââ configs # Configs for
 experiments settings âââ model # Marlin models âââ preprocess #
 Preprocessing scripts âââ dataset # Dataloaders âââ utils # Utility
@@ -99,15 +101,17 @@
 marlin_vit_base.yaml \ --data_dir /path/to/youtube_faces \ --n_gpus 4 \ --
 num_workers 8 \ --batch_size 16 \ --epochs 2000 \ --official_pretrained /path/
 to/videomae/checkpoint.pth ``` After trained, you can load the checkpoint for
 inference by ```python from marlin_pytorch import Marlin from
 marlin_pytorch.config import register_model_from_yaml register_model_from_yaml
 ("my_marlin_model", "path/to/config.yaml") model = Marlin.from_file
 ("my_marlin_model", "path/to/marlin.ckpt") ``` ## References If you find this
-work useful in your research, please cite it. ```bibtex @article{cai2022marlin,
-title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
-author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav
-and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-journal = {arXiv preprint arXiv:2211.06627}, year = {2022}, } ``` ##
-Acknowledgements Some code about model is based on [MCG-NJU/VideoMAE](https://
-github.com/MCG-NJU/VideoMAE). The code related to preprocessing is borrowed
-from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
+work useful for your research, please consider citing it. ```bibtex
+@inproceedings{cai2022marlin, title = {MARLIN: Masked Autoencoder for facial
+video Representation LearnINg}, author = {Cai, Zhixi and Ghosh, Shreya and
+Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and
+Haffari, Reza and Hayat, Munawar}, booktitle = {Proceedings of the IEEE/CVF
+Conference on Computer Vision and Pattern Recognition (CVPR)}, year = {2023},
+month = {June}, pages = {1493-1504} } ``` ## Acknowledgements Some code about
+model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The
+code related to preprocessing is borrowed from [JDAI-CV/FaceX-Zoo](https://
+github.com/JDAI-CV/FaceX-Zoo).
```

### Comparing `marlin_pytorch-0.3.1/README.md` & `marlin_pytorch-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         <img src="https://img.shields.io/pypi/dm/marlin-pytorch?style=flat-square">
     </a>
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/release.yaml?branch=master&label=release&style=flat-square"></a>
     <a href="https://coveralls.io/github/ControlNet/MARLIN"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square"></a>
 </div>
 
 This repo is the official PyTorch implementation for the paper 
-[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/2211.06627) (CVPR 2023).
+[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://openaccess.thecvf.com/content/CVPR2023/html/Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper) (CVPR 2023).
 
 ## Repository Structure
 
 The repository contains 2 parts:
  - `marlin-pytorch`: The PyPI package for MARLIN used for inference.
  - The implementation for the paper including training and evaluation scripts.
 
@@ -224,21 +224,23 @@
 from marlin_pytorch.config import register_model_from_yaml
 
 register_model_from_yaml("my_marlin_model", "path/to/config.yaml")
 model = Marlin.from_file("my_marlin_model", "path/to/marlin.ckpt")
 ```
 
 ## References
-If you find this work useful in your research, please cite it.
+If you find this work useful for your research, please consider citing it.
 ```bibtex
-@article{cai2022marlin,
+@inproceedings{cai2022marlin,
   title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
   author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-  journal = {arXiv preprint arXiv:2211.06627},
-  year = {2022},
+  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
+  year = {2023},
+  month = {June},
+  pages = {1493-1504}
 }
 ```
 
 ## Acknowledgements
 
 Some code about model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The code related to preprocessing
 is borrowed from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
```

#### html2text {}

```diff
@@ -6,24 +6,26 @@
  [https://img.shields.io/github/license/ControlNet/MARLIN?style=flat-square]
  [https://img.shields.io/badge/arXiv-2211.06627-b31b1b.svg?style=flat-square]
   [https://img.shields.io/pypi/v/marlin-pytorch?style=flat-square] [https://
       img.shields.io/pypi/dm/marlin-pytorch?style=flat-square] [https://
   img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square] [https://
 img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch]
    [https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
-      unittest.yaml?branch=dev&label=release&style=flat-square] [https://
+     unittest.yaml?branch=dev&label=unittest&style=flat-square] [https://
        img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
      release.yaml?branch=master&label=release&style=flat-square] [https://
  img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square]
 This repo is the official PyTorch implementation for the paper [MARLIN: Masked
-Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/
-2211.06627) (CVPR 2023). ## Repository Structure The repository contains 2
-parts: - `marlin-pytorch`: The PyPI package for MARLIN used for inference. -
-The implementation for the paper including training and evaluation scripts. ```
-. âââ assets # Images for README.md âââ LICENSE âââ README.md
+Autoencoder for facial video Representation LearnINg](https://
+openaccess.thecvf.com/content/CVPR2023/html/
+Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper)
+(CVPR 2023). ## Repository Structure The repository contains 2 parts: -
+`marlin-pytorch`: The PyPI package for MARLIN used for inference. - The
+implementation for the paper including training and evaluation scripts. ``` .
+âââ assets # Images for README.md âââ LICENSE âââ README.md
 âââ MODEL_ZOO.md âââ CITATION.cff âââ .gitignore âââ
 .github # below is for the PyPI package marlin-pytorch âââ src # Source
 code for marlin-pytorch âââ tests # Unittest âââ
 requirements.lib.txt âââ setup.py âââ init.py âââ version.txt
 # below is for the paper implementation âââ configs # Configs for
 experiments settings âââ model # Marlin models âââ preprocess #
 Preprocessing scripts âââ dataset # Dataloaders âââ utils # Utility
@@ -85,15 +87,17 @@
 marlin_vit_base.yaml \ --data_dir /path/to/youtube_faces \ --n_gpus 4 \ --
 num_workers 8 \ --batch_size 16 \ --epochs 2000 \ --official_pretrained /path/
 to/videomae/checkpoint.pth ``` After trained, you can load the checkpoint for
 inference by ```python from marlin_pytorch import Marlin from
 marlin_pytorch.config import register_model_from_yaml register_model_from_yaml
 ("my_marlin_model", "path/to/config.yaml") model = Marlin.from_file
 ("my_marlin_model", "path/to/marlin.ckpt") ``` ## References If you find this
-work useful in your research, please cite it. ```bibtex @article{cai2022marlin,
-title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
-author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav
-and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-journal = {arXiv preprint arXiv:2211.06627}, year = {2022}, } ``` ##
-Acknowledgements Some code about model is based on [MCG-NJU/VideoMAE](https://
-github.com/MCG-NJU/VideoMAE). The code related to preprocessing is borrowed
-from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
+work useful for your research, please consider citing it. ```bibtex
+@inproceedings{cai2022marlin, title = {MARLIN: Masked Autoencoder for facial
+video Representation LearnINg}, author = {Cai, Zhixi and Ghosh, Shreya and
+Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and
+Haffari, Reza and Hayat, Munawar}, booktitle = {Proceedings of the IEEE/CVF
+Conference on Computer Vision and Pattern Recognition (CVPR)}, year = {2023},
+month = {June}, pages = {1493-1504} } ``` ## Acknowledgements Some code about
+model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The
+code related to preprocessing is borrowed from [JDAI-CV/FaceX-Zoo](https://
+github.com/JDAI-CV/FaceX-Zoo).
```

### Comparing `marlin_pytorch-0.3.1/setup.py` & `marlin_pytorch-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/config.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/config.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/face_detector.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/face_detector.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/model/decoder.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/model/decoder.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/model/encoder.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/model/encoder.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/model/marlin.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/model/marlin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from .decoder import MarlinDecoder
 from .encoder import MarlinEncoder
 from ..util import read_video, padding_video, DownloadProgressBar
 
 
 class Marlin(Module):
+
     def __init__(self,
         img_size: int,
         patch_size: int,
         n_frames: int,
         encoder_embed_dim: int,
         encoder_depth: int,
         encoder_num_heads: int,
@@ -153,17 +154,20 @@
         total_frames = int(probe["streams"][0]["nb_frames"])
         if total_frames <= self.clip_frames:
             video = read_video(video_path, channel_first=True) / 255  # (T, C, H, W)
             # pad frames to 16
             v = padding_video(video, self.clip_frames, "same")  # (T, C, H, W)
             assert v.shape[0] == self.clip_frames
             yield v.permute(1, 0, 2, 3).unsqueeze(0).to(self.device)
-        elif total_frames < self.clip_frames * sample_rate:
+        elif total_frames <= self.clip_frames * sample_rate:
             video = read_video(video_path, channel_first=True) / 255  # (T, C, H, W)
             # use first 16 frames
+            if video.shape[0] < self.clip_frames:
+                # double-check the number of frames, see https://github.com/pytorch/vision/issues/2490
+                v = padding_video(video, self.clip_frames, "same")  # (T, C, H, W)
             v = video[:self.clip_frames]
             yield v.permute(1, 0, 2, 3).unsqueeze(0).to(self.device)
         else:
             # extract features based on sliding window
             cap = cv2.VideoCapture(video_path)
             deq = deque(maxlen=self.clip_frames)
```

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/model/modules.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/model/modules.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/model/positional_embedding.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/model/positional_embedding.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch/util.py` & `marlin_pytorch-0.3.2/src/marlin_pytorch/util.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/PKG-INFO` & `marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marlin-pytorch
-Version: 0.3.1
+Version: 0.3.2
 Summary: Official pytorch implementation for MARLIN.
 Home-page: https://github.com/ControlNet/MARLIN
 Author: ControlNet
 Author-email: smczx@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/MARLIN/issues
 Project-URL: Source Code, https://github.com/ControlNet/MARLIN
@@ -58,21 +58,21 @@
         <img src="https://img.shields.io/pypi/dm/marlin-pytorch?style=flat-square">
     </a>
     <a href="https://www.python.org/"><img src="https://img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square"></a>
     <a href="https://pytorch.org/"><img src="https://img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch"></a>
 </div>
 
 <div align="center">
-    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=release&style=flat-square"></a>
+    <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/unittest.yaml?branch=dev&label=unittest&style=flat-square"></a>
     <a href="https://github.com/ControlNet/MARLIN/actions"><img src="https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/release.yaml?branch=master&label=release&style=flat-square"></a>
     <a href="https://coveralls.io/github/ControlNet/MARLIN"><img src="https://img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square"></a>
 </div>
 
 This repo is the official PyTorch implementation for the paper 
-[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/2211.06627) (CVPR 2023).
+[MARLIN: Masked Autoencoder for facial video Representation LearnINg](https://openaccess.thecvf.com/content/CVPR2023/html/Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper) (CVPR 2023).
 
 ## Repository Structure
 
 The repository contains 2 parts:
  - `marlin-pytorch`: The PyPI package for MARLIN used for inference.
  - The implementation for the paper including training and evaluation scripts.
 
@@ -251,21 +251,23 @@
 from marlin_pytorch.config import register_model_from_yaml
 
 register_model_from_yaml("my_marlin_model", "path/to/config.yaml")
 model = Marlin.from_file("my_marlin_model", "path/to/marlin.ckpt")
 ```
 
 ## References
-If you find this work useful in your research, please cite it.
+If you find this work useful for your research, please consider citing it.
 ```bibtex
-@article{cai2022marlin,
+@inproceedings{cai2022marlin,
   title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
   author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-  journal = {arXiv preprint arXiv:2211.06627},
-  year = {2022},
+  booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
+  year = {2023},
+  month = {June},
+  pages = {1493-1504}
 }
 ```
 
 ## Acknowledgements
 
 Some code about model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The code related to preprocessing
 is borrowed from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: marlin-pytorch Version: 0.3.1 Summary: Official
+Metadata-Version: 2.1 Name: marlin-pytorch Version: 0.3.2 Summary: Official
 pytorch implementation for MARLIN. Home-page: https://github.com/ControlNet/
 MARLIN Author: ControlNet Author-email: smczx@hotmail.com License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ControlNet/MARLIN/issues Project-
 URL: Source Code, https://github.com/ControlNet/MARLIN Keywords: deep
 learning,pytorch,AI Platform: UNKNOWN Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.6 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
@@ -20,24 +20,26 @@
  [https://img.shields.io/github/license/ControlNet/MARLIN?style=flat-square]
  [https://img.shields.io/badge/arXiv-2211.06627-b31b1b.svg?style=flat-square]
   [https://img.shields.io/pypi/v/marlin-pytorch?style=flat-square] [https://
       img.shields.io/pypi/dm/marlin-pytorch?style=flat-square] [https://
   img.shields.io/pypi/pyversions/marlin-pytorch?style=flat-square] [https://
 img.shields.io/badge/PyTorch-%3E%3D1.8.0-EE4C2C?style=flat-square&logo=pytorch]
    [https://img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
-      unittest.yaml?branch=dev&label=release&style=flat-square] [https://
+     unittest.yaml?branch=dev&label=unittest&style=flat-square] [https://
        img.shields.io/github/actions/workflow/status/ControlNet/MARLIN/
      release.yaml?branch=master&label=release&style=flat-square] [https://
  img.shields.io/coverallsCoverage/github/ControlNet/MARLIN?style=flat-square]
 This repo is the official PyTorch implementation for the paper [MARLIN: Masked
-Autoencoder for facial video Representation LearnINg](https://arxiv.org/abs/
-2211.06627) (CVPR 2023). ## Repository Structure The repository contains 2
-parts: - `marlin-pytorch`: The PyPI package for MARLIN used for inference. -
-The implementation for the paper including training and evaluation scripts. ```
-. âââ assets # Images for README.md âââ LICENSE âââ README.md
+Autoencoder for facial video Representation LearnINg](https://
+openaccess.thecvf.com/content/CVPR2023/html/
+Cai_MARLIN_Masked_Autoencoder_for_Facial_Video_Representation_LearnINg_CVPR_2023_paper)
+(CVPR 2023). ## Repository Structure The repository contains 2 parts: -
+`marlin-pytorch`: The PyPI package for MARLIN used for inference. - The
+implementation for the paper including training and evaluation scripts. ``` .
+âââ assets # Images for README.md âââ LICENSE âââ README.md
 âââ MODEL_ZOO.md âââ CITATION.cff âââ .gitignore âââ
 .github # below is for the PyPI package marlin-pytorch âââ src # Source
 code for marlin-pytorch âââ tests # Unittest âââ
 requirements.lib.txt âââ setup.py âââ init.py âââ version.txt
 # below is for the paper implementation âââ configs # Configs for
 experiments settings âââ model # Marlin models âââ preprocess #
 Preprocessing scripts âââ dataset # Dataloaders âââ utils # Utility
@@ -99,15 +101,17 @@
 marlin_vit_base.yaml \ --data_dir /path/to/youtube_faces \ --n_gpus 4 \ --
 num_workers 8 \ --batch_size 16 \ --epochs 2000 \ --official_pretrained /path/
 to/videomae/checkpoint.pth ``` After trained, you can load the checkpoint for
 inference by ```python from marlin_pytorch import Marlin from
 marlin_pytorch.config import register_model_from_yaml register_model_from_yaml
 ("my_marlin_model", "path/to/config.yaml") model = Marlin.from_file
 ("my_marlin_model", "path/to/marlin.ckpt") ``` ## References If you find this
-work useful in your research, please cite it. ```bibtex @article{cai2022marlin,
-title = {MARLIN: Masked Autoencoder for facial video Representation LearnINg},
-author = {Cai, Zhixi and Ghosh, Shreya and Stefanov, Kalin and Dhall, Abhinav
-and Cai, Jianfei and Rezatofighi, Hamid and Haffari, Reza and Hayat, Munawar},
-journal = {arXiv preprint arXiv:2211.06627}, year = {2022}, } ``` ##
-Acknowledgements Some code about model is based on [MCG-NJU/VideoMAE](https://
-github.com/MCG-NJU/VideoMAE). The code related to preprocessing is borrowed
-from [JDAI-CV/FaceX-Zoo](https://github.com/JDAI-CV/FaceX-Zoo).
+work useful for your research, please consider citing it. ```bibtex
+@inproceedings{cai2022marlin, title = {MARLIN: Masked Autoencoder for facial
+video Representation LearnINg}, author = {Cai, Zhixi and Ghosh, Shreya and
+Stefanov, Kalin and Dhall, Abhinav and Cai, Jianfei and Rezatofighi, Hamid and
+Haffari, Reza and Hayat, Munawar}, booktitle = {Proceedings of the IEEE/CVF
+Conference on Computer Vision and Pattern Recognition (CVPR)}, year = {2023},
+month = {June}, pages = {1493-1504} } ``` ## Acknowledgements Some code about
+model is based on [MCG-NJU/VideoMAE](https://github.com/MCG-NJU/VideoMAE). The
+code related to preprocessing is borrowed from [JDAI-CV/FaceX-Zoo](https://
+github.com/JDAI-CV/FaceX-Zoo).
```

### Comparing `marlin_pytorch-0.3.1/src/marlin_pytorch.egg-info/SOURCES.txt` & `marlin_pytorch-0.3.2/src/marlin_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/test/test_marlin_pytorch.py` & `marlin_pytorch-0.3.2/test/test_marlin_pytorch.py`

 * *Files identical despite different names*

### Comparing `marlin_pytorch-0.3.1/test/test_version.py` & `marlin_pytorch-0.3.2/test/test_version.py`

 * *Files identical despite different names*

