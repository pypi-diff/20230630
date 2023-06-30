# Comparing `tmp/dover-lap-1.2.0.tar.gz` & `tmp/dover-lap-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/desh/Work/dover-lap/dist/.tmp-3g3xh83o/dover-lap-1.2.0.tar", last modified: Sun Apr 16 15:40:47 2023, max compression
+gzip compressed data, was "/Users/desh/Work/dover-lap/dist/.tmp-lgvonxky/dover-lap-1.3.0.tar", last modified: Fri Jun 30 09:13:43 2023, max compression
```

## Comparing `dover-lap-1.2.0.tar` & `dover-lap-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.202525 dover-lap-1.2.0/
--rw-r--r--   0 desh       (501) staff       (20)     1065 2020-09-03 00:18:50.000000 dover-lap-1.2.0/LICENSE
--rw-r--r--   0 desh       (501) staff       (20)       24 2020-11-30 03:18:26.000000 dover-lap-1.2.0/MANIFEST.in
--rw-r--r--   0 desh       (501) staff       (20)     4931 2023-04-16 15:40:47.202322 dover-lap-1.2.0/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)     4478 2023-04-16 15:34:23.000000 dover-lap-1.2.0/README.md
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.196703 dover-lap-1.2.0/dover_lap/
--rw-r--r--   0 desh       (501) staff       (20)       39 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/__init__.py
--rwxr-xr-x   0 desh       (501) staff       (20)     4870 2023-04-16 15:31:18.000000 dover-lap-1.2.0/dover_lap/dover_lap.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.199341 dover-lap-1.2.0/dover_lap/libs/
--rw-r--r--   0 desh       (501) staff       (20)       80 2023-03-27 18:35:28.000000 dover-lap-1.2.0/dover_lap/libs/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     4198 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/libs/rttm.py
--rw-r--r--   0 desh       (501) staff       (20)     8884 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/libs/turn.py
--rw-r--r--   0 desh       (501) staff       (20)     3899 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/libs/uem.py
--rw-r--r--   0 desh       (501) staff       (20)     2556 2023-04-15 19:32:10.000000 dover-lap-1.2.0/dover_lap/libs/utils.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.200435 dover-lap-1.2.0/dover_lap/src/
--rw-r--r--   0 desh       (501) staff       (20)      132 2021-03-06 14:56:26.000000 dover-lap-1.2.0/dover_lap/src/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     2128 2023-04-16 15:32:21.000000 dover-lap-1.2.0/dover_lap/src/doverlap.py
--rw-r--r--   0 desh       (501) staff       (20)     1969 2023-04-16 15:32:34.000000 dover-lap-1.2.0/dover_lap/src/label_mapping.py
--rw-r--r--   0 desh       (501) staff       (20)     4385 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/label_voting.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.201534 dover-lap-1.2.0/dover_lap/src/mapping/
--rw-r--r--   0 desh       (501) staff       (20)       66 2023-03-27 18:35:28.000000 dover-lap-1.2.0/dover_lap/src/mapping/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     7800 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/src/mapping/greedy.py
--rw-r--r--   0 desh       (501) staff       (20)     4304 2023-04-16 15:32:07.000000 dover-lap-1.2.0/dover_lap/src/mapping/hungarian.py
--rw-r--r--   0 desh       (501) staff       (20)     1548 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/src/mapping/map_utils.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.201996 dover-lap-1.2.0/dover_lap/src/voting/
--rw-r--r--   0 desh       (501) staff       (20)       42 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/voting/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     2030 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/voting/average.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.197884 dover-lap-1.2.0/dover_lap.egg-info/
--rw-r--r--   0 desh       (501) staff       (20)     4931 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)      733 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/SOURCES.txt
--rw-r--r--   0 desh       (501) staff       (20)        1 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/dependency_links.txt
--rw-r--r--   0 desh       (501) staff       (20)       55 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/entry_points.txt
--rw-r--r--   0 desh       (501) staff       (20)       75 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/requires.txt
--rw-r--r--   0 desh       (501) staff       (20)       10 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/top_level.txt
--rw-r--r--   0 desh       (501) staff       (20)       74 2023-04-15 19:23:06.000000 dover-lap-1.2.0/requirements.txt
--rw-r--r--   0 desh       (501) staff       (20)       38 2023-04-16 15:40:47.202586 dover-lap-1.2.0/setup.cfg
--rw-r--r--   0 desh       (501) staff       (20)      907 2023-04-15 19:23:06.000000 dover-lap-1.2.0/setup.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.965057 dover-lap-1.3.0/
+-rw-r--r--   0 desh       (501) staff       (20)     1065 2020-09-03 00:18:50.000000 dover-lap-1.3.0/LICENSE
+-rw-r--r--   0 desh       (501) staff       (20)       24 2020-11-30 03:18:26.000000 dover-lap-1.3.0/MANIFEST.in
+-rw-r--r--   0 desh       (501) staff       (20)     5746 2023-06-30 09:13:43.964904 dover-lap-1.3.0/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)     5293 2023-04-25 17:04:42.000000 dover-lap-1.3.0/README.md
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.960332 dover-lap-1.3.0/dover_lap/
+-rw-r--r--   0 desh       (501) staff       (20)       39 2021-01-16 15:09:22.000000 dover-lap-1.3.0/dover_lap/__init__.py
+-rwxr-xr-x   0 desh       (501) staff       (20)     5292 2023-04-25 17:04:42.000000 dover-lap-1.3.0/dover_lap/dover_lap.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.962360 dover-lap-1.3.0/dover_lap/libs/
+-rw-r--r--   0 desh       (501) staff       (20)       80 2023-03-27 18:35:28.000000 dover-lap-1.3.0/dover_lap/libs/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     4198 2021-01-16 15:09:22.000000 dover-lap-1.3.0/dover_lap/libs/rttm.py
+-rw-r--r--   0 desh       (501) staff       (20)     9006 2023-04-25 17:04:42.000000 dover-lap-1.3.0/dover_lap/libs/turn.py
+-rw-r--r--   0 desh       (501) staff       (20)     3899 2023-04-15 19:23:06.000000 dover-lap-1.3.0/dover_lap/libs/uem.py
+-rw-r--r--   0 desh       (501) staff       (20)     2556 2023-04-15 19:32:10.000000 dover-lap-1.3.0/dover_lap/libs/utils.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.963259 dover-lap-1.3.0/dover_lap/src/
+-rw-r--r--   0 desh       (501) staff       (20)      132 2021-03-06 14:56:26.000000 dover-lap-1.3.0/dover_lap/src/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     2261 2023-04-25 17:04:42.000000 dover-lap-1.3.0/dover_lap/src/doverlap.py
+-rw-r--r--   0 desh       (501) staff       (20)     1969 2023-04-25 00:59:18.000000 dover-lap-1.3.0/dover_lap/src/label_mapping.py
+-rw-r--r--   0 desh       (501) staff       (20)     5748 2023-04-25 17:04:42.000000 dover-lap-1.3.0/dover_lap/src/label_voting.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.964158 dover-lap-1.3.0/dover_lap/src/mapping/
+-rw-r--r--   0 desh       (501) staff       (20)       66 2023-03-27 18:35:28.000000 dover-lap-1.3.0/dover_lap/src/mapping/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     7800 2023-04-25 15:27:32.000000 dover-lap-1.3.0/dover_lap/src/mapping/greedy.py
+-rw-r--r--   0 desh       (501) staff       (20)     4360 2023-06-30 09:10:13.000000 dover-lap-1.3.0/dover_lap/src/mapping/hungarian.py
+-rw-r--r--   0 desh       (501) staff       (20)     1548 2023-04-15 19:23:06.000000 dover-lap-1.3.0/dover_lap/src/mapping/map_utils.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.964609 dover-lap-1.3.0/dover_lap/src/voting/
+-rw-r--r--   0 desh       (501) staff       (20)       42 2023-04-16 15:19:54.000000 dover-lap-1.3.0/dover_lap/src/voting/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     2391 2023-04-25 17:14:51.000000 dover-lap-1.3.0/dover_lap/src/voting/average.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-06-30 09:13:43.961255 dover-lap-1.3.0/dover_lap.egg-info/
+-rw-r--r--   0 desh       (501) staff       (20)     5746 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)      733 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/SOURCES.txt
+-rw-r--r--   0 desh       (501) staff       (20)        1 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/dependency_links.txt
+-rw-r--r--   0 desh       (501) staff       (20)       55 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/entry_points.txt
+-rw-r--r--   0 desh       (501) staff       (20)       75 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/requires.txt
+-rw-r--r--   0 desh       (501) staff       (20)       10 2023-06-30 09:13:43.000000 dover-lap-1.3.0/dover_lap.egg-info/top_level.txt
+-rw-r--r--   0 desh       (501) staff       (20)       74 2023-04-15 19:23:06.000000 dover-lap-1.3.0/requirements.txt
+-rw-r--r--   0 desh       (501) staff       (20)       38 2023-06-30 09:13:43.965099 dover-lap-1.3.0/setup.cfg
+-rw-r--r--   0 desh       (501) staff       (20)      907 2023-06-30 09:12:03.000000 dover-lap-1.3.0/setup.py
```

### Comparing `dover-lap-1.2.0/LICENSE` & `dover-lap-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/PKG-INFO` & `dover-lap-1.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: dover-lap
-Version: 1.2.0
-Summary: Combine overlap-aware diarization output RTTMs
-Home-page: https://github.com/desh2608/dover-lap
-Author: Desh Raj
-Author-email: r.desh26@gmail.com
-License: Apache-2.0 License
-Keywords: diarization dover
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: BSD License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DOVER-Lap
 Official implementation for [DOVER-Lap: A method for combining overlap-aware diarization outputs](https://arxiv.org/pdf/2011.01997.pdf).
 
 ## Installation
 
 ```shell
 pip install dover-lap
@@ -40,19 +25,33 @@
 
 ```shell
 Usage: dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
 
   Apply the DOVER-Lap algorithm on the input RTTM files.
 
 Options:
+  --gaussian-filter-std FLOAT     Standard deviation for Gaussian filter
+                                  applied before voting. This can help reduce
+                                  the effect of outliers in the input RTTMs.
+                                  For quick turn-taking, set this to a small
+                                  value (e.g. 0.1). 0.5 is a good value for
+                                  most cases. Set this to a very small value,
+                                  e.g. 0.01, to remove filtering.  [default:
+                                  0.5]
+
   --custom-weight TEXT            Weights for input RTTMs
   --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
-  --weight-type [rank|custom]     Specify whether to use rank weighting or
+  --weight-type [rank|custom|norm]
+                                  Specify whether to use rank weighting or
                                   provide custom weights  [default: rank]
 
+  --voting-method [average]       Choose voting method to use: average: use
+                                  weighted average to combine input RTTMs
+                                  [default: average]
+
   --second-maximal                If this flag is set, run a second iteration
                                   of the maximal matching for greedy label
                                   mapping  [default: False]
 
   --label-mapping [hungarian|greedy]
                                   Choose label mapping algorithm to use
                                   [default: greedy]
@@ -90,16 +89,16 @@
 and similarly for the input hypothesis. The DER results are shown below.
 
 |                                   |   MS  |  FA  | Conf. |  DER  |
 |-----------------------------------|:-----:|:----:|:-----:|:-----:|
 | Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
 | Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
 | Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
-| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.76 | 8.17 | 20.73 |
-| DOVER-Lap (Greedy mapping)*        | 9.71 | 3.02 |  **7.68** | **20.40** |
+| DOVER-Lap (Hungarian mapping)     | 9.98 | 2.13 | 8.25 | 20.35 |
+| DOVER-Lap (Greedy mapping)*        | 9.96 | 2.16 |  **7.75** | **19.86** |
 
 _* The Greedy label mapping is exponential in number of inputs (see [this paper](https://arxiv.org/abs/2104.01954))._
 
 ## Running time
 
 The algorithm is implemented in pure Python with NumPy for tensor computations. 
 The time complexity is expected to increase exponentially with the number of
```

### Comparing `dover-lap-1.2.0/README.md` & `dover-lap-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: dover-lap
+Version: 1.3.0
+Summary: Combine overlap-aware diarization output RTTMs
+Home-page: https://github.com/desh2608/dover-lap
+Author: Desh Raj
+Author-email: r.desh26@gmail.com
+License: Apache-2.0 License
+Keywords: diarization dover
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DOVER-Lap
 Official implementation for [DOVER-Lap: A method for combining overlap-aware diarization outputs](https://arxiv.org/pdf/2011.01997.pdf).
 
 ## Installation
 
 ```shell
 pip install dover-lap
@@ -25,19 +40,33 @@
 
 ```shell
 Usage: dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
 
   Apply the DOVER-Lap algorithm on the input RTTM files.
 
 Options:
+  --gaussian-filter-std FLOAT     Standard deviation for Gaussian filter
+                                  applied before voting. This can help reduce
+                                  the effect of outliers in the input RTTMs.
+                                  For quick turn-taking, set this to a small
+                                  value (e.g. 0.1). 0.5 is a good value for
+                                  most cases. Set this to a very small value,
+                                  e.g. 0.01, to remove filtering.  [default:
+                                  0.5]
+
   --custom-weight TEXT            Weights for input RTTMs
   --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
-  --weight-type [rank|custom]     Specify whether to use rank weighting or
+  --weight-type [rank|custom|norm]
+                                  Specify whether to use rank weighting or
                                   provide custom weights  [default: rank]
 
+  --voting-method [average]       Choose voting method to use: average: use
+                                  weighted average to combine input RTTMs
+                                  [default: average]
+
   --second-maximal                If this flag is set, run a second iteration
                                   of the maximal matching for greedy label
                                   mapping  [default: False]
 
   --label-mapping [hungarian|greedy]
                                   Choose label mapping algorithm to use
                                   [default: greedy]
@@ -75,16 +104,16 @@
 and similarly for the input hypothesis. The DER results are shown below.
 
 |                                   |   MS  |  FA  | Conf. |  DER  |
 |-----------------------------------|:-----:|:----:|:-----:|:-----:|
 | Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
 | Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
 | Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
-| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.76 | 8.17 | 20.73 |
-| DOVER-Lap (Greedy mapping)*        | 9.71 | 3.02 |  **7.68** | **20.40** |
+| DOVER-Lap (Hungarian mapping)     | 9.98 | 2.13 | 8.25 | 20.35 |
+| DOVER-Lap (Greedy mapping)*        | 9.96 | 2.16 |  **7.75** | **19.86** |
 
 _* The Greedy label mapping is exponential in number of inputs (see [this paper](https://arxiv.org/abs/2104.01954))._
 
 ## Running time
 
 The algorithm is implemented in pure Python with NumPy for tensor computations. 
 The time complexity is expected to increase exponentially with the number of
```

### Comparing `dover-lap-1.2.0/dover_lap/dover_lap.py` & `dover-lap-1.3.0/dover_lap/dover_lap.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,14 +94,24 @@
     default=0.1,
     help="DOVER weighting factor",
     show_default=True,
 )
 @click.option(
     "--custom-weight", cls=PythonLiteralOption, help="Weights for input RTTMs"
 )
+@click.option(
+    "--gaussian-filter-std",
+    type=float,
+    default=0.5,
+    help="Standard deviation for Gaussian filter applied before voting. This can help"
+    " reduce the effect of outliers in the input RTTMs. For quick turn-taking, set"
+    " this to a small value (e.g. 0.1). 0.5 is a good value for most cases. Set this"
+    " to a very small value, e.g. 0.01, to remove filtering.",
+    show_default=True,
+)
 @click.command(
     cls=command_required_option(
         "weight_type", {"custom": "custom_weight", "rank": "dover_weight", "norm": None}
     )
 )
 def main(
     input_rttms: List[click.Path],
```

### Comparing `dover-lap-1.2.0/dover_lap/libs/rttm.py` & `dover-lap-1.3.0/dover_lap/libs/rttm.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/libs/turn.py` & `dover-lap-1.3.0/dover_lap/libs/turn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """Classes for representing speaker turns and interacting with RTTM files.
 
 Taken from https://github.com/nryant/dscore
 """
+from collections import namedtuple
 from intervaltree import Interval, IntervalTree
 
 from .uem import UEM
 from .utils import groupby, warn, xor
 
 
+Token = namedtuple("Token", ["type", "timestamp", "speaker", "hyp_index", "weight"])
+
+
 class Turn(object):
     """Speaker turn class.
 
     A turn represents a segment of audio attributed to a single speaker.
 
     Parameters
     ----------
```

### Comparing `dover-lap-1.2.0/dover_lap/libs/uem.py` & `dover-lap-1.3.0/dover_lap/libs/uem.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/libs/utils.py` & `dover-lap-1.3.0/dover_lap/libs/utils.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/src/doverlap.py` & `dover-lap-1.3.0/dover_lap/src/doverlap.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         file_id: str,
         label_mapping: Optional[str] = "greedy",
         second_maximal: Optional[bool] = False,
         voting_method: Optional[str] = "average",
         weight_type: Optional[str] = "rank",
         dover_weight: Optional[float] = 0.1,
         custom_weight: Optional[List[str]] = None,
+        gaussian_filter_std: float = 0.01,
     ) -> List[List[Turn]]:
 
         # Label mapping stage
         mapped_turns_list, weights = LabelMapping.get_mapped_turns_list(
             turns_list,
             file_id,
             method=label_mapping,
@@ -37,15 +38,19 @@
             assert isinstance(custom_weight, list)
             weights = np.array([float(x) for x in custom_weight])
         elif weight_type == "norm":
             weights /= np.linalg.norm(weights, ord=1)  # use normalized weights
 
         # Label voting stage
         combined_turns_list = LabelVoting.get_combined_turns(
-            mapped_turns_list, file_id, voting_method, weights
+            mapped_turns_list,
+            file_id,
+            voting_method,
+            weights,
+            gaussian_filter_std=gaussian_filter_std,
         )
         # Merge consecutive turns with the same label
         combined_turns_list = merge_turns(combined_turns_list)
         return combined_turns_list
 
     def __get_ranks(weights: np.array) -> np.array:
```

### Comparing `dover-lap-1.2.0/dover_lap/src/label_mapping.py` & `dover-lap-1.3.0/dover_lap/src/label_mapping.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/src/mapping/greedy.py` & `dover-lap-1.3.0/dover_lap/src/mapping/greedy.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/src/mapping/hungarian.py` & `dover-lap-1.3.0/dover_lap/src/mapping/hungarian.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,22 @@
         DERs = np.zeros((N, N))
         for i in range(N):
             ref = [
                 (turn.speaker_id, turn.onset, turn.offset)
                 for turn in self.turns_list[i]
             ]
             for j in range(N):
+                if i == j:
+                    continue
                 hyp = [
                     (turn.speaker_id, turn.onset, turn.offset)
                     for turn in self.turns_list[j]
                 ]
                 DERs[i, j] = DER(ref, hyp).der
-        mean_ders = DERs.mean(axis=0)
+        mean_ders = DERs.mean(axis=1)
         return -1 * mean_ders
 
     def _map_pair(
         self, ref_turns: List[Turn], sys_turns: List[Turn]
     ) -> Dict[Tuple[int, str], int]:
         ref = [(turn.speaker_id, turn.onset, turn.offset) for turn in ref_turns]
         sys = [(turn.speaker_id, turn.onset, turn.offset) for turn in sys_turns]
```

### Comparing `dover-lap-1.2.0/dover_lap/src/mapping/map_utils.py` & `dover-lap-1.3.0/dover_lap/src/mapping/map_utils.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/dover_lap/src/voting/average.py` & `dover-lap-1.3.0/dover_lap/src/voting/average.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 from typing import Optional, List
 
 import numpy as np
+from scipy.ndimage import gaussian_filter1d
 from scipy.stats import rankdata
 
 from dover_lap.libs.turn import Turn
 
 
 class WeightedAverageVoting:
-    def __init__(self) -> None:
-        pass
+    def __init__(self, gaussian_filter_std: float = 0.01) -> None:
+        self.gaussian_filter_std = gaussian_filter_std
 
     def get_combined_turns(
         self, regions: np.ndarray, start_end: np.ndarray, file_id: str
     ) -> List[Turn]:
         """
         Implements combination using the DOVER-Lap weighted average voting method.
 
-        :param regions, matrix of shape (num_regions, num_speakers), where each row
-            represents a homogeneous time region, and each column represents a speaker.
-            The value in each cell represents the weight of the speaker in that region.
+        :param regions, matrix of shape (num_regions, num_speakers, num_hypothesis).
+            The value in cell (t, k, n) represents the weight speaker `k` in region `t`
+            contributed by hypothesis `n`.
         :param start_end, list of start and end times for each region
         """
         assert (
             regions.shape[0] == start_end.shape[0]
         ), "Regions and start_end must have the same number of rows"
 
+        # Sum the weights from all hypotheses
+        regions = np.sum(regions, axis=2)
+
+        # Apply Gaussian filter to the regions matrix along the T axis
+        regions = gaussian_filter1d(
+            regions, sigma=self.gaussian_filter_std, axis=0, mode="nearest"
+        )
+
         # Get the number of speakers in each region
         num_spks = np.sum(regions, axis=1).round().astype(int)
 
         # Rank the weights in each region. We use the min method to break ties. This
         # means that if two speakers have the same weight, they will be assigned the
         # rank of the lower speaker. Note that we negate the regions matrix because
         # rankdata() sorts in ascending order.
```

### Comparing `dover-lap-1.2.0/dover_lap.egg-info/PKG-INFO` & `dover-lap-1.3.0/dover_lap.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dover-lap
-Version: 1.2.0
+Version: 1.3.0
 Summary: Combine overlap-aware diarization output RTTMs
 Home-page: https://github.com/desh2608/dover-lap
 Author: Desh Raj
 Author-email: r.desh26@gmail.com
 License: Apache-2.0 License
 Keywords: diarization dover
 Classifier: Development Status :: 3 - Alpha
@@ -40,19 +40,33 @@
 
 ```shell
 Usage: dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
 
   Apply the DOVER-Lap algorithm on the input RTTM files.
 
 Options:
+  --gaussian-filter-std FLOAT     Standard deviation for Gaussian filter
+                                  applied before voting. This can help reduce
+                                  the effect of outliers in the input RTTMs.
+                                  For quick turn-taking, set this to a small
+                                  value (e.g. 0.1). 0.5 is a good value for
+                                  most cases. Set this to a very small value,
+                                  e.g. 0.01, to remove filtering.  [default:
+                                  0.5]
+
   --custom-weight TEXT            Weights for input RTTMs
   --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
-  --weight-type [rank|custom]     Specify whether to use rank weighting or
+  --weight-type [rank|custom|norm]
+                                  Specify whether to use rank weighting or
                                   provide custom weights  [default: rank]
 
+  --voting-method [average]       Choose voting method to use: average: use
+                                  weighted average to combine input RTTMs
+                                  [default: average]
+
   --second-maximal                If this flag is set, run a second iteration
                                   of the maximal matching for greedy label
                                   mapping  [default: False]
 
   --label-mapping [hungarian|greedy]
                                   Choose label mapping algorithm to use
                                   [default: greedy]
@@ -90,16 +104,16 @@
 and similarly for the input hypothesis. The DER results are shown below.
 
 |                                   |   MS  |  FA  | Conf. |  DER  |
 |-----------------------------------|:-----:|:----:|:-----:|:-----:|
 | Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
 | Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
 | Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
-| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.76 | 8.17 | 20.73 |
-| DOVER-Lap (Greedy mapping)*        | 9.71 | 3.02 |  **7.68** | **20.40** |
+| DOVER-Lap (Hungarian mapping)     | 9.98 | 2.13 | 8.25 | 20.35 |
+| DOVER-Lap (Greedy mapping)*        | 9.96 | 2.16 |  **7.75** | **19.86** |
 
 _* The Greedy label mapping is exponential in number of inputs (see [this paper](https://arxiv.org/abs/2104.01954))._
 
 ## Running time
 
 The algorithm is implemented in pure Python with NumPy for tensor computations. 
 The time complexity is expected to increase exponentially with the number of
```

### Comparing `dover-lap-1.2.0/dover_lap.egg-info/SOURCES.txt` & `dover-lap-1.3.0/dover_lap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dover-lap-1.2.0/setup.py` & `dover-lap-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description = open("README.md").read()
 
 dev_requires = ["pre-commit", "black", "flake8"]
 
 setup(
     name="dover-lap",
-    version="1.2.0",
+    version="1.3.0",
     author="Desh Raj",
     author_email="r.desh26@gmail.com",
     description="Combine overlap-aware diarization output RTTMs",
     keywords="diarization dover",
     url="https://github.com/desh2608/dover-lap",
     license="Apache-2.0 License",
     packages=find_packages(),
```

