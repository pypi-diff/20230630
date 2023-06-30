# Comparing `tmp/pod5-0.2.2.tar.gz` & `tmp/pod5-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pod5-0.2.2.tar", last modified: Tue Jun  6 15:16:19 2023, max compression
+gzip compressed data, was "pod5-0.2.3.tar", last modified: Wed Jun 28 15:57:45 2023, max compression
```

## Comparing `pod5-0.2.2.tar` & `pod5-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.453690 pod5-0.2.2/
--rw-r--r--   0 root         (0) root         (0)    19537 2023-06-06 15:16:19.453690 pod5-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    18873 2023-06-06 07:26:56.000000 pod5-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1451 2023-06-06 15:16:08.000000 pod5-0.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 15:16:19.453690 pod5-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-06 07:26:56.000000 pod5-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.437689 pod5-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.441689 pod5-0.2.2/src/pod5/
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-06 15:15:09.000000 pod5-0.2.2/src/pod5/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/api_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13092 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/pod5_types.py
--rw-rw-rw-   0 root         (0) root         (0)    36471 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/repack.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/signal_tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.453690 pod5-0.2.2/src/pod5/tools/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/main.py
--rw-rw-rw-   0 root         (0) root         (0)    20644 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)    27154 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_convert_from_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)     9952 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_convert_to_fast5.py
--rw-rw-rw-   0 root         (0) root         (0)     4722 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6822 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_merge.py
--rw-rw-rw-   0 root         (0) root         (0)     3304 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_recover.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_repack.py
--rw-rw-rw-   0 root         (0) root         (0)    18494 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_subset.py
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_update.py
--rw-rw-rw-   0 root         (0) root         (0)    16629 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/pod5_view.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/polars_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5796 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/tools/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2023-06-06 07:26:56.000000 pod5-0.2.2/src/pod5/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 15:16:19.445689 pod5-0.2.2/src/pod5.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19537 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      848 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 15:16:19.000000 pod5-0.2.2/src/pod5.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.433904 pod5-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)    19530 2023-06-28 15:57:45.433904 pod5-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    18873 2023-06-26 10:25:34.000000 pod5-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-28 15:57:36.000000 pod5-0.2.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 15:57:45.433904 pod5-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-26 10:25:34.000000 pod5-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.369899 pod5-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.373899 pod5-0.2.3/src/pod5/
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-28 15:57:24.000000 pod5-0.2.3/src/pod5/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/api_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13092 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/pod5_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    36471 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     7675 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/repack.py
+-rw-rw-rw-   0 root         (0) root         (0)     4827 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/signal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.429904 pod5-0.2.3/src/pod5/tools/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    20644 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)    27286 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_convert_from_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)    10005 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_convert_to_fast5.py
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6822 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_merge.py
+-rw-rw-rw-   0 root         (0) root         (0)     3304 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_recover.py
+-rw-rw-rw-   0 root         (0) root         (0)     2723 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_repack.py
+-rw-rw-rw-   0 root         (0) root         (0)    18541 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_subset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/pod5_update.py
+-rw-rw-rw-   0 root         (0) root         (0)    16686 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/pod5_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/tools/polars_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6105 2023-06-27 15:08:10.000000 pod5-0.2.3/src/pod5/tools/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2023-06-26 10:25:34.000000 pod5-0.2.3/src/pod5/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 15:57:45.377899 pod5-0.2.3/src/pod5.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19530 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-28 15:57:45.000000 pod5-0.2.3/src/pod5.egg-info/top_level.txt
```

### Comparing `pod5-0.2.2/PKG-INFO` & `pod5-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.2
+Version: 0.2.3
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
-Author-email: "Oxford Nanopore Technologies, Limited" <support@nanoporetech.com>
+Author-email: Oxford Nanopore Technologies plc <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pod5-0.2.2/README.md` & `pod5-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/pyproject.toml` & `pod5-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pod5"
-authors = [{name="Oxford Nanopore Technologies, Limited", email="support@nanoporetech.com"}]
+authors = [{name="Oxford Nanopore Technologies plc", email="support@nanoporetech.com"}]
 readme = "README.md"
 requires-python = "~= 3.7"
 dynamic = ["version"]
 description="Oxford Nanopore Technologies Pod5 File Format Python API and Tools"
 
 keywords = ['nanopore']
 
@@ -20,15 +20,15 @@
     'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Bio-Informatics',
 ]
 
 dependencies = [
-    'lib_pod5 == 0.2.2',
+    'lib_pod5 == 0.2.3',
     "iso8601",
     'importlib-metadata; python_version<"3.8"',
     "more_itertools",
     "numpy >= 1.20.0",
     "pyarrow ~= 11.0.0",
     "pytz",
     "packaging",
```

### Comparing `pod5-0.2.2/src/pod5/__init__.py` & `pod5-0.2.3/src/pod5/__init__.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/api_utils.py` & `pod5-0.2.3/src/pod5/api_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/pod5_types.py` & `pod5-0.2.3/src/pod5/pod5_types.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/reader.py` & `pod5-0.2.3/src/pod5/reader.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/repack.py` & `pod5-0.2.3/src/pod5/repack.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/signal_tools.py` & `pod5-0.2.3/src/pod5/signal_tools.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/main.py` & `pod5-0.2.3/src/pod5/tools/main.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/parsers.py` & `pod5-0.2.3/src/pod5/tools/parsers.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_convert_from_fast5.py` & `pod5-0.2.3/src/pod5/tools/pod5_convert_from_fast5.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 from pod5.signal_tools import DEFAULT_SIGNAL_CHUNK_SIZE, vbz_compress_signal_chunked
 from pod5.tools.parsers import pod5_convert_from_fast5_argparser, run_tool
 from pod5.tools.utils import (
     DEFAULT_THREADS,
     PBAR_DEFAULTS,
     collect_inputs,
     init_logging,
+    limit_threads,
     logged,
     logged_all,
     terminate_processes,
 )
 
 READ_CHUNK_SIZE = 400
 TIMEOUT_SECONDS = 600
@@ -421,15 +422,17 @@
     # Resolve the offset in enumeration values between both files
     p5_scaled_end_reason = fast5_end_reason - 1
     return p5.EndReason.from_reason_with_default_forced(
         p5.EndReasonEnum(p5_scaled_end_reason)
     )
 
 
-def convert_datetime_as_epoch_ms(time_str: Optional[str]) -> datetime.datetime:
+def convert_datetime_as_epoch_ms(
+    time_str: Union[str, bytes, None]
+) -> datetime.datetime:
     """Convert the fast5 time string to timestamp"""
     epoch = datetime.datetime.utcfromtimestamp(0).replace(tzinfo=datetime.timezone.utc)
     if time_str is None:
         return epoch
     try:
         return iso8601.parse_date(decode_str(time_str))
     except iso8601.iso8601.ParseError:
@@ -437,40 +440,40 @@
 
 
 def convert_run_info(
     acq_id: str,
     adc_max: int,
     adc_min: int,
     sample_rate: int,
-    context_tags: Dict[str, str],
+    context_tags: Dict[str, Union[str, bytes]],
     device_type: str,
-    tracking_id: Dict[str, str],
+    tracking_id: Dict[str, Union[str, bytes]],
 ) -> p5.RunInfo:
     """Create a Pod5RunInfo instance from parsed fast5 data"""
     return p5.RunInfo(
         acquisition_id=acq_id,
         acquisition_start_time=convert_datetime_as_epoch_ms(
-            tracking_id["exp_start_time"]
+            tracking_id.get("exp_start_time")
         ),
         adc_max=adc_max,
         adc_min=adc_min,
         context_tags={
             str(key): decode_str(value) for key, value in context_tags.items()
         },
         experiment_name="",
         flow_cell_id=decode_str(tracking_id.get("flow_cell_id", b"")),
         flow_cell_product_code=decode_str(
             tracking_id.get("flow_cell_product_code", b"")
         ),
-        protocol_name=decode_str(tracking_id["exp_script_name"]),
-        protocol_run_id=decode_str(tracking_id["protocol_run_id"]),
+        protocol_name=decode_str(tracking_id.get("exp_script_name", b"")),
+        protocol_run_id=decode_str(tracking_id.get("protocol_run_id", b"")),
         protocol_start_time=convert_datetime_as_epoch_ms(
             tracking_id.get("protocol_start_time", None)
         ),
-        sample_id=decode_str(tracking_id["sample_id"]),
+        sample_id=decode_str(tracking_id.get("sample_id", b"")),
         sample_rate=sample_rate,
         sequencing_kit=decode_str(context_tags.get("sequencing_kit", b"")),
         sequencer_position=decode_str(tracking_id.get("device_id", b"")),
         sequencer_position_type=decode_str(tracking_id.get("device_type", device_type)),
         software="python-pod5-converter",
         system_name=decode_str(tracking_id.get("host_product_serial_number", b"")),
         system_type=decode_str(tracking_id.get("host_product_code", b"")),
@@ -770,14 +773,16 @@
         raise FileExistsError(
             "Output path points to an existing file and --force-overwrite not set"
         )
 
     if len(output.parts) > 1:
         output.parent.mkdir(parents=True, exist_ok=True)
 
+    threads = limit_threads(threads)
+
     pending_fast5s = collect_inputs(inputs, recursive, "*.fast5", threads=threads)
     if not pending_fast5s:
         logger.fatal(f"Found no *.fast5 files in inputs: {inputs}")
         raise RuntimeError("Found no fast5 inputs to process - Exiting")
 
     output_handler = OutputHandler(output, one_to_one, force_overwrite)
     status = StatusMonitor(pending_fast5s)
```

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_convert_to_fast5.py` & `pod5-0.2.3/src/pod5/tools/pod5_convert_to_fast5.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import h5py
 import numpy
 import vbz_h5py_plugin  # noqa: F401
 from more_itertools import chunked
 
 import pod5 as p5
 from pod5.tools.parsers import pod5_convert_to_fast5_argparser, run_tool
-from pod5.tools.utils import DEFAULT_THREADS, collect_inputs
+from pod5.tools.utils import DEFAULT_THREADS, collect_inputs, limit_threads
 
 # Pod5 does not have 'partial' so need to add that back in here.
 FAST5_END_REASONS = {
     "unknown": 0,
     "partial": 1,  # Do not remove, required by fast5.
     "mux_change": 2,
     "unblock_mux_change": 3,
@@ -251,14 +251,16 @@
     threads: int = DEFAULT_THREADS,
     force_overwrite: bool = False,
     file_read_count: int = 4000,
 ):
     if output.exists() and not output.is_dir():
         raise FileExistsError("Cannot output to a file")
 
+    threads = limit_threads(threads)
+
     with ProcessPoolExecutor(max_workers=threads) as executor:
         total_reads = 0
         futures: Dict[Future, Path] = {}
 
         # Enumerate over input pod5 files
         for input_idx, source in enumerate(
             collect_inputs(inputs, recursive, "*.pod5", threads=threads)
```

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_filter.py` & `pod5-0.2.3/src/pod5/tools/pod5_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List
 from pod5.tools.polars_utils import PL_DEST_FNAME, PL_READ_ID, PL_UUID_REGEX
 from pod5.tools.utils import (
     DEFAULT_THREADS,
     PBAR_DEFAULTS,
     collect_inputs,
     init_logging,
+    limit_threads,
     logged_all,
 )
 
 import polars as pl
 
 from tqdm.auto import tqdm
 
@@ -131,14 +132,16 @@
     # Create parent directories if they do not exist
     if not output.parent.exists():
         output.parent.mkdir(parents=True, exist_ok=True)
 
     targets = parse_read_id_targets(ids, output=output)
     print(f"Parsed {len(targets.collect())} reads_ids from: {ids.name}")
 
+    threads = limit_threads(threads)
+
     _inputs = collect_inputs(inputs, recursive, "*.pod5", threads=threads)
     sources = parse_sources(_inputs, duplicate_ok=duplicate_ok, threads=threads)
     print(f"Found {len(sources.collect())} read_ids from {len(_inputs)} inputs")
 
     # Map the target outputs to which source read ids they're comprised of
     transfers = calculate_transfers(
         sources=sources,
```

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_inspect.py` & `pod5-0.2.3/src/pod5/tools/pod5_inspect.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_merge.py` & `pod5-0.2.3/src/pod5/tools/pod5_merge.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_recover.py` & `pod5-0.2.3/src/pod5/tools/pod5_recover.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_repack.py` & `pod5-0.2.3/src/pod5/tools/pod5_repack.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pod5 as p5
 import pod5.repack
 from pod5.tools.utils import (
     DEFAULT_THREADS,
     PBAR_DEFAULTS,
     assert_no_duplicate_filenames,
     collect_inputs,
+    limit_threads,
 )
 from pod5.tools.parsers import prepare_pod5_repack_argparser, run_tool
 
 
 def resolve_overwrite(src: Path, dest: Path, force: bool) -> None:
     if dest.exists():
         if dest == src:
@@ -53,14 +54,16 @@
     if output.exists() and not output.is_dir():
         raise ValueError(f"Output cannot be an existing file: {output}")
 
     # Create output directory if required
     if not output.is_dir():
         output.mkdir(parents=True, exist_ok=True)
 
+    threads = limit_threads(threads)
+
     _inputs = collect_inputs(
         inputs, recursive=recursive, pattern="*.pod5", threads=threads
     )
     assert_no_duplicate_filenames(_inputs)
 
     # Remove existing files if required
     for input_filename in _inputs:
```

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_subset.py` & `pod5-0.2.3/src/pod5/tools/pod5_subset.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     pl_format_read_id,
 )
 from pod5.tools.utils import (
     DEFAULT_THREADS,
     PBAR_DEFAULTS,
     collect_inputs,
     init_logging,
+    limit_threads,
     logged,
     logged_all,
     terminate_processes,
 )
 from pod5.tools.parsers import prepare_pod5_subset_argparser, run_tool
 
 
@@ -281,16 +282,16 @@
 
 
 @logged_all
 def parse_sources(
     paths: Set[Path], duplicate_ok: bool, threads: int = DEFAULT_THREADS
 ) -> pl.LazyFrame:
     """Reads all inputs and return formatted lazy dataframe"""
-    assert threads > 0
 
+    threads = limit_threads(threads)
     n_proc = min(threads, len(paths))
 
     ctx = mp.get_context("spawn")
     work: mp.JoinableQueue = ctx.JoinableQueue(maxsize=len(paths) + n_proc)
     parsed_sources = ctx.Queue(maxsize=len(paths))
     for path in paths:
         work.put(path)
@@ -449,15 +450,15 @@
 
 
 @logged_all
 def launch_subsetting(transfers: pl.LazyFrame, threads: int = DEFAULT_THREADS) -> None:
     """
     Iterate over the transfers dataframe subsetting reads from sources to destinations
     """
-    assert threads > 0
+    threads = limit_threads(threads)
     assert {PL_READ_ID, PL_SRC_FNAME, PL_DEST_FNAME}.issubset(set(transfers.columns))
 
     ctx = mp.get_context("spawn")
     work = WorkQueue(ctx, transfers)
 
     active_processes = []
     try:
```

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_update.py` & `pod5-0.2.3/src/pod5/tools/pod5_update.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/pod5_view.py` & `pod5-0.2.3/src/pod5/tools/pod5_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pod5 as p5
 from pod5.tools.parsers import prepare_pod5_view_argparser, run_tool
 from pod5.tools.polars_utils import pl_format_empty_string, pl_format_read_id
 from pod5.tools.utils import (
     DEFAULT_THREADS,
     collect_inputs,
     init_logging,
+    limit_threads,
     logged,
     logged_all,
     terminate_processes,
 )
 
 
 logger = init_logging()
@@ -506,14 +507,16 @@
 ) -> None:
     """Given a list of POD5 files write a table to view their contents"""
 
     if list_fields:
         print_fields()
         return
 
+    threads = limit_threads(threads)
+
     output_path = resolve_output(output, force_overwrite)
 
     # Decode escaped separator characters e.g. \t
     sep = codecs.decode(separator, "unicode-escape")
 
     # Parse column selection args
     selection = select_fields(**kwargs)
```

### Comparing `pod5-0.2.2/src/pod5/tools/polars_utils.py` & `pod5-0.2.3/src/pod5/tools/polars_utils.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5/tools/utils.py` & `pod5-0.2.3/src/pod5/tools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,25 @@
 import os
 from time import perf_counter
 from typing import Collection, Iterable, List, Set, Union
 from pathlib import Path
 import uuid
 
 
-DEFAULT_THREADS = min(mp.cpu_count(), 8)
+# os.cpu_count() can return None if it fails
+DEFAULT_THREADS = min(os.cpu_count() or 4, 4)
+
+
+def limit_threads(requested: int) -> int:
+    """
+    Santise and limit the number of `requested` threads to the number of logical cores
+    """
+    if requested < 1:
+        return os.cpu_count() or 4
+    return min(os.cpu_count() or requested, requested)
 
 
 def collect_inputs(
     paths: Iterable[Path],
     recursive: bool,
     pattern: Union[str, Collection[str]],
     threads: int = DEFAULT_THREADS,
```

### Comparing `pod5-0.2.2/src/pod5/writer.py` & `pod5-0.2.3/src/pod5/writer.py`

 * *Files identical despite different names*

### Comparing `pod5-0.2.2/src/pod5.egg-info/PKG-INFO` & `pod5-0.2.3/src/pod5.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pod5
-Version: 0.2.2
+Version: 0.2.3
 Summary: Oxford Nanopore Technologies Pod5 File Format Python API and Tools
-Author-email: "Oxford Nanopore Technologies, Limited" <support@nanoporetech.com>
+Author-email: Oxford Nanopore Technologies plc <support@nanoporetech.com>
 Keywords: nanopore
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pod5-0.2.2/src/pod5.egg-info/SOURCES.txt` & `pod5-0.2.3/src/pod5.egg-info/SOURCES.txt`

 * *Files identical despite different names*

