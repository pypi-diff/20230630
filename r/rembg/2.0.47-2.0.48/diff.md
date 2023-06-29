# Comparing `tmp/rembg-2.0.47.tar.gz` & `tmp/rembg-2.0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rembg-2.0.47.tar", last modified: Wed Jun 21 17:29:54 2023, max compression
+gzip compressed data, was "rembg-2.0.48.tar", last modified: Thu Jun 29 23:48:04 2023, max compression
```

## Comparing `rembg-2.0.47.tar` & `rembg-2.0.48.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-21 17:28:48.000000 rembg-2.0.47/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-21 17:28:48.000000 rembg-2.0.47/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 17:29:54.925344 rembg-2.0.47/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-21 17:28:48.000000 rembg-2.0.47/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-21 17:28:48.000000 rembg-2.0.47/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/bg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/b_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/i_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/p_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/commands/s_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/session_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg/sessions/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/dis_anime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/dis_general_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/silueta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net_cloth_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2net_human_seg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-21 17:28:48.000000 rembg-2.0.47/rembg/sessions/u2netp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/rembg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 17:29:54.000000 rembg-2.0.47/rembg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-21 17:29:54.925344 rembg-2.0.47/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-21 17:28:48.000000 rembg-2.0.47/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:29:54.925344 rembg-2.0.47/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-21 17:28:48.000000 rembg-2.0.47/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-21 17:28:48.000000 rembg-2.0.47/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-29 23:46:48.000000 rembg-2.0.48/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-29 23:46:48.000000 rembg-2.0.48/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 23:48:04.068781 rembg-2.0.48/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-06-29 23:46:48.000000 rembg-2.0.48/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-29 23:46:48.000000 rembg-2.0.48/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.072781 rembg-2.0.48/rembg/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-29 23:48:04.072781 rembg-2.0.48/rembg/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/bg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/b_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/i_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/p_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/commands/s_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/session_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg/sessions/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/dis_anime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/dis_general_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5394 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/silueta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_cloth_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2net_human_seg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-29 23:46:48.000000 rembg-2.0.48/rembg/sessions/u2netp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/rembg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 23:48:04.000000 rembg-2.0.48/rembg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-29 23:48:04.072781 rembg-2.0.48/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-29 23:46:48.000000 rembg-2.0.48/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 23:48:04.068781 rembg-2.0.48/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-29 23:46:48.000000 rembg-2.0.48/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-29 23:46:48.000000 rembg-2.0.48/versioneer.py
```

### Comparing `rembg-2.0.47/LICENSE.txt` & `rembg-2.0.48/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/PKG-INFO` & `rembg-2.0.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.47
+Version: 2.0.48
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -188,14 +188,18 @@
 
 Passing extras parameters
 
 ```
 rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
 ```
 
+```
+rembg i -m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -336,15 +340,15 @@
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
 -   isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
 -   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### How to train your own model
 
-If You need more fine tunned models try this:
+If You need more fine tuned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289
 
 
 ## Some video tutorials
 
 - https://www.youtube.com/watch?v=3xqwpXjxyMQ
 - https://www.youtube.com/watch?v=dFKRGXdkGJU
```

### Comparing `rembg-2.0.47/README.md` & `rembg-2.0.48/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,18 @@
 
 Passing extras parameters
 
 ```
 rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
 ```
 
+```
+rembg i -m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -308,15 +312,15 @@
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
 -   isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
 -   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### How to train your own model
 
-If You need more fine tunned models try this:
+If You need more fine tuned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289
 
 
 ## Some video tutorials
 
 - https://www.youtube.com/watch?v=3xqwpXjxyMQ
 - https://www.youtube.com/watch?v=dFKRGXdkGJU
```

#### html2text {}

```diff
@@ -59,86 +59,87 @@
 input.png | rembg i > output.png ``` Remove the background from a local file
 ``` rembg i path/to/input.png path/to/output.png ``` Remove the background
 specifying a model ``` rembg i -m u2netp path/to/input.png path/to/output.png
 ``` Remove the background returning only the mask ``` rembg i -om path/to/
 input.png path/to/output.png ``` Remove the background applying an alpha
 matting ``` rembg i -a path/to/input.png path/to/output.png ``` Passing extras
 parameters ``` rembg i -m sam -x '{"input_labels": [1], "input_points": [
-[100,100]]}' path/to/input.png path/to/output.png ``` ### rembg `p` Used when
-input and output are folders. Remove the background from all images in a folder
-``` rembg p path/to/input path/to/output ``` Same as before, but watching for
-new/changed files to process ``` rembg p -w path/to/input path/to/output ```
-### rembg `s` Used to start http server. To see the complete endpoints
-documentation, go to: `http://localhost:5000/api`. Remove the background from
-an image url ``` curl -s "http://localhost:5000/api/remove?url=http://
-input.png" -o output.png ``` Remove the background from an uploaded image ```
-curl -s -F file=@/path/to/input.jpg "http://localhost:5000/api/remove" -
-o output.png ``` ### rembg `b` Process a sequence of RGB24 images from stdin.
-This is intended to be used with another program, such as FFMPEG, that outputs
-RGB24 pixel data to stdout, which is piped into the stdin of this program,
-although nothing prevents you from manually typing in images at stdin. ```
-rembg b image_width image_height -o output_specifier ``` Arguments: -
-image_width : width of input image(s) - image_height : height of input image(s)
-- output_specifier: printf-style specifier for output filenames, for example if
-`output-%03u.png`, then output files will be named `output-000.png`, `output-
-001.png`, `output-002.png`, etc. Output files will be saved in PNG format
-regardless of the extension specified. You can omit it to write results to
-stdout. Example usage with FFMPEG: ``` ffmpeg -i input.mp4 -ss 10 -an -
-f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280 720 -o folder/output-%03u.png
-``` The width and height values must match the dimension of output images from
-FFMPEG. Note for FFMPEG, the "`-an -f rawvideo -pix_fmt rgb24 pipe:1`" part is
-required for the whole thing to work. ## Usage as a library Input and output as
-bytes ```python from rembg import remove input_path = 'input.png' output_path =
-'output.png' with open(input_path, 'rb') as i: with open(output_path, 'wb') as
-o: input = i.read() output = remove(input) o.write(output) ``` Input and output
-as a PIL image ```python from rembg import remove from PIL import Image
-input_path = 'input.png' output_path = 'output.png' input = Image.open
-(input_path) output = remove(input) output.save(output_path) ``` Input and
-output as a numpy array ```python from rembg import remove import cv2
-input_path = 'input.png' output_path = 'output.png' input = cv2.imread
-(input_path) output = remove(input) cv2.imwrite(output_path, output) ``` How to
-iterate over files in a performatic way ```python from pathlib import Path from
-rembg import remove, new_session session = new_session() for file in Path
-('path/to/folder').glob('*.png'): input_path = str(file) output_path = str
-(file.parent / (file.stem + ".out.png")) with open(input_path, 'rb') as i: with
-open(output_path, 'wb') as o: input = i.read() output = remove(input,
-session=session) o.write(output) ``` To see a full list of examples on how to
-use rembg, go to the [examples](USAGE.md) page. ## Usage as a docker Just
-replace the `rembg` command for `docker run danielgatis/rembg`. Try this: ```
-docker run danielgatis/rembg i path/to/input.png path/to/output.png ``` ##
-Models All models are downloaded and saved in the user home folder in the
-`.u2net` directory. The available models are: - u2net ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx), [source]
-(https://github.com/xuebinqin/U-2-Net)): A pre-trained model for general use
-cases. - u2netp ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/u2netp.onnx), [source](https://github.com/xuebinqin/U-2-Net)):
-A lightweight version of u2net model. - u2net_human_seg ([download](https://
-github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx),
-[source](https://github.com/xuebinqin/U-2-Net)): A pre-trained model for human
-segmentation. - u2net_cloth_seg ([download](https://github.com/danielgatis/
-rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx), [source](https://
-github.com/levindabhi/cloth-segmentation)): A pre-trained model for Cloths
-Parsing from human portrait. Here clothes are parsed into 3 category: Upper
-body, Lower body and Full body. - silueta ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://
-github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is
-reduced to 43Mb. - isnet-general-use ([download](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source]
-(https://github.com/xuebinqin/DIS)): A new pre-trained model for general use
-cases. - isnet-anime ([download](https://github.com/danielgatis/rembg/releases/
-download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-
-segmentation)): A high-accuracy segmentation for anime character. - sam (
-[download encoder](https://github.com/danielgatis/rembg/releases/download/
-v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/
-danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source]
-(https://github.com/facebookresearch/segment-anything)): A pre-trained model
-for any use cases. ### How to train your own model If You need more fine tunned
-models try this: https://github.com/danielgatis/rembg/issues/193#issuecomment-
-1055534289 ## Some video tutorials - https://www.youtube.com/
-watch?v=3xqwpXjxyMQ - https://www.youtube.com/watch?v=dFKRGXdkGJU - https://
-www.youtube.com/watch?v=Ai-BS_T7yjE - https://www.youtube.com/
-watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=D7W-C0urVcQ ## References
-- https://arxiv.org/pdf/2005.09007.pdf - https://github.com/NathanUA/U-2-Net -
-https://github.com/pymatting/pymatting ## Buy me a coffee Liked some of my
-work? Buy me a coffee (or more likely a beer) [Buy_Me_A_Coffee] ## License
-Copyright (c) 2020-present [Daniel Gatis](https://github.com/danielgatis)
-Licensed under [MIT License](./LICENSE.txt)
+[100,100]]}' path/to/input.png path/to/output.png ``` ``` rembg i -
+m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png
+path/to/output.png ``` ### rembg `p` Used when input and output are folders.
+Remove the background from all images in a folder ``` rembg p path/to/input
+path/to/output ``` Same as before, but watching for new/changed files to
+process ``` rembg p -w path/to/input path/to/output ``` ### rembg `s` Used to
+start http server. To see the complete endpoints documentation, go to: `http://
+localhost:5000/api`. Remove the background from an image url ``` curl -s "http:
+//localhost:5000/api/remove?url=http://input.png" -o output.png ``` Remove the
+background from an uploaded image ``` curl -s -F file=@/path/to/input.jpg
+"http://localhost:5000/api/remove" -o output.png ``` ### rembg `b` Process a
+sequence of RGB24 images from stdin. This is intended to be used with another
+program, such as FFMPEG, that outputs RGB24 pixel data to stdout, which is
+piped into the stdin of this program, although nothing prevents you from
+manually typing in images at stdin. ``` rembg b image_width image_height -
+o output_specifier ``` Arguments: - image_width : width of input image(s) -
+image_height : height of input image(s) - output_specifier: printf-style
+specifier for output filenames, for example if `output-%03u.png`, then output
+files will be named `output-000.png`, `output-001.png`, `output-002.png`, etc.
+Output files will be saved in PNG format regardless of the extension specified.
+You can omit it to write results to stdout. Example usage with FFMPEG: ```
+ffmpeg -i input.mp4 -ss 10 -an -f rawvideo -pix_fmt rgb24 pipe:1 | rembg b 1280
+720 -o folder/output-%03u.png ``` The width and height values must match the
+dimension of output images from FFMPEG. Note for FFMPEG, the "`-an -f rawvideo
+-pix_fmt rgb24 pipe:1`" part is required for the whole thing to work. ## Usage
+as a library Input and output as bytes ```python from rembg import remove
+input_path = 'input.png' output_path = 'output.png' with open(input_path, 'rb')
+as i: with open(output_path, 'wb') as o: input = i.read() output = remove
+(input) o.write(output) ``` Input and output as a PIL image ```python from
+rembg import remove from PIL import Image input_path = 'input.png' output_path
+= 'output.png' input = Image.open(input_path) output = remove(input)
+output.save(output_path) ``` Input and output as a numpy array ```python from
+rembg import remove import cv2 input_path = 'input.png' output_path =
+'output.png' input = cv2.imread(input_path) output = remove(input) cv2.imwrite
+(output_path, output) ``` How to iterate over files in a performatic way
+```python from pathlib import Path from rembg import remove, new_session
+session = new_session() for file in Path('path/to/folder').glob('*.png'):
+input_path = str(file) output_path = str(file.parent / (file.stem +
+".out.png")) with open(input_path, 'rb') as i: with open(output_path, 'wb') as
+o: input = i.read() output = remove(input, session=session) o.write(output) ```
+To see a full list of examples on how to use rembg, go to the [examples]
+(USAGE.md) page. ## Usage as a docker Just replace the `rembg` command for
+`docker run danielgatis/rembg`. Try this: ``` docker run danielgatis/rembg i
+path/to/input.png path/to/output.png ``` ## Models All models are downloaded
+and saved in the user home folder in the `.u2net` directory. The available
+models are: - u2net ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net.onnx), [source](https://github.com/xuebinqin/U-2-Net)): A
+pre-trained model for general use cases. - u2netp ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx), [source]
+(https://github.com/xuebinqin/U-2-Net)): A lightweight version of u2net model.
+- u2net_human_seg ([download](https://github.com/danielgatis/rembg/releases/
+download/v0.0.0/u2net_human_seg.onnx), [source](https://github.com/xuebinqin/U-
+2-Net)): A pre-trained model for human segmentation. - u2net_cloth_seg (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/
+u2net_cloth_seg.onnx), [source](https://github.com/levindabhi/cloth-
+segmentation)): A pre-trained model for Cloths Parsing from human portrait.
+Here clothes are parsed into 3 category: Upper body, Lower body and Full body.
+- silueta ([download](https://github.com/danielgatis/rembg/releases/download/
+v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/
+295)): Same as u2net but the size is reduced to 43Mb. - isnet-general-use (
+[download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-
+general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-
+trained model for general use cases. - isnet-anime ([download](https://
+github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx),
+[source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy
+segmentation for anime character. - sam ([download encoder](https://github.com/
+danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download
+decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-
+decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-
+anything)): A pre-trained model for any use cases. ### How to train your own
+model If You need more fine tuned models try this: https://github.com/
+danielgatis/rembg/issues/193#issuecomment-1055534289 ## Some video tutorials -
+https://www.youtube.com/watch?v=3xqwpXjxyMQ - https://www.youtube.com/
+watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=Ai-BS_T7yjE - https://
+www.youtube.com/watch?v=dFKRGXdkGJU - https://www.youtube.com/watch?v=D7W-
+C0urVcQ ## References - https://arxiv.org/pdf/2005.09007.pdf - https://
+github.com/NathanUA/U-2-Net - https://github.com/pymatting/pymatting ## Buy me
+a coffee Liked some of my work? Buy me a coffee (or more likely a beer) [Buy_Me
+A_Coffee] ## License Copyright (c) 2020-present [Daniel Gatis](https://
+github.com/danielgatis) Licensed under [MIT License](./LICENSE.txt)
```

### Comparing `rembg-2.0.47/rembg/bg.py` & `rembg-2.0.48/rembg/bg.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/rembg/cli.py` & `rembg-2.0.48/rembg/cli.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/rembg/commands/b_command.py` & `rembg-2.0.48/rembg/commands/b_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     **kwargs
 ) -> None:
     try:
         kwargs.update(json.loads(extras))
     except Exception:
         pass
 
-    session = new_session(model)
+    session = new_session(model, **kwargs)
     bytes_per_img = image_width * image_height * 3
 
     if output_specifier:
         output_dir = os.path.dirname(
             os.path.abspath(os.path.expanduser(output_specifier))
         )
```

### Comparing `rembg-2.0.47/rembg/commands/i_command.py` & `rembg-2.0.48/rembg/commands/i_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 )
 def i_command(model: str, extras: str, input: IO, output: IO, **kwargs) -> None:
     try:
         kwargs.update(json.loads(extras))
     except Exception:
         pass
 
-    output.write(remove(input.read(), session=new_session(model), **kwargs))
+    output.write(remove(input.read(), session=new_session(model, **kwargs), **kwargs))
```

### Comparing `rembg-2.0.47/rembg/commands/p_command.py` & `rembg-2.0.48/rembg/commands/p_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     **kwargs,
 ) -> None:
     try:
         kwargs.update(json.loads(extras))
     except Exception:
         pass
 
-    session = new_session(model)
+    session = new_session(model, **kwargs)
 
     def process(each_input: pathlib.Path) -> None:
         try:
             mimetype = filetype.guess(each_input)
             if mimetype is None:
                 return
             if mimetype.mime.find("image") < 0:
```

### Comparing `rembg-2.0.47/rembg/commands/s_command.py` & `rembg-2.0.48/rembg/commands/s_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,15 +182,17 @@
                 kwargs.update(json.loads(commons.extras))
             except Exception:
                 pass
 
         return Response(
             remove(
                 content,
-                session=sessions.setdefault(commons.model, new_session(commons.model)),
+                session=sessions.setdefault(
+                    commons.model, new_session(commons.model, **kwargs)
+                ),
                 alpha_matting=commons.a,
                 alpha_matting_foreground_threshold=commons.af,
                 alpha_matting_background_threshold=commons.ab,
                 alpha_matting_erode_size=commons.ae,
                 only_mask=commons.om,
                 post_process_mask=commons.ppm,
                 bgcolor=commons.bgc,
@@ -241,40 +243,35 @@
             description="Image file (byte stream) that has to be processed.",
         ),
         commons: CommonQueryPostParams = Depends(),
     ):
         return await asyncify(im_without_bg)(file, commons)  # type: ignore
 
     def gr_app(app):
-        def inference(input_path, model):
+        def inference(input_path, model, cmd_args):
             output_path = "output.png"
+
+            kwargs = {}
+            if cmd_args:
+                kwargs.update(json.loads(cmd_args))
+            kwargs["session"] = new_session(model, **kwargs)
+
             with open(input_path, "rb") as i:
                 with open(output_path, "wb") as o:
                     input = i.read()
-                    output = remove(input, session=new_session(model))
+                    output = remove(input, **kwargs)
                     o.write(output)
             return os.path.join(output_path)
 
         interface = gr.Interface(
             inference,
             [
                 gr.components.Image(type="filepath", label="Input"),
-                gr.components.Dropdown(
-                    [
-                        "u2net",
-                        "u2netp",
-                        "u2net_human_seg",
-                        "u2net_cloth_seg",
-                        "silueta",
-                        "isnet-general-use",
-                        "isnet-anime",
-                    ],
-                    value="u2net",
-                    label="Models",
-                ),
+                gr.components.Dropdown(sessions_names, value="u2net", label="Models"),
+                gr.components.Textbox(label="Arguments"),
             ],
             gr.components.Image(type="filepath", label="Output"),
         )
 
         interface.queue(concurrency_count=3)
         app = gr.mount_gradio_app(app, interface, path="/")
         return app
```

### Comparing `rembg-2.0.47/rembg/session_factory.py` & `rembg-2.0.48/rembg/session_factory.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/rembg/sessions/__init__.py` & `rembg-2.0.48/rembg/sessions/__init__.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/rembg/sessions/base.py` & `rembg-2.0.48/rembg/sessions/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             for provider in providers:
                 if provider in _providers:
                     self.providers.append(provider)
         else:
             self.providers.extend(_providers)
 
         self.inner_session = ort.InferenceSession(
-            str(self.__class__.download_models()),
+            str(self.__class__.download_models(*args, **kwargs)),
             providers=self.providers,
             sess_options=sess_opts,
         )
 
     def normalize(
         self,
         img: PILImage,
```

### Comparing `rembg-2.0.47/rembg/sessions/dis_anime.py` & `rembg-2.0.48/rembg/sessions/u2net.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class DisSession(BaseSession):
+class U2netSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
-            self.normalize(img, (0.485, 0.456, 0.406), (1.0, 1.0, 1.0), (1024, 1024)),
+            self.normalize(
+                img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
+            ),
         )
 
         pred = ort_outs[0][:, 0, :, :]
 
         ma = np.max(pred)
         mi = np.min(pred)
 
@@ -27,23 +29,23 @@
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
-            else "md5:6f184e756bb3bd901c8849220a83e38e",
+            else "md5:60024c5c889badc19c04ad937298a77b",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "isnet-anime"
+        return "u2net"
```

### Comparing `rembg-2.0.47/rembg/sessions/dis_general_use.py` & `rembg-2.0.48/rembg/sessions/dis_general_use.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,23 +27,23 @@
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
             else "md5:fc16ebd8b0c10d971d3513d564d01e29",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "isnet-general-use"
```

### Comparing `rembg-2.0.47/rembg/sessions/sam.py` & `rembg-2.0.48/rembg/sessions/sam.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,16 +132,16 @@
             for i in range(masks.shape[0])
         ]
 
         return masks
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname_encoder = f"{cls.name()}_encoder.onnx"
-        fname_decoder = f"{cls.name()}_decoder.onnx"
+        fname_encoder = f"{cls.name(*args, **kwargs)}_encoder.onnx"
+        fname_decoder = f"{cls.name(*args, **kwargs)}_decoder.onnx"
 
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
             else "md5:13d97c5c79ab13ef86d67cbde5f1b250",
             fname=fname_encoder,
@@ -156,14 +156,14 @@
             else "md5:fa3d1c36a3187d3de1c8deebf33dd127",
             fname=fname_decoder,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
         return (
-            os.path.join(cls.u2net_home(), fname_encoder),
-            os.path.join(cls.u2net_home(), fname_decoder),
+            os.path.join(cls.u2net_home(*args, **kwargs), fname_encoder),
+            os.path.join(cls.u2net_home(*args, **kwargs), fname_decoder),
         )
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "sam"
```

### Comparing `rembg-2.0.47/rembg/sessions/silueta.py` & `rembg-2.0.48/rembg/sessions/silueta.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,12 +40,12 @@
             if cls.checksum_disabled(*args, **kwargs)
             else "md5:55e59e0d8062d2f5d013f4725ee84782",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "silueta"
```

### Comparing `rembg-2.0.47/rembg/sessions/u2net.py` & `rembg-2.0.48/rembg/sessions/u2netp.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class U2netSession(BaseSession):
+class U2netpSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
             self.normalize(
                 img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
             ),
         )
@@ -29,23 +29,23 @@
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net.onnx",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
-            else "md5:60024c5c889badc19c04ad937298a77b",
+            else "md5:8e83ca70e441ab06c318d82300c84806",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "u2net"
+        return "u2netp"
```

### Comparing `rembg-2.0.47/rembg/sessions/u2net_cloth_seg.py` & `rembg-2.0.48/rembg/sessions/u2net_cloth_seg.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,45 +5,45 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 from scipy.special import log_softmax
 
 from .base import BaseSession
 
-pallete1 = [
+palette1 = [
     0,
     0,
     0,
     255,
     255,
     255,
     0,
     0,
     0,
     0,
     0,
     0,
 ]
 
-pallete2 = [
+palette2 = [
     0,
     0,
     0,
     0,
     0,
     0,
     255,
     255,
     255,
     0,
     0,
     0,
 ]
 
-pallete3 = [
+palette3 = [
     0,
     0,
     0,
     0,
     0,
     0,
     0,
@@ -72,41 +72,41 @@
 
         mask = Image.fromarray(pred.astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         masks = []
 
         mask1 = mask.copy()
-        mask1.putpalette(pallete1)
+        mask1.putpalette(palette1)
         mask1 = mask1.convert("RGB").convert("L")
         masks.append(mask1)
 
         mask2 = mask.copy()
-        mask2.putpalette(pallete2)
+        mask2.putpalette(palette2)
         mask2 = mask2.convert("RGB").convert("L")
         masks.append(mask2)
 
         mask3 = mask.copy()
-        mask3.putpalette(pallete3)
+        mask3.putpalette(palette3)
         mask3 = mask3.convert("RGB").convert("L")
         masks.append(mask3)
 
         return masks
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_cloth_seg.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
             else "md5:2434d1f3cb744e0e49386c906e5a08bb",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "u2net_cloth_seg"
```

### Comparing `rembg-2.0.47/rembg/sessions/u2net_human_seg.py` & `rembg-2.0.48/rembg/sessions/u2net_human_seg.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,23 +29,23 @@
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
             "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2net_human_seg.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
             else "md5:c09ddc2e0104f800e3e1bb4652583d1f",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
         return "u2net_human_seg"
```

### Comparing `rembg-2.0.47/rembg/sessions/u2netp.py` & `rembg-2.0.48/rembg/sessions/dis_anime.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,21 +5,19 @@
 import pooch
 from PIL import Image
 from PIL.Image import Image as PILImage
 
 from .base import BaseSession
 
 
-class U2netpSession(BaseSession):
+class DisSession(BaseSession):
     def predict(self, img: PILImage, *args, **kwargs) -> List[PILImage]:
         ort_outs = self.inner_session.run(
             None,
-            self.normalize(
-                img, (0.485, 0.456, 0.406), (0.229, 0.224, 0.225), (320, 320)
-            ),
+            self.normalize(img, (0.485, 0.456, 0.406), (1.0, 1.0, 1.0), (1024, 1024)),
         )
 
         pred = ort_outs[0][:, 0, :, :]
 
         ma = np.max(pred)
         mi = np.min(pred)
 
@@ -29,23 +27,23 @@
         mask = Image.fromarray((pred * 255).astype("uint8"), mode="L")
         mask = mask.resize(img.size, Image.LANCZOS)
 
         return [mask]
 
     @classmethod
     def download_models(cls, *args, **kwargs):
-        fname = f"{cls.name()}.onnx"
+        fname = f"{cls.name(*args, **kwargs)}.onnx"
         pooch.retrieve(
-            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/u2netp.onnx",
+            "https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx",
             None
             if cls.checksum_disabled(*args, **kwargs)
-            else "md5:8e83ca70e441ab06c318d82300c84806",
+            else "md5:6f184e756bb3bd901c8849220a83e38e",
             fname=fname,
             path=cls.u2net_home(*args, **kwargs),
             progressbar=True,
         )
 
-        return os.path.join(cls.u2net_home(), fname)
+        return os.path.join(cls.u2net_home(*args, **kwargs), fname)
 
     @classmethod
     def name(cls, *args, **kwargs):
-        return "u2netp"
+        return "isnet-anime"
```

### Comparing `rembg-2.0.47/rembg.egg-info/PKG-INFO` & `rembg-2.0.48/rembg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rembg
-Version: 2.0.47
+Version: 2.0.48
 Summary: Remove image background
 Home-page: https://github.com/danielgatis/rembg
 Author: Daniel Gatis
 Author-email: danielgatis@gmail.com
 Keywords: remove,background,u2net
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
@@ -188,14 +188,18 @@
 
 Passing extras parameters
 
 ```
 rembg i -m sam -x '{"input_labels": [1], "input_points": [[100,100]]}' path/to/input.png path/to/output.png
 ```
 
+```
+rembg i -m u2net_custom -x '{"model_path": "~/.u2net/u2net.onnx"}' path/to/input.png path/to/output.png
+```
+
 ### rembg `p`
 
 Used when input and output are folders.
 
 Remove the background from all images in a folder
 
 ```
@@ -336,15 +340,15 @@
 -   silueta ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/silueta.onnx), [source](https://github.com/xuebinqin/U-2-Net/issues/295)): Same as u2net but the size is reduced to 43Mb.
 -   isnet-general-use ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-general-use.onnx), [source](https://github.com/xuebinqin/DIS)): A new pre-trained model for general use cases.
 -   isnet-anime ([download](https://github.com/danielgatis/rembg/releases/download/v0.0.0/isnet-anime.onnx), [source](https://github.com/SkyTNT/anime-segmentation)): A high-accuracy segmentation for anime character.
 -   sam ([download encoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-encoder-quant.onnx), [download decoder](https://github.com/danielgatis/rembg/releases/download/v0.0.0/vit_b-decoder-quant.onnx), [source](https://github.com/facebookresearch/segment-anything)): A pre-trained model for any use cases.
 
 ### How to train your own model
 
-If You need more fine tunned models try this:
+If You need more fine tuned models try this:
 https://github.com/danielgatis/rembg/issues/193#issuecomment-1055534289
 
 
 ## Some video tutorials
 
 - https://www.youtube.com/watch?v=3xqwpXjxyMQ
 - https://www.youtube.com/watch?v=dFKRGXdkGJU
```

### Comparing `rembg-2.0.47/rembg.egg-info/SOURCES.txt` & `rembg-2.0.48/rembg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,11 @@
 rembg/sessions/base.py
 rembg/sessions/dis_anime.py
 rembg/sessions/dis_general_use.py
 rembg/sessions/sam.py
 rembg/sessions/silueta.py
 rembg/sessions/u2net.py
 rembg/sessions/u2net_cloth_seg.py
+rembg/sessions/u2net_custom.py
 rembg/sessions/u2net_human_seg.py
 rembg/sessions/u2netp.py
 tests/test_remove.py
```

### Comparing `rembg-2.0.47/setup.py` & `rembg-2.0.48/setup.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/tests/test_remove.py` & `rembg-2.0.48/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `rembg-2.0.47/versioneer.py` & `rembg-2.0.48/versioneer.py`

 * *Files identical despite different names*

