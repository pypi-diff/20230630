# Comparing `tmp/lib_pod5-0.2.2-cp39-cp39-win_amd64.whl.zip` & `tmp/lib_pod5-0.2.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 2093119 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     1104 b- defN 23-May-18 16:02 lib_pod5/__init__.py
--rw-rw-rw-  2.0 fat      139 b- defN 23-Jun-06 15:46 lib_pod5/_version.py
--rw-rw-rw-  2.0 fat  6945792 b- defN 23-Jun-06 15:49 lib_pod5/pod5_format_pybind.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     7396 b- defN 23-May-18 16:02 lib_pod5/pod5_format_pybind.pyi
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 15:40 lib_pod5/py.typed
--rw-rw-rw-  2.0 fat     1167 b- defN 23-Jun-06 15:50 lib_pod5-0.2.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-06 15:50 lib_pod5-0.2.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-06 15:50 lib_pod5-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      720 b- defN 23-Jun-06 15:50 lib_pod5-0.2.2.dist-info/RECORD
-9 files, 6956427 bytes uncompressed, 2091881 bytes compressed:  69.9%
+Zip file size: 2852655 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 16:05 lib_pod5/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 16:05 lib_pod5.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-28 16:05 lib_pod5-0.2.3.dist-info/
+-rw-rw-rw-  2.0 unx     7192 b- defN 23-Jun-28 16:05 lib_pod5/pod5_format_pybind.pyi
+-rw-r--r--  2.0 unx      136 b- defN 23-Jun-28 16:05 lib_pod5/_version.py
+-rw-r--r--  2.0 unx     1058 b- defN 23-Jun-28 16:05 lib_pod5/__init__.py
+-rwxr-xr-x  2.0 unx  8579008 b- defN 23-Jun-28 16:05 lib_pod5/pod5_format_pybind.cpython-37m-x86_64-linux-gnu.so
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jun-28 16:05 lib_pod5/py.typed
+-rw-r--r--  2.0 unx      150 b- defN 23-Jun-28 16:05 lib_pod5-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1129 b- defN 23-Jun-28 16:05 lib_pod5-0.2.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx      742 b- defN 23-Jun-28 16:05 lib_pod5-0.2.3.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-28 16:05 lib_pod5-0.2.3.dist-info/top_level.txt
+12 files, 8589424 bytes uncompressed, 2851067 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
-Filename: lib_pod5/__init__.py
+Filename: lib_pod5/
 Comment: 
 
-Filename: lib_pod5/_version.py
+Filename: lib_pod5.libs/
 Comment: 
 
-Filename: lib_pod5/pod5_format_pybind.cp39-win_amd64.pyd
+Filename: lib_pod5-0.2.3.dist-info/
 Comment: 
 
 Filename: lib_pod5/pod5_format_pybind.pyi
 Comment: 
 
+Filename: lib_pod5/_version.py
+Comment: 
+
+Filename: lib_pod5/__init__.py
+Comment: 
+
+Filename: lib_pod5/pod5_format_pybind.cpython-37m-x86_64-linux-gnu.so
+Comment: 
+
 Filename: lib_pod5/py.typed
 Comment: 
 
-Filename: lib_pod5-0.2.2.dist-info/METADATA
+Filename: lib_pod5-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: lib_pod5-0.2.2.dist-info/WHEEL
+Filename: lib_pod5-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: lib_pod5-0.2.2.dist-info/top_level.txt
+Filename: lib_pod5-0.2.3.dist-info/RECORD
 Comment: 
 
-Filename: lib_pod5-0.2.2.dist-info/RECORD
+Filename: lib_pod5-0.2.3.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## lib_pod5/__init__.py

 * *Ordering differences only*

```diff
@@ -1,46 +1,46 @@
-""" Imports everything from the pod5_format_pybind11 module and associated .pyi"""
-
-from ._version import __version__, __version_tuple__
-from .pod5_format_pybind import (
-    EmbeddedFileData,
-    FileWriter,
-    FileWriterOptions,
-    Pod5AsyncSignalLoader,
-    Pod5FileReader,
-    Pod5RepackerOutput,
-    Pod5SignalCacheBatch,
-    Repacker,
-    compress_signal,
-    create_file,
-    recover_file,
-    decompress_signal,
-    format_read_id_to_str,
-    get_error_string,
-    load_read_id_iterable,
-    open_file,
-    update_file,
-    vbz_compressed_signal_max_size,
-)
-
-__all__ = [
-    "__version__",
-    "__version_tuple__",
-    "EmbeddedFileData",
-    "FileWriter",
-    "FileWriterOptions",
-    "Pod5AsyncSignalLoader",
-    "Pod5FileReader",
-    "Pod5RepackerOutput",
-    "Pod5SignalCacheBatch",
-    "Repacker",
-    "compress_signal",
-    "create_file",
-    "recover_file",
-    "decompress_signal",
-    "format_read_id_to_str",
-    "get_error_string",
-    "load_read_id_iterable",
-    "open_file",
-    "update_file",
-    "vbz_compressed_signal_max_size",
-]
+""" Imports everything from the pod5_format_pybind11 module and associated .pyi"""
+
+from ._version import __version__, __version_tuple__
+from .pod5_format_pybind import (
+    EmbeddedFileData,
+    FileWriter,
+    FileWriterOptions,
+    Pod5AsyncSignalLoader,
+    Pod5FileReader,
+    Pod5RepackerOutput,
+    Pod5SignalCacheBatch,
+    Repacker,
+    compress_signal,
+    create_file,
+    recover_file,
+    decompress_signal,
+    format_read_id_to_str,
+    get_error_string,
+    load_read_id_iterable,
+    open_file,
+    update_file,
+    vbz_compressed_signal_max_size,
+)
+
+__all__ = [
+    "__version__",
+    "__version_tuple__",
+    "EmbeddedFileData",
+    "FileWriter",
+    "FileWriterOptions",
+    "Pod5AsyncSignalLoader",
+    "Pod5FileReader",
+    "Pod5RepackerOutput",
+    "Pod5SignalCacheBatch",
+    "Repacker",
+    "compress_signal",
+    "create_file",
+    "recover_file",
+    "decompress_signal",
+    "format_read_id_to_str",
+    "get_error_string",
+    "load_read_id_iterable",
+    "open_file",
+    "update_file",
+    "vbz_compressed_signal_max_size",
+]
```

## lib_pod5/_version.py

```diff
@@ -1,3 +1,3 @@
-# This file is auto generated by cmake during compilation
-__version__ = version = "0.2.2"
-__version_tuple__ = version_tuple = (0, 2, 2)
+# This file is auto generated by cmake during compilation
+__version__ = version = "0.2.3"
+__version_tuple__ = version_tuple = (0, 2, 3)
```

## lib_pod5/pod5_format_pybind.pyi

 * *Ordering differences only*

```diff
@@ -1,204 +1,204 @@
-"""
-c++ bindings for pod5_format
-"""
-
-# pylint: skip-file
-
-# created with mypy.stubgen for code completion
-# > pip install mypy
-# > stubgen -m lib_pod5.pod5_format_pybind
-
-from typing import Any, Iterable, List, Optional, Tuple, Union
-
-import numpy as np
-import numpy.typing as npt
-
-class EmbeddedFileData:
-    def __init__(self, *args, **kwargs) -> None: ...
-    @property
-    def length(self) -> int: ...
-    @property
-    def offset(self) -> int: ...
-    @property
-    def file_path(self) -> str: ...
-
-class FileWriter:
-    def __init__(self, *args, **kwargs) -> None: ...
-    def add_end_reason(self, end_reason_enum: int) -> int: ...
-    def add_pore(self, pore_type: str) -> int: ...
-    def add_reads(
-        self,
-        count: int,
-        read_ids: npt.NDArray[np.uint8],
-        read_numbers: npt.NDArray[np.uint32],
-        start_samples: npt.NDArray[np.uint64],
-        channels: npt.NDArray[np.uint16],
-        wells: npt.NDArray[np.uint8],
-        pore_types: npt.NDArray[np.int16],
-        calibration_offsets: npt.NDArray[np.float32],
-        calibration_scales: npt.NDArray[np.float32],
-        median_befores: npt.NDArray[np.float32],
-        end_reasons: npt.NDArray[np.int16],
-        end_reason_forceds: npt.NDArray[np.bool_],
-        run_infos: npt.NDArray[np.int16],
-        num_minknow_events: npt.NDArray[np.uint64],
-        tracked_scaling_scales: npt.NDArray[np.float32],
-        tracked_scaling_shifts: npt.NDArray[np.float32],
-        predicted_scaling_scales: npt.NDArray[np.float32],
-        predicted_scaling_shifts: npt.NDArray[np.float32],
-        num_reads_since_mux_changes: npt.NDArray[np.uint32],
-        time_since_mux_changes: npt.NDArray[np.float32],
-        signals: List[npt.NDArray[np.int16]],
-    ) -> None: ...
-    def add_reads_pre_compressed(
-        self,
-        count: int,
-        read_ids: npt.NDArray[np.uint8],
-        read_numbers: npt.NDArray[np.uint32],
-        start_samples: npt.NDArray[np.uint64],
-        channels: npt.NDArray[np.uint16],
-        wells: npt.NDArray[np.uint8],
-        pore_types: npt.NDArray[np.int16],
-        calibration_offsets: npt.NDArray[np.float32],
-        calibration_scales: npt.NDArray[np.float32],
-        median_befores: npt.NDArray[np.float32],
-        end_reasons: npt.NDArray[np.int16],
-        end_reason_forceds: npt.NDArray[np.bool_],
-        run_infos: npt.NDArray[np.int16],
-        num_minknow_events: npt.NDArray[np.uint64],
-        tracked_scaling_scales: npt.NDArray[np.float32],
-        tracked_scaling_shifts: npt.NDArray[np.float32],
-        predicted_scaling_scales: npt.NDArray[np.float32],
-        predicted_scaling_shifts: npt.NDArray[np.float32],
-        num_reads_since_mux_changes: npt.NDArray[np.uint32],
-        time_since_mux_changes: npt.NDArray[np.float32],
-        signal_chunks: List[npt.NDArray[np.uint8]],
-        signal_chunk_lengths: npt.NDArray[np.uint32],
-        signal_chunk_counts: npt.NDArray[np.uint32],
-    ) -> None: ...
-    def add_run_info(
-        self,
-        acquisition_id: str,
-        acquisition_start_time: int,
-        adc_max: int,
-        adc_min: int,
-        context_tags: List[Tuple[str, str]],
-        experiment_name: str,
-        flow_cell_id: str,
-        flow_cell_product_code: str,
-        protocol_name: str,
-        protocol_run_id: str,
-        protocol_start_time: int,
-        sample_id: str,
-        sample_rate: int,
-        sequencing_kit: str,
-        sequencer_position: str,
-        sequencer_position_type: str,
-        software: str,
-        system_name: str,
-        system_type: str,
-        tracking_id: List[Tuple[str, str]],
-    ) -> int: ...
-    def close(self) -> None: ...
-
-class FileWriterOptions:
-    max_signal_chunk_size: int
-    read_table_batch_size: int
-    signal_compression_type: Any
-    signal_table_batch_size: int
-    def __init__(self, *args, **kwargs) -> None: ...
-
-class Pod5AsyncSignalLoader:
-    def __init__(self, *args, **kwargs) -> None: ...
-    def release_next_batch(self) -> Pod5SignalCacheBatch: ...
-
-class Pod5FileReader:
-    def __init__(self, *args, **kwargs) -> None: ...
-    def batch_get_signal(
-        self, get_samples: bool, get_sample_count: bool
-    ) -> Pod5AsyncSignalLoader: ...
-    def batch_get_signal_batches(
-        self,
-        get_samples: bool,
-        get_samples_count: bool,
-        batches: npt.NDArray[np.uint32],
-    ) -> Pod5AsyncSignalLoader: ...
-    def batch_get_signal_selection(
-        self,
-        get_samples: bool,
-        get_sample_count: bool,
-        batch_counts: npt.NDArray[np.uint32],
-        batch_rows: npt.NDArray[np.uint32],
-    ) -> Pod5AsyncSignalLoader: ...
-    def close(self) -> None: ...
-    def get_file_read_table_location(self) -> EmbeddedFileData: ...
-    def get_file_run_info_table_location(self) -> EmbeddedFileData: ...
-    def get_file_signal_table_location(self) -> EmbeddedFileData: ...
-    def get_file_version_pre_migration(self) -> str: ...
-    def plan_traversal(
-        self,
-        read_id_data: npt.NDArray[np.uint8],
-        batch_counts: npt.NDArray[np.uint32],
-        batch_rows: npt.NDArray[np.uint32],
-    ) -> int: ...
-
-class Pod5RepackerOutput:
-    def __init__(self, *args, **kwargs) -> None: ...
-
-class Pod5SignalCacheBatch:
-    def __init__(self, *args, **kwargs) -> None: ...
-    @property
-    def batch_index(self) -> int: ...
-    @property
-    def sample_count(self) -> npt.NDArray[np.uint64]: ...
-    @property
-    def samples(self) -> List[npt.NDArray[np.int16]]: ...
-
-class Repacker:
-    def __init__(self) -> None: ...
-    def add_all_reads_to_output(
-        self, output: Pod5RepackerOutput, input: Pod5FileReader
-    ) -> None: ...
-    def add_output(self, output: FileWriter) -> Pod5RepackerOutput: ...
-    def add_selected_reads_to_output(
-        self,
-        output: Pod5RepackerOutput,
-        input: Pod5FileReader,
-        batch_counts: npt.NDArray[np.uint32],
-        all_batch_rows: npt.NDArray[np.uint32],
-    ) -> None: ...
-    def finish(self) -> None: ...
-    @property
-    def batches_completed(self) -> int: ...
-    @property
-    def batches_requested(self) -> int: ...
-    @property
-    def is_complete(self) -> bool: ...
-    @property
-    def pending_batch_writes(self) -> int: ...
-    @property
-    def reads_completed(self) -> int: ...
-    @property
-    def reads_sample_bytes_completed(self) -> int: ...
-
-def compress_signal(
-    signal: npt.NDArray[np.int16], compressed_signal_out: npt.NDArray[np.uint8]
-) -> int: ...
-def create_file(
-    src_filename: str, writer_name: str, options: Optional[FileWriterOptions]
-) -> FileWriter: ...
-def recover_file(src_filename: str, dst_filename: str) -> FileWriter: ...
-def decompress_signal(
-    compressed_signal: Union[npt.NDArray[np.uint8], memoryview],
-    signal_out: npt.NDArray[np.int16],
-) -> None: ...
-def format_read_id_to_str(
-    read_id_data_out: npt.NDArray[np.uint8],
-) -> List[str]: ...
-def get_error_string() -> str: ...
-def load_read_id_iterable(
-    read_ids_str: Iterable, read_id_data_out: npt.NDArray[np.uint8]
-) -> int: ...
-def open_file(filename: str) -> Pod5FileReader: ...
-def update_file(reader: Pod5FileReader, output: str): ...
-def vbz_compressed_signal_max_size(sample_count: int) -> int: ...
+"""
+c++ bindings for pod5_format
+"""
+
+# pylint: skip-file
+
+# created with mypy.stubgen for code completion
+# > pip install mypy
+# > stubgen -m lib_pod5.pod5_format_pybind
+
+from typing import Any, Iterable, List, Optional, Tuple, Union
+
+import numpy as np
+import numpy.typing as npt
+
+class EmbeddedFileData:
+    def __init__(self, *args, **kwargs) -> None: ...
+    @property
+    def length(self) -> int: ...
+    @property
+    def offset(self) -> int: ...
+    @property
+    def file_path(self) -> str: ...
+
+class FileWriter:
+    def __init__(self, *args, **kwargs) -> None: ...
+    def add_end_reason(self, end_reason_enum: int) -> int: ...
+    def add_pore(self, pore_type: str) -> int: ...
+    def add_reads(
+        self,
+        count: int,
+        read_ids: npt.NDArray[np.uint8],
+        read_numbers: npt.NDArray[np.uint32],
+        start_samples: npt.NDArray[np.uint64],
+        channels: npt.NDArray[np.uint16],
+        wells: npt.NDArray[np.uint8],
+        pore_types: npt.NDArray[np.int16],
+        calibration_offsets: npt.NDArray[np.float32],
+        calibration_scales: npt.NDArray[np.float32],
+        median_befores: npt.NDArray[np.float32],
+        end_reasons: npt.NDArray[np.int16],
+        end_reason_forceds: npt.NDArray[np.bool_],
+        run_infos: npt.NDArray[np.int16],
+        num_minknow_events: npt.NDArray[np.uint64],
+        tracked_scaling_scales: npt.NDArray[np.float32],
+        tracked_scaling_shifts: npt.NDArray[np.float32],
+        predicted_scaling_scales: npt.NDArray[np.float32],
+        predicted_scaling_shifts: npt.NDArray[np.float32],
+        num_reads_since_mux_changes: npt.NDArray[np.uint32],
+        time_since_mux_changes: npt.NDArray[np.float32],
+        signals: List[npt.NDArray[np.int16]],
+    ) -> None: ...
+    def add_reads_pre_compressed(
+        self,
+        count: int,
+        read_ids: npt.NDArray[np.uint8],
+        read_numbers: npt.NDArray[np.uint32],
+        start_samples: npt.NDArray[np.uint64],
+        channels: npt.NDArray[np.uint16],
+        wells: npt.NDArray[np.uint8],
+        pore_types: npt.NDArray[np.int16],
+        calibration_offsets: npt.NDArray[np.float32],
+        calibration_scales: npt.NDArray[np.float32],
+        median_befores: npt.NDArray[np.float32],
+        end_reasons: npt.NDArray[np.int16],
+        end_reason_forceds: npt.NDArray[np.bool_],
+        run_infos: npt.NDArray[np.int16],
+        num_minknow_events: npt.NDArray[np.uint64],
+        tracked_scaling_scales: npt.NDArray[np.float32],
+        tracked_scaling_shifts: npt.NDArray[np.float32],
+        predicted_scaling_scales: npt.NDArray[np.float32],
+        predicted_scaling_shifts: npt.NDArray[np.float32],
+        num_reads_since_mux_changes: npt.NDArray[np.uint32],
+        time_since_mux_changes: npt.NDArray[np.float32],
+        signal_chunks: List[npt.NDArray[np.uint8]],
+        signal_chunk_lengths: npt.NDArray[np.uint32],
+        signal_chunk_counts: npt.NDArray[np.uint32],
+    ) -> None: ...
+    def add_run_info(
+        self,
+        acquisition_id: str,
+        acquisition_start_time: int,
+        adc_max: int,
+        adc_min: int,
+        context_tags: List[Tuple[str, str]],
+        experiment_name: str,
+        flow_cell_id: str,
+        flow_cell_product_code: str,
+        protocol_name: str,
+        protocol_run_id: str,
+        protocol_start_time: int,
+        sample_id: str,
+        sample_rate: int,
+        sequencing_kit: str,
+        sequencer_position: str,
+        sequencer_position_type: str,
+        software: str,
+        system_name: str,
+        system_type: str,
+        tracking_id: List[Tuple[str, str]],
+    ) -> int: ...
+    def close(self) -> None: ...
+
+class FileWriterOptions:
+    max_signal_chunk_size: int
+    read_table_batch_size: int
+    signal_compression_type: Any
+    signal_table_batch_size: int
+    def __init__(self, *args, **kwargs) -> None: ...
+
+class Pod5AsyncSignalLoader:
+    def __init__(self, *args, **kwargs) -> None: ...
+    def release_next_batch(self) -> Pod5SignalCacheBatch: ...
+
+class Pod5FileReader:
+    def __init__(self, *args, **kwargs) -> None: ...
+    def batch_get_signal(
+        self, get_samples: bool, get_sample_count: bool
+    ) -> Pod5AsyncSignalLoader: ...
+    def batch_get_signal_batches(
+        self,
+        get_samples: bool,
+        get_samples_count: bool,
+        batches: npt.NDArray[np.uint32],
+    ) -> Pod5AsyncSignalLoader: ...
+    def batch_get_signal_selection(
+        self,
+        get_samples: bool,
+        get_sample_count: bool,
+        batch_counts: npt.NDArray[np.uint32],
+        batch_rows: npt.NDArray[np.uint32],
+    ) -> Pod5AsyncSignalLoader: ...
+    def close(self) -> None: ...
+    def get_file_read_table_location(self) -> EmbeddedFileData: ...
+    def get_file_run_info_table_location(self) -> EmbeddedFileData: ...
+    def get_file_signal_table_location(self) -> EmbeddedFileData: ...
+    def get_file_version_pre_migration(self) -> str: ...
+    def plan_traversal(
+        self,
+        read_id_data: npt.NDArray[np.uint8],
+        batch_counts: npt.NDArray[np.uint32],
+        batch_rows: npt.NDArray[np.uint32],
+    ) -> int: ...
+
+class Pod5RepackerOutput:
+    def __init__(self, *args, **kwargs) -> None: ...
+
+class Pod5SignalCacheBatch:
+    def __init__(self, *args, **kwargs) -> None: ...
+    @property
+    def batch_index(self) -> int: ...
+    @property
+    def sample_count(self) -> npt.NDArray[np.uint64]: ...
+    @property
+    def samples(self) -> List[npt.NDArray[np.int16]]: ...
+
+class Repacker:
+    def __init__(self) -> None: ...
+    def add_all_reads_to_output(
+        self, output: Pod5RepackerOutput, input: Pod5FileReader
+    ) -> None: ...
+    def add_output(self, output: FileWriter) -> Pod5RepackerOutput: ...
+    def add_selected_reads_to_output(
+        self,
+        output: Pod5RepackerOutput,
+        input: Pod5FileReader,
+        batch_counts: npt.NDArray[np.uint32],
+        all_batch_rows: npt.NDArray[np.uint32],
+    ) -> None: ...
+    def finish(self) -> None: ...
+    @property
+    def batches_completed(self) -> int: ...
+    @property
+    def batches_requested(self) -> int: ...
+    @property
+    def is_complete(self) -> bool: ...
+    @property
+    def pending_batch_writes(self) -> int: ...
+    @property
+    def reads_completed(self) -> int: ...
+    @property
+    def reads_sample_bytes_completed(self) -> int: ...
+
+def compress_signal(
+    signal: npt.NDArray[np.int16], compressed_signal_out: npt.NDArray[np.uint8]
+) -> int: ...
+def create_file(
+    src_filename: str, writer_name: str, options: Optional[FileWriterOptions]
+) -> FileWriter: ...
+def recover_file(src_filename: str, dst_filename: str) -> FileWriter: ...
+def decompress_signal(
+    compressed_signal: Union[npt.NDArray[np.uint8], memoryview],
+    signal_out: npt.NDArray[np.int16],
+) -> None: ...
+def format_read_id_to_str(
+    read_id_data_out: npt.NDArray[np.uint8],
+) -> List[str]: ...
+def get_error_string() -> str: ...
+def load_read_id_iterable(
+    read_ids_str: Iterable, read_id_data_out: npt.NDArray[np.uint8]
+) -> int: ...
+def open_file(filename: str) -> Pod5FileReader: ...
+def update_file(reader: Pod5FileReader, output: str): ...
+def vbz_compressed_signal_max_size(sample_count: int) -> int: ...
```

## Comparing `lib_pod5-0.2.2.dist-info/METADATA` & `lib_pod5-0.2.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: lib-pod5
-Version: 0.2.2
-Summary: Python bindings for the POD5 file format
-Author-email: "Oxford Nanopore Technologies, Limited" <support@nanoporetech.com>
-Keywords: nanopore
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Provides-Extra: dev
-Requires-Dist: build ; extra == 'dev'
-Requires-Dist: pytest (~=7.3) ; extra == 'dev'
-
-LIB_POD5 Package
-================
-
-POD5 is a file format for storing nanopore dna data in an easily accessible way.
-
-What does this project contain
-------------------------------
-
-This project contains the low-level core library (extension modules) for reading and
-writing POD5 files. This project forms the basis of the pure-python `pod5` package which
-is probably the project you want.
+Metadata-Version: 2.1
+Name: lib-pod5
+Version: 0.2.3
+Summary: Python bindings for the POD5 file format
+Author-email: Oxford Nanopore Technologies plc <support@nanoporetech.com>
+Keywords: nanopore
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Provides-Extra: dev
+Requires-Dist: build ; extra == 'dev'
+Requires-Dist: pytest (~=7.3) ; extra == 'dev'
+
+LIB_POD5 Package
+================
+
+POD5 is a file format for storing nanopore dna data in an easily accessible way.
+
+What does this project contain
+------------------------------
+
+This project contains the low-level core library (extension modules) for reading and
+writing POD5 files. This project forms the basis of the pure-python `pod5` package which
+is probably the project you want.
```

