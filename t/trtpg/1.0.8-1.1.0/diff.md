# Comparing `tmp/trtpg-1.0.8-py3-none-any.whl.zip` & `tmp/trtpg-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,46 +1,22 @@
-Zip file size: 118081 bytes, number of entries: 44
--rw-rw-r--  2.0 unx     1084 b- defN 23-Jun-26 03:16 trtpg/LICENSE.md
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 03:16 trtpg/VERSION
--rw-rw-r--  2.0 unx     1188 b- defN 23-Jun-26 03:16 trtpg/__init__.py
--rw-rw-r--  2.0 unx     4262 b- defN 23-Jun-26 04:28 trtpg/__main__.py
--rw-rw-r--  2.0 unx     4088 b- defN 23-Jun-26 03:16 trtpg/config.py
--rw-rw-r--  2.0 unx     8237 b- defN 23-Jun-26 04:24 trtpg/extract_unsupported_operators.py
--rw-rw-r--  2.0 unx    25739 b- defN 23-Jun-26 04:57 trtpg/generate.py
--rw-rw-r--  2.0 unx     1438 b- defN 23-Jun-26 03:16 trtpg/log.py
--rw-rw-r--  2.0 unx     4370 b- defN 23-Jun-26 04:26 trtpg/readme.md
--rw-rw-r--  2.0 unx     2646 b- defN 23-Jun-26 04:24 trtpg/yaml_parser.py
--rw-rw-r--  2.0 unx    49231 b- defN 23-Jun-26 03:16 trtpg/doc/config.png
--rw-rw-r--  2.0 unx     4373 b- defN 23-Jun-26 03:16 trtpg/doc/edit_yaml_config.md
--rw-rw-r--  2.0 unx    19016 b- defN 23-Jun-26 03:16 trtpg/doc/onnx.png
--rw-rw-r--  2.0 unx     9401 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.cpp
--rw-rw-r--  2.0 unx     4895 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2DynamicExt.h
--rw-rw-r--  2.0 unx     8977 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.cpp
--rw-rw-r--  2.0 unx     4706 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/IPluginV2IOExt.h
--rw-rw-r--  2.0 unx     1381 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/license.template
--rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/makefile
--rw-rw-r--  2.0 unx     1976 b- defN 23-Jun-26 03:16 trtpg/plugin_templates/supported_operator_trt84.txt
--rw-rw-r--  2.0 unx     1532 b- defN 23-Jun-26 03:16 trtpg/samples/readme.md
--rw-rw-r--  2.0 unx     5750 b- defN 23-Jun-26 03:16 trtpg/samples/sample.yml
--rw-rw-r--  2.0 unx     8606 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/README.md
--rw-rw-r--  2.0 unx      749 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/efficientdet.yml
--rw-rw-r--  2.0 unx     1528 b- defN 23-Jun-26 03:16 trtpg/samples/efficientdet/modify_onnx.py
--rw-rw-r--  2.0 unx     7574 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/README.md
--rw-rw-r--  2.0 unx     1618 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/modify_onnx.py
--rw-rw-r--  2.0 unx      423 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet.yml
--rw-rw-r--  2.0 unx      439 b- defN 23-Jun-26 03:16 trtpg/samples/onnx_packnet/onnx_packnet_modified.yml
--rw-rw-r--  2.0 unx     5322 b- defN 23-Jun-26 03:16 trtpg/samples/pointpillar/README.md
--rw-rw-r--  2.0 unx      632 b- defN 23-Jun-26 03:16 trtpg/samples/pointpillar/pointpillar.yml
--rw-rw-r--  2.0 unx     6995 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/README.md
--rw-rw-r--  2.0 unx     1537 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py
--rw-rw-r--  2.0 unx      246 b- defN 23-Jun-26 03:16 trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/README.md
--rw-rw-r--  2.0 unx     1553 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/modify_onnx.py
--rw-rw-r--  2.0 unx      798 b- defN 23-Jun-26 03:16 trtpg/samples/yolov4/yolov4.yml
--rw-rw-r--  2.0 unx     5860 b- defN 23-Jun-26 03:16 trtpg/tests/generate_fake_onnx_from_yml.py
--rw-rw-r--  2.0 unx     3926 b- defN 23-Jun-26 03:16 trtpg/tests/test.yml
--rw-rw-r--  2.0 unx      312 b- defN 23-Jun-26 05:44 trtpg-1.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 05:44 trtpg-1.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       46 b- defN 23-Jun-26 05:44 trtpg-1.0.8.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Jun-26 05:44 trtpg-1.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3885 b- defN 23-Jun-26 05:44 trtpg-1.0.8.dist-info/RECORD
-44 files, 224331 bytes uncompressed, 111825 bytes compressed:  50.2%
+Zip file size: 32340 bytes, number of entries: 20
+-rw-r--r--  2.0 unx     1188 b- defN 23-Jun-29 08:06 tpg/__init__.py
+-rw-r--r--  2.0 unx     4088 b- defN 23-Jun-29 08:06 tpg/config.py
+-rw-r--r--  2.0 unx     8136 b- defN 23-Jun-29 08:06 tpg/extract_unsupported_operators.py
+-rw-r--r--  2.0 unx    25587 b- defN 23-Jun-29 08:06 tpg/generate.py
+-rw-r--r--  2.0 unx     1438 b- defN 23-Jun-29 08:06 tpg/log.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-Jun-29 08:06 tpg/tpg.py
+-rw-r--r--  2.0 unx     2652 b- defN 23-Jun-29 08:06 tpg/yaml_parser.py
+-rw-r--r--  2.0 unx     9401 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2DynamicExt.cpp
+-rw-r--r--  2.0 unx     4895 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2DynamicExt.h
+-rw-r--r--  2.0 unx     8977 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2IOExt.cpp
+-rw-r--r--  2.0 unx     4706 b- defN 23-Jun-29 08:06 tpg/plugin_templates/IPluginV2IOExt.h
+-rw-r--r--  2.0 unx     1381 b- defN 23-Jun-29 08:06 tpg/plugin_templates/license.template
+-rw-r--r--  2.0 unx     1772 b- defN 23-Jun-29 08:06 tpg/plugin_templates/makefile
+-rw-r--r--  2.0 unx     1976 b- defN 23-Jun-29 08:06 tpg/plugin_templates/supported_operator_trt84.txt
+-rw-r--r--  2.0 unx     1084 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5050 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1664 b- defN 23-Jun-30 02:05 trtpg-1.1.0.dist-info/RECORD
+20 files, 88329 bytes uncompressed, 29630 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,133 +1,61 @@
-Filename: trtpg/LICENSE.md
+Filename: tpg/__init__.py
 Comment: 
 
-Filename: trtpg/VERSION
+Filename: tpg/config.py
 Comment: 
 
-Filename: trtpg/__init__.py
+Filename: tpg/extract_unsupported_operators.py
 Comment: 
 
-Filename: trtpg/__main__.py
+Filename: tpg/generate.py
 Comment: 
 
-Filename: trtpg/config.py
+Filename: tpg/log.py
 Comment: 
 
-Filename: trtpg/extract_unsupported_operators.py
+Filename: tpg/tpg.py
 Comment: 
 
-Filename: trtpg/generate.py
+Filename: tpg/yaml_parser.py
 Comment: 
 
-Filename: trtpg/log.py
+Filename: tpg/plugin_templates/IPluginV2DynamicExt.cpp
 Comment: 
 
-Filename: trtpg/readme.md
+Filename: tpg/plugin_templates/IPluginV2DynamicExt.h
 Comment: 
 
-Filename: trtpg/yaml_parser.py
+Filename: tpg/plugin_templates/IPluginV2IOExt.cpp
 Comment: 
 
-Filename: trtpg/doc/config.png
+Filename: tpg/plugin_templates/IPluginV2IOExt.h
 Comment: 
 
-Filename: trtpg/doc/edit_yaml_config.md
+Filename: tpg/plugin_templates/license.template
 Comment: 
 
-Filename: trtpg/doc/onnx.png
+Filename: tpg/plugin_templates/makefile
 Comment: 
 
-Filename: trtpg/plugin_templates/IPluginV2DynamicExt.cpp
+Filename: tpg/plugin_templates/supported_operator_trt84.txt
 Comment: 
 
-Filename: trtpg/plugin_templates/IPluginV2DynamicExt.h
+Filename: trtpg-1.1.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: trtpg/plugin_templates/IPluginV2IOExt.cpp
+Filename: trtpg-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: trtpg/plugin_templates/IPluginV2IOExt.h
+Filename: trtpg-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: trtpg/plugin_templates/license.template
+Filename: trtpg-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: trtpg/plugin_templates/makefile
+Filename: trtpg-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: trtpg/plugin_templates/supported_operator_trt84.txt
-Comment: 
-
-Filename: trtpg/samples/readme.md
-Comment: 
-
-Filename: trtpg/samples/sample.yml
-Comment: 
-
-Filename: trtpg/samples/efficientdet/README.md
-Comment: 
-
-Filename: trtpg/samples/efficientdet/efficientdet.yml
-Comment: 
-
-Filename: trtpg/samples/efficientdet/modify_onnx.py
-Comment: 
-
-Filename: trtpg/samples/onnx_packnet/README.md
-Comment: 
-
-Filename: trtpg/samples/onnx_packnet/modify_onnx.py
-Comment: 
-
-Filename: trtpg/samples/onnx_packnet/onnx_packnet.yml
-Comment: 
-
-Filename: trtpg/samples/onnx_packnet/onnx_packnet_modified.yml
-Comment: 
-
-Filename: trtpg/samples/pointpillar/README.md
-Comment: 
-
-Filename: trtpg/samples/pointpillar/pointpillar.yml
-Comment: 
-
-Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/README.md
-Comment: 
-
-Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/modify_onnx.py
-Comment: 
-
-Filename: trtpg/samples/sampleOnnxMnistCoordConvAC/sampleOnnxMnistCoordConvAC.yml
-Comment: 
-
-Filename: trtpg/samples/yolov4/README.md
-Comment: 
-
-Filename: trtpg/samples/yolov4/modify_onnx.py
-Comment: 
-
-Filename: trtpg/samples/yolov4/yolov4.yml
-Comment: 
-
-Filename: trtpg/tests/generate_fake_onnx_from_yml.py
-Comment: 
-
-Filename: trtpg/tests/test.yml
-Comment: 
-
-Filename: trtpg-1.0.8.dist-info/METADATA
-Comment: 
-
-Filename: trtpg-1.0.8.dist-info/WHEEL
-Comment: 
-
-Filename: trtpg-1.0.8.dist-info/entry_points.txt
-Comment: 
-
-Filename: trtpg-1.0.8.dist-info/top_level.txt
-Comment: 
-
-Filename: trtpg-1.0.8.dist-info/RECORD
+Filename: trtpg-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `trtpg/LICENSE.md` & `trtpg-1.1.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `trtpg/__init__.py` & `tpg/__init__.py`

 * *Files identical despite different names*

## Comparing `trtpg/__main__.py` & `tpg/tpg.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,47 +15,50 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
+
 import argparse
+
 import sys
-from trtpg.extract_unsupported_operators import generate_yaml
-from trtpg.generate import *
+import os
+from tpg.extract_unsupported_operators import generate_yaml
+from tpg.generate import *
 
 class MyParser(argparse.ArgumentParser):
     def error(self, message):
         sys.stderr.write('error: %s\n' % message)
         self.print_help()
         sys.exit(2)
 
 def main():
     parser = MyParser()
-    subparsers = parser.add_subparsers(dest="func")
+    subparsers = parser.add_subparsers(dest='func')
     parser_extract = subparsers.add_parser("extract", help="generate yml from onnx")
-    parser_extract.add_argument("--onnx", type=str, default="Required Onnx File",
+    parser_extract.add_argument("--onnx", type=str, default='',
                         help="onnx for extraction")
     parser_extract.add_argument("--custom_operators", type=str, default='',
                         help="user-specify custom operator, split by \",\"")
     parser_extract.add_argument("--io_tensors", nargs='+',
                         help="specify io tensor explicitly so that you don't edit the yaml file.\
                         usage: --io_tensors op_name_1:1x1x1x1,2x2x2,-1x-1x-1:7x7x7,-1x-1 op_name_2:inputs_shapes:output_shapes")
     parser_extract.add_argument("--format_combinations", nargs='+',
                         help="specify support format combination explicitly so that you don't edit the yaml file.\
                         usage: --format_combinations op_name_1:float32+int8+int8,float16+int8+int8 op_name_2:support_format_combination_str")
-    parser_extract.add_argument("--yaml", type=str, default='Required Yaml File',
+    parser_extract.add_argument("--yaml", type=str, default='',
                         help="output yaml")
     parser_extract.add_argument("--trt_version", type=str, default='8.4',
                         help="filter unsupported op based on the version")
     parser_extract.set_defaults(func=generate_yaml)
 
     parser_generate = subparsers.add_parser("generate", help="generate plugin codes from yml")
-    parser_generate.add_argument("--yaml", type=str, default='Required Yaml File',
+    parser_generate.add_argument("--yaml", type=str, default='',
                         help="output yaml config")
     parser_generate.add_argument("--no_makefile", action='store_false',
                         help="don't generate make file")
     parser_generate.add_argument("--trt_lib_dir", type=str, default=DEFAULT_TRT_LIB_DIR,
                         help="directory contains the libnvinfer_plugin.so")
     parser_generate.add_argument("--trt_include_dir", type=str, default=DEFAULT_TRT_INCLUDE_DIR,
                         help="directory contains the NvInferPlugin.h")
@@ -63,16 +66,16 @@
                         help="CUDA include path")
     parser_generate.add_argument("-o", "--output", type=str, default='./',
                         help="output directory which the generated plugin directory located")
     parser_generate.add_argument("--print", action='store_true',
                         help="to print the generate h, cpp and makefile to console")
     parser_generate.set_defaults(func=generate)
     args = parser.parse_args()
+
     if args.func is None:
         parser.print_help()
-        return 1
-    
+        exit()
+
     args.func(args)
-    return 0
 
 if __name__ == "__main__":
     main()
```

## Comparing `trtpg/config.py` & `tpg/config.py`

 * *Files identical despite different names*

## Comparing `trtpg/extract_unsupported_operators.py` & `tpg/extract_unsupported_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from .log import *
+from tpg.log import *
+
+import argparse
+import os
+import sys
+import onnx
+import numpy as np
+import yaml
 
 try:
     import onnx_graphsurgeon as gs
 except ModuleNotFoundError as e:
     print("Automatic installing onnx_graphsurgeon.")
     import pip
     pip.main("install onnx_graphsurgeon --index-url https://pypi.ngc.nvidia.com".split(" "))
     import onnx_graphsurgeon as gs
 
-import argparse
-import os
-import sys
-import onnx
-import numpy as np
-import yaml
-
 template_dir = os.path.dirname(os.path.realpath(__file__)) + "/plugin_templates/"
 def get_supported_op_list(version):
     op_lists = []
     if version == '8.4':
         with open(os.path.join(template_dir, "supported_operator_trt84.txt")) as f:
             lines = f.readlines()
             for line in lines:
@@ -173,19 +173,14 @@
     return format_combinations
 
 def write_custom_format_combinations(d, format_combinations):
     for op_name in format_combinations:
         d[op_name]["support_format_combination"] = format_combinations[op_name]["support_format_combination"]
 
 def generate_yaml(args):
-
-    if not os.path.exists(args.onnx):
-        print(f"Not exists file: {args.onnx}")
-        return 1
-
     graph = gs.import_onnx(onnx.load(args.onnx))
     d = {}
     op_parsed = []
     if args.custom_operators != "":
         target_nodes = args.custom_operators.split(",")
         for node in graph.nodes:
             if node.op in op_parsed:
```

## Comparing `trtpg/generate.py` & `tpg/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
-from .config import *
-from .log import *
-from .yaml_parser import read_yaml
+from tpg.config import *
+from tpg.log import *
+from tpg.yaml_parser import read_yaml
 
 import os
 import sys
 import shutil
 from string import Template
 import argparse
 import re
@@ -594,19 +594,16 @@
 
     if args.print:
         print(h)
         print(cpp)
         print(makefile)
 
 def generate(args):
-    if not os.path.exists(args.yaml):
-        if args.yaml == "@sample":
-            args.yaml = os.path.join(os.path.dirname(os.path.realpath(__file__)), "samples", "sample.yml")
-        else:
-            print(f"Not exists file: {args.yaml}")
-            return 1
-    
-    configs = read_yaml(args.yaml)
+    configs = None
+    if args.yaml != '':
+        configs = read_yaml(args.yaml)
+    else:
+        assert False, 'must provide the yaml config'
     for config in configs:
         codegen(config, args)
```

## Comparing `trtpg/log.py` & `tpg/log.py`

 * *Files identical despite different names*

## Comparing `trtpg/readme.md` & `trtpg-1.1.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,61 @@
+Metadata-Version: 2.1
+Name: trtpg
+Version: 1.1.0
+Summary: Generate TensorRT plugin in fly
+Home-page: https://github.com/NVIDIA-AI-IOT/tensorrt_plugin_generator
+Author-email: cntse@nvidia.com
+License: UNKNOWN
+Keywords: tensorrt plugin generator
+Platform: linux
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: pyyaml
+Requires-Dist: numpy
+Requires-Dist: onnx
+
 # TPG: TensorRT Plugin Generator
 
 - [TPG: TensorRT Plugin Generator](#tpg-tensorrt-plugin-generator)
   - [1. Installation](#1-installation)
+    - [1.1 Install from source code](#11-install-from-source-code)
+    - [1.2 install from pypi](#12-install-from-pypi)
   - [2. Usage](#2-usage)
     - [2.1 Generate plugin yaml for Unsupported Operators](#21-generate-plugin-yaml-for-unsupported-operators)
     - [2.2 Complete the yaml config](#22-complete-the-yaml-config)
     - [2.3 Generate Plugin Codes From the plugin yaml](#23-generate-plugin-codes-from-the-plugin-yaml)
     - [2.4 Finish The Plugin Inference Kennel](#24-finish-the-plugin-inference-kennel)
   - [3. Best Practice](#3-best-practice)
 
 TPG is a tool that can quickly generate the plugin code(**NOT INCLUDE THE INFERENCE KERNEL IMPLEMENTATION**) for TensorRT unsupported operators. the user only need to focus on the plugin kernel implementation and doesn't need to worry about how does TensorRT plugin works or how to use the plugin API.
 ## 1. Installation
 
+### 1.1 Install from source code
+
 ```
 git clone https://github.com/NVIDIA-AI-IOT/tensorrt_plugin_generator
 cd trt-plugin-generator
-pip3 install pyyaml
+python3 setup.py install
+```
+
+### 1.2 install from pypi
+
+```
+pip3 install trtpg
 ```
 
 ## 2. Usage
 
 ### 2.1 Generate plugin yaml for Unsupported Operators
 
 
 ```
-python tpg.py extract --onnx model.onnx --custom_operators custom_add,custom_conv --yaml plugin.yml
+trtpg extract --onnx model.onnx --custom_operators custom_add,custom_conv --yaml plugin.yml
 ```
 ![onnx.png](./doc/onnx.png)
 
 ### 2.2 Complete the yaml config
 
 User still need to edit the generated YAML file to specify some information explicitly since TPG can not deduce them from onnx directly or it depends on how the plugin works while TPG know nothing about it. All the items need user to specify has marked as "need_user_to_specify".
 
@@ -42,20 +69,20 @@
 For more information, you can refer to [how to edit the yaml](./doc/edit_yaml_config.md). also TPG will throw assertion error if you make mistakes in the config yaml.
 
 ### 2.3 Generate Plugin Codes From the plugin yaml
 
 Once we have a valid yaml file, we can generate the plugin code all in once now:
 
 ```
-python tpg.py generate plugin.yml --output ./plugin_codes
+trtpg generate --yaml plugin.yml --output ./plugin_codes
 ```
 
 For more options(e.g. to specify the trt library path):
 ```
-python tpg.py generate -h
+trtpg generate -h
 ```
 
 We can see the generated plugin codes under ./plugin_codes. with a Makefile that can be used for compile a minimal dynamic library.
 
 The compiled library can be loaded with `trtexec --plugins=libMyFancyPlugin.so` or be loaded with dlopen(refer to [link](https://github.com/NVIDIA/TensorRT/blob/b55c4710ce01f076c26710a48879fcb2661be4a9/samples/common/common.h#L893)).
 
 ### 2.4 Finish The Plugin Inference Kennel
@@ -74,7 +101,9 @@
 
 For the detailed usage of TPG, you can refer to our [samples](./samples/readme.md)
 
 More tips:
 - Enable DEBUG_PLUGIN micro at the start of the generated cpp file so that you can catch call log of the plugin API, it's enable by default.
 - provide more information in the yaml as much as possible so that TPG can take the work for you, e.g. if you know your plugin's output is -1x1x1, then specify it -1x1x1 is better than -1x-1x-1, the latter will require you to handle extra unknown dimensions.
 
+
+
```

## Comparing `trtpg/yaml_parser.py` & `tpg/yaml_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 import yaml
-from .config import *
-from .log import *
+from tpg.config import *
+from tpg.log import *
 
 def read_yaml(path):
     configs = []
     with open(path, 'r') as stream:
         logging.info('load yaml: ' + path)
         data = yaml.safe_load(stream)
         for node_name in data:
```

## Comparing `trtpg/plugin_templates/IPluginV2DynamicExt.cpp` & `tpg/plugin_templates/IPluginV2DynamicExt.cpp`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/IPluginV2DynamicExt.h` & `tpg/plugin_templates/IPluginV2DynamicExt.h`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/IPluginV2IOExt.cpp` & `tpg/plugin_templates/IPluginV2IOExt.cpp`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/IPluginV2IOExt.h` & `tpg/plugin_templates/IPluginV2IOExt.h`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/license.template` & `tpg/plugin_templates/license.template`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/makefile` & `tpg/plugin_templates/makefile`

 * *Files identical despite different names*

## Comparing `trtpg/plugin_templates/supported_operator_trt84.txt` & `tpg/plugin_templates/supported_operator_trt84.txt`

 * *Files identical despite different names*

