# Comparing `tmp/clp_logging-0.0.8.tar.gz` & `tmp/clp_logging-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/liondavi/src/yscope/loglib-py/dist/.tmp-ww0_cnk5/clp_logging-0.0.8.tar", last modified: Tue Mar 21 03:47:44 2023, max compression
+gzip compressed data, was "/home/liondavi/src/yscope/loglib-py/dist/.tmp-af5fi76e/clp_logging-0.0.9.tar", last modified: Sat Apr  1 23:14:26 2023, max compression
```

## Comparing `clp_logging-0.0.8.tar` & `clp_logging-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.820881 clp_logging-0.0.8/
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.816881 clp_logging-0.0.8/.github/
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.816881 clp_logging-0.0.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1127 2022-12-14 21:43:24.000000 clp_logging-0.0.8/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       27 2022-12-14 21:27:56.000000 clp_logging-0.0.8/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      557 2022-12-14 21:43:38.000000 clp_logging-0.0.8/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      283 2022-12-14 22:22:09.000000 clp_logging-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       99 2022-10-27 18:41:44.000000 clp_logging-0.0.8/.gitignore
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    11341 2022-10-27 18:41:44.000000 clp_logging-0.0.8/LICENSE
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     7186 2023-03-21 03:47:44.820881 clp_logging-0.0.8/PKG-INFO
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1662 2022-10-27 18:41:44.000000 clp_logging-0.0.8/README-protocol.md
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     6703 2023-03-21 02:34:37.000000 clp_logging-0.0.8/README.md
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      861 2023-03-21 03:45:43.000000 clp_logging-0.0.8/pyproject.toml
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      305 2022-10-27 18:41:44.000000 clp_logging-0.0.8/requirements-dev.txt
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       38 2023-03-21 03:47:44.820881 clp_logging-0.0.8/setup.cfg
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.816881 clp_logging-0.0.8/src/
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.820881 clp_logging-0.0.8/src/clp_logging/
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        0 2022-10-27 18:41:44.000000 clp_logging-0.0.8/src/clp_logging/__init__.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     5765 2023-03-21 00:13:41.000000 clp_logging-0.0.8/src/clp_logging/decoder.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    11899 2023-01-24 21:34:11.000000 clp_logging-0.0.8/src/clp_logging/encoder.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    28199 2023-03-21 03:41:18.000000 clp_logging-0.0.8/src/clp_logging/handlers.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     3729 2023-03-21 00:13:41.000000 clp_logging-0.0.8/src/clp_logging/protocol.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        0 2022-10-27 18:41:44.000000 clp_logging-0.0.8/src/clp_logging/py.typed
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    15082 2023-03-21 00:13:41.000000 clp_logging-0.0.8/src/clp_logging/readers.py
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.820881 clp_logging-0.0.8/src/clp_logging.egg-info/
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     7186 2023-03-21 03:47:44.000000 clp_logging-0.0.8/src/clp_logging.egg-info/PKG-INFO
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      656 2023-03-21 03:47:44.000000 clp_logging-0.0.8/src/clp_logging.egg-info/SOURCES.txt
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        1 2023-03-21 03:47:44.000000 clp_logging-0.0.8/src/clp_logging.egg-info/dependency_links.txt
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       66 2023-03-21 03:47:44.000000 clp_logging-0.0.8/src/clp_logging.egg-info/requires.txt
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       12 2023-03-21 03:47:44.000000 clp_logging-0.0.8/src/clp_logging.egg-info/top_level.txt
-drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-03-21 03:47:44.820881 clp_logging-0.0.8/tests/
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1171 2023-02-21 19:25:43.000000 clp_logging-0.0.8/tests/__init__.py
--rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    17296 2023-03-21 03:41:18.000000 clp_logging-0.0.8/tests/test_handlers.py
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.655584 clp_logging-0.0.9/
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.651584 clp_logging-0.0.9/.github/
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.651584 clp_logging-0.0.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1127 2022-12-14 21:43:24.000000 clp_logging-0.0.9/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       27 2022-12-14 21:27:56.000000 clp_logging-0.0.9/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      557 2022-12-14 21:43:38.000000 clp_logging-0.0.9/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      283 2022-12-14 22:22:09.000000 clp_logging-0.0.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       99 2022-10-27 18:41:44.000000 clp_logging-0.0.9/.gitignore
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    11341 2022-10-27 18:41:44.000000 clp_logging-0.0.9/LICENSE
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     9040 2023-04-01 23:14:26.655584 clp_logging-0.0.9/PKG-INFO
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1662 2022-10-27 18:41:44.000000 clp_logging-0.0.9/README-protocol.md
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     8557 2023-04-01 22:46:30.000000 clp_logging-0.0.9/README.md
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      861 2023-04-01 23:12:58.000000 clp_logging-0.0.9/pyproject.toml
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      300 2023-04-01 23:01:02.000000 clp_logging-0.0.9/requirements-dev.txt
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       38 2023-04-01 23:14:26.655584 clp_logging-0.0.9/setup.cfg
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.651584 clp_logging-0.0.9/src/
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.655584 clp_logging-0.0.9/src/clp_logging/
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        0 2022-10-27 18:41:44.000000 clp_logging-0.0.9/src/clp_logging/__init__.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     5920 2023-03-31 01:52:34.000000 clp_logging-0.0.9/src/clp_logging/decoder.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    11899 2023-03-27 01:02:49.000000 clp_logging-0.0.9/src/clp_logging/encoder.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    29991 2023-03-31 01:52:34.000000 clp_logging-0.0.9/src/clp_logging/handlers.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     3586 2023-03-27 01:02:41.000000 clp_logging-0.0.9/src/clp_logging/protocol.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        0 2022-10-27 18:41:44.000000 clp_logging-0.0.9/src/clp_logging/py.typed
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    27613 2023-04-01 22:46:30.000000 clp_logging-0.0.9/src/clp_logging/readers.py
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.655584 clp_logging-0.0.9/src/clp_logging.egg-info/
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     9040 2023-04-01 23:14:26.000000 clp_logging-0.0.9/src/clp_logging.egg-info/PKG-INFO
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)      656 2023-04-01 23:14:26.000000 clp_logging-0.0.9/src/clp_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)        1 2023-04-01 23:14:26.000000 clp_logging-0.0.9/src/clp_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       66 2023-04-01 23:14:26.000000 clp_logging-0.0.9/src/clp_logging.egg-info/requires.txt
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)       12 2023-04-01 23:14:26.000000 clp_logging-0.0.9/src/clp_logging.egg-info/top_level.txt
+drwxr-xr-x   0 liondavi (1000006) Domain Users (1000000)        0 2023-04-01 23:14:26.655584 clp_logging-0.0.9/tests/
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)     1315 2023-04-01 22:46:30.000000 clp_logging-0.0.9/tests/__init__.py
+-rw-r--r--   0 liondavi (1000006) Domain Users (1000000)    25546 2023-04-01 22:46:30.000000 clp_logging-0.0.9/tests/test_handlers.py
```

### Comparing `clp_logging-0.0.8/.github/ISSUE_TEMPLATE/bug-report.yml` & `clp_logging-0.0.9/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/.github/ISSUE_TEMPLATE/feature-request.yml` & `clp_logging-0.0.9/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/LICENSE` & `clp_logging-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/PKG-INFO` & `clp_logging-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,179 @@
-Metadata-Version: 2.1
-Name: clp_logging
-Version: 0.0.8
-Summary: Logging/encoding/decoding using CLP's IR stream format
-Author-email: david lion <david.lion@yscope.com>
-License: Apache License 2.0
-Project-URL: Homepage, https://github.com/y-scope/clp-loglib-py
-Project-URL: Bug Tracker, https://github.com/y-scope/clp-loglib-py/issues
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CLP Python Logging Library
+
 This is a Python `logging` library meant to supplement [CLP (Compressed Log Processor)][0].
 Logs are compressed in a streaming fashion into CLP's Internal Representation (IR) format before written to disk.
-More details are described in this [Uber's blog][1].  
+More details are described in this [Uber's blog][1].
 
-Logs compressed in IR format can be viewed in a [log viewer][2] or programmatically analyzed using 
-APIs provided here. They can also be decompressed back into plain-text log files using [CLP][0] (in a future release).    
+Logs compressed in IR format can be viewed in a [log viewer][2] or programmatically analyzed using
+APIs provided here. They can also be decompressed back into plain-text log files using [CLP][0] (in a future release).
 
 To achieve the best compression ratio, CLP should be used to compress large
 batches of logs, one batch at a time. However, individual log
 files are generally small and are generated across a long period of time.
 
 This logging library helps solve this problem by logging directly in CLP's
 Internal Representation (IR). A log created with a CLP logging handler is first
 parsed and then appended to a compressed output stream in IR form.
 See [README-protocol.md](README-protocol.md) for more details on the format of
 CLP IR.
 
 These log files containing the compressed CLP IR streams can then all be
 ingested into CLP together at a later time.
 
-[0]: https://github.com/y-scope/clp
-[1]: https://www.uber.com/blog/reducing-logging-cost-by-two-orders-of-magnitude-using-clp/
-[2]: https://github.com/y-scope/yscope-log-viewer
-
 ## Quick Start
+
 The package is hosted with pypi (https://pypi.org/project/clp-logging/), so it
 can be installed with `pip`:
 
 `python3 -m pip install --upgrade clp-logging`
 
 ## Logger handlers
+
 ### CLPStreamHandler
+
 - Writes encoded logs directly to a stream
+
 ### CLPFileHandler
+
 - Simple wrapper around CLPStreamHandler that calls open
+
 #### Example: CLPFileHandler
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPFileHandler
 
 clp_handler = CLPFileHandler(Path("example.clp.zst"))
 logger = logging.getLogger(__name__)
 logger.addHandler(clp_handler)
 logger.warn("example warning")
 ```
 
 ### CLPSockHandler + CLPSockListener
 
 This library also supports multiple processes writing to the same log file.
-In this case, all logging processes write to a listener server process through a TCP socket.  
+In this case, all logging processes write to a listener server process through a TCP socket.
 The socket name is the log file path passed to CLPSockHandler with a ".sock" suffix.
 
 A CLPSockListener can be explicitly created (and will run as a daemon) by calling:
  `CLPSockListener.fork(log_path, sock_path, timezone, timestamp_format)`.
 Alternatively CLPSockHandlers can transparently start an associated CLPSockListener
 by calling `CLPSockHandler` with `create_listener=True`.
 
-CLPSockListener must be explicitly stopped once logging is completed. 
+CLPSockListener must be explicitly stopped once logging is completed.
 There are two ways to stop the listener process:
- - Calling `stop_listener()` from an existing handler, e.g., `clp_handler.stop_listener()`, or from a new handler with the same log path, e.g., `CLPSockHandler(Path("example.clp.zst")).stop_listener()`
- - Kill the CLPSockListener process with SIGTERM
+
+- Calling `stop_listener()` from an existing handler, e.g., `clp_handler.stop_listener()`, or from a new handler with the same log path, e.g., `CLPSockHandler(Path("example.clp.zst")).stop_listener()`
+- Kill the CLPSockListener process with SIGTERM
 
 #### Example: CLPSockHandler + CLPSockListener
+
 In the handler processes or threads:
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPSockHandler
 
 clp_handler = CLPSockHandler(Path("example.clp.zst"), create_listener=True)
 logger = logging.getLogger(__name__)
 logger.addHandler(clp_handler)
 logger.warn("example warning")
 ```
+
 In a single process or thread once logging is completed:
+
 ```python
 from pathlib import Path
 from clp_logging.handlers import CLPSockHandler
 
 CLPSockHandler(Path("example.clp.zst")).stop_listener()
 ```
 
 ## CLP readers (decoders)
+
 ### CLPStreamReader
+
 - Read/decode any arbitrary stream
 - Can be used as an iterator that returns each log message as an object
 - Can skip n logs: `clp_reader.skip_nlogs(N)`
 - Can skip to first log after given time (since unix epoch):
-    - `clp_reader.skip_to_time(TIME)`
+  - `clp_reader.skip_to_time(TIME)`
 
 ### CLPFileReader
+
 - Simple wrapper around CLPStreamHandler that calls open
 
 #### Example code: CLPFileReader
+
 ```python
 from pathlib import Path
 from typing import List
 
 from clp_logging.readers import CLPFileReader, Log
 
 # create a list of all Log objects
 log_objects: List[Log] = []
 with CLPFileReader(Path("example.clp.zst")) as clp_reader:
     for log in clp_reader:
         log_objects.append(log)
 ```
 
+### CLPSegmentStreaming
+
+* Classes inheriting CLPBaseReader are only capable of reading a single CLP IR stream from start to finish. This is required as to know the timestamp of an individual log, the starting timestamp (from the IR stream preamble) and all timestamp deltas up to that log must be known. In scenarios where a IR stream is periodically uploaded in chunks, users would need to either continuously read the entire stream or re-read the entire stream from the start.
+* The CLPSegmentStreaming class has the ability to take an input IR stream and segment it, outputting multiple independent IR streams. This makes it possible to read arbitrary segments of the original input IR stream without needing to decode it from the start.
+* In technical terms, the segment streaming reader allows the read operation to start from a non-zero offset, and streams the legal encoded logs from one stream to another.
+* Each read call will return an encoded metadata which can be used to resume from the current call.S
+
+#### Example code: CLPSegmentStreaming
+
+```python
+from clp_logging.readers import CLPSegmentStreaming
+from clp_logging.protocol import Metadata
+
+segment_idx: int = 0
+segment_max_size: int = 8192
+offset: int = 0
+metadata: Metadata = None
+while True:
+	bytes_read: int
+	with open("example.clp", "rb") as fin, open(f"{segment_idx}.clp", "wb") as fout:
+		bytes_read, metadata = CLPSegmentStreaming.read(
+			fin,
+			fout,
+			offset=offset,
+			max_bytes_to_write=segment_max_size,
+			metadata=metadata
+		)
+		segment_idx += 1
+		offset += bytes_read
+	if metadata == None:
+		break
+```
+
+In the example code provided, "example.clp" is streamed into segments named "0.clp", "1.clp", and so on. Each segment is smaller than 8192 bytes and can be decoded independently.
+
 ## Log level timeout feature: CLPLogLevelTimeout
 
 All log handlers support a configurable timeout feature. A (user configurable)
 timeout will be scheduled based on logs' logging level (verbosity) that will
 flush the zstandard frame and allow users to run arbitrary code.
 This feature allows users to automatically perform log related tasks, such as
 periodically uploading their logs for storage. By setting the timeout in
 response to the logs' logging level the responsiveness of a task can be
 adjusted based on the severity of logging level seen.
 An additional timeout is always triggered on closing the logging handler.
 
 See the class documentation for specific details.
 
 #### Example code: CLPLogLevelTimeout
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPLogLevelTimeout, CLPSockHandler
 
 class LogTimeoutUploader:
     # Store relevent information/objects to carry out the timeout task
@@ -157,33 +193,44 @@
 uploader = LogTimeoutUploader(log_path)
 loglevel_timeout = CLPLogLevelTimeout(uploader.timeout)
 clp_handler = CLPSockHandler(log_path, create_listener=True, loglevel_timeout=loglevel_timeout)
 logging.getLogger(__name__).addHandler(clp_handler)
 ```
 
 ## Compatibility
+
 Tested on Python 3.6 and 3.8 and should work on any newer version.
 Built/packaged on Python 3.8 for convenience regarding type annotation.
 
 ## Building/Packaging
+
 1. Create and enter a virtual environment:
-    `python3.8 -m venv venv; . ./venv/bin/activate`
+   `python3.8 -m venv venv; . ./venv/bin/activate`
 2. Install development dependencies:
-    `pip install -r requirements-dev.txt`
+   `pip install -r requirements-dev.txt`
 3. Build:
-    `python -m build`
+   `python -m build`
 
 ## Testing
+
 Note the baseline comparison logging handler and the CLP handler both get
 unique timestamps. It is possible for these timestamps to differ, which will
 result in a test reporting a false positive error.
+
 1. Create and enter a virtual environment:
-    `python -m venv venv; .  ./venv/bin/activate`
-2. Install:
-    `pip install dist/clp_logging-*-py3-none-any.whl` or `pip install -e .`
-3. Run unittest:
-    `python -m unittest -bv`
+   `python -m venv venv; .  ./venv/bin/activate`
+2. Install development dependencies:
+   `pip install -r requirements-dev.txt`
+3. Install:
+   `pip install dist/clp_logging-*-py3-none-any.whl` or `pip install -e .`
+4. Run unittest:
+   `python -m unittest -bv`
 
 ## Contributing
+
 Ensure to run `mypy` and `black` (found in
 [requirements-dev.txt](requirements-dev.txt)) during development to ensure
 smooth pull requests.
+
+[0]: https://github.com/y-scope/clp
+[1]: https://www.uber.com/blog/reducing-logging-cost-by-two-orders-of-magnitude-using-clp/
+[2]: https://github.com/y-scope/yscope-log-viewer
```

### Comparing `clp_logging-0.0.8/README-protocol.md` & `clp_logging-0.0.9/README-protocol.md`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/pyproject.toml` & `clp_logging-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clp_logging"
-version = "0.0.8"
+version = "0.0.9"
 license = { text = "Apache License 2.0" }
 authors = [
     { name="david lion", email="david.lion@yscope.com" },
 ]
 description = "Logging/encoding/decoding using CLP's IR stream format"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `clp_logging-0.0.8/src/clp_logging/decoder.py` & `clp_logging-0.0.9/src/clp_logging/decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             return None, -1
         pos += magic_len
         encoding_len: int = len(METADATA_JSON_ENCODING)
         if not view[pos : pos + encoding_len] == METADATA_JSON_ENCODING:
             return None, -2
         pos += encoding_len
 
-        type_byte: bytes = view[pos : pos + 1]
+        type_byte: bytes = view[pos : pos + SIZEOF_BYTE]
         pos += SIZEOF_BYTE
         json_size: int
         if type_byte == METADATA_LEN_UBYTE:
             json_size = int.from_bytes(view[pos : pos + SIZEOF_BYTE], BYTE_ORDER)
             pos += SIZEOF_BYTE
         elif type_byte == METADATA_LEN_USHORT:
             json_size = int.from_bytes(view[pos : pos + SIZEOF_SHORT], BYTE_ORDER)
@@ -108,58 +108,56 @@
         `bytes`). Therefore `token_type` (`type_byte[0]`) can never be
         negative.
 
         :param src: Bytes to decode
         :param pos: The position in `src` to begin decoding from
         :return: A tuple of the token type byte, the token in bytes, and the
         index read up to in `src` (including `pos`). Token type is 0 for
-        EOF_CHAR, -1 if `src` is exhausted before completing a token, or -2 on
-        error.
+        EOF_CHAR, -1 if `src` is exhausted before completing a token, or < -1
+        for other errors.
         """
-        type_byte: memoryview = src[pos : pos + 1]
-        token_type: int = type_byte[0]
+        # We cannot directly get a single byte at pos with src[pos] as this
+        # will return an integer and we still need to do byte comparisons
+        # later.
+        type_byte: memoryview = src[pos : pos + SIZEOF_BYTE]
         pos += SIZEOF_BYTE
+        if type_byte == EOF_CHAR:
+            return ID_EOF, type_byte, pos
 
         info: Optional[Tuple[int, bool]] = SIZEOF.get(type_byte.tobytes())
         if not info:
-            return -2, type_byte, pos
+            return -3, type_byte, pos
 
         size: int
         signed: bool
         size, signed = info
         end: int = pos + size
         src_len: int = len(src)
         if end >= src_len:
             return -1, type_byte, end
 
+        # SIZEOF_BYTE can only ever be 1 to match the size of an element in a
+        # bytes-like python object. Therefore, we can get the integer value of
+        # type_byte by indexing it.
+        token_type: int = type_byte[0]
         token_id: int = token_type & ID_MASK
         if token_id == ID_VAR:
             if type_byte == VAR_COMPACT_ENCODING:
                 return token_type, src[pos:end], end
             else:
                 var_size: int = int.from_bytes(src[pos:end], BYTE_ORDER, signed=signed)
                 pos = end
                 end += var_size
                 if end >= src_len:
                     return -1, type_byte, end
                 return token_type, src[pos:end], end
-
         elif token_id == ID_LOGTYPE:
             logtype_size: int = int.from_bytes(src[pos:end], BYTE_ORDER, signed=signed)
             pos = end
             end += logtype_size
             if end >= src_len:
                 return -1, type_byte, end
             return token_type, src[pos:end], end
-
         elif token_id == ID_TIMESTAMP:
             return token_type, src[pos:end], end
-
-        elif token_id == ID_EOF:
-            # Calling `zstream.flush(FLUSH_FRAME)` seems to leave
-            # \x00\x00\x00\xc9 between frames.
-            if b"\x00\x00\x00\xc9" == src[pos:end]:
-                return token_type, type_byte, end
-            else:
-                return -4, type_byte, end
         else:
-            return -3, type_byte, end
+            return -2, type_byte, end
```

### Comparing `clp_logging-0.0.8/src/clp_logging/encoder.py` & `clp_logging-0.0.9/src/clp_logging/encoder.py`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/src/clp_logging/handlers.py` & `clp_logging-0.0.9/src/clp_logging/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABCMeta, abstractmethod
 import logging
 import os
 import time
-from datetime import datetime
+from datetime import datetime, tzinfo
 from math import floor
 from pathlib import Path
 from queue import Empty, Queue
 from signal import signal, SIGINT, SIGTERM
 import socket
 from threading import Thread, Timer
 import sys
 from types import FrameType
-from typing import Callable, ClassVar, Dict, IO, List, Optional, Tuple, TypeVar
+from typing import Callable, ClassVar, Dict, IO, List, Optional, Tuple, TypeVar, Union
 
 import dateutil.tz
 from zstandard import FLUSH_FRAME, ZstdCompressor, ZstdCompressionWriter
 
 from clp_logging.encoder import CLPEncoder
 from clp_logging.protocol import (
     BYTE_ORDER,
@@ -32,33 +32,40 @@
 
 DEFAULT_LOG_FORMAT: str = " %(levelname)s %(name)s %(message)s"
 WARN_PREFIX: str = " [WARN][clp_logging]"
 
 
 def _init_timeinfo(fmt: Optional[str], tz: Optional[str]) -> Tuple[str, str]:
     """
-    Set default timestamp format or timezone if not specified.
-    In the future sanitization of user input should also go here.
-    Currently, timestamp format defaults to a format for the Java readers, due
+    Return the timestamp format and timezone (in TZID format) that should be
+    used. If not specified by the user, this function will choose default
+    values to use.
+    The timestamp format (`fmt`) defaults to a format for the Java readers, due
     to compatibility issues between language time libraries.
     (`datatime.isoformat` is always used for the timestamp format in python
     readers.)
+    The timzeone format (`tz`) first defaults to the system local timezone. If
+    that fails it will default to UTC.
+    In the future sanitization of user input should also go here.
+
     :param fmt: Timestamp format written in preamble to be used when generating
     the logs with a reader.
     :param tz: Timezone in TZID format written in preamble to be used when
     generating the timestamp from Unix epoch time.
+    :return: Tuple of timestamp format string and timezone in TZID format.
     """
     if not fmt:
         fmt = "yyyy-MM-d H:m:s.A"
     if not tz:
-        tzf = dateutil.tz.gettz()
+        tzf: Optional[tzinfo] = dateutil.tz.gettz()
         if tzf:
-            if tzf._filename == "/etc/localtime":
-                tzp = Path.resolve(Path(tzf._filename))
+            tzp: Path = Path.resolve(Path(tzf._filename))  # type: ignore
             tz = "/".join([tzp.parent.name, tzp.name])
+        else:
+            tz = "UTC"
     return fmt, tz
 
 
 class CLPBaseHandler(logging.Handler, metaclass=ABCMeta):
     def __init__(self) -> None:
         super().__init__()
         self.formatter: logging.Formatter = logging.Formatter(DEFAULT_LOG_FORMAT)
@@ -194,36 +201,39 @@
 
         """
         self.hard_timeout_deltas: Dict[int, int] = hard_timeout_deltas
         self.soft_timeout_deltas: Dict[int, int] = soft_timeout_deltas
         self.timeout_fn: Callable[[], None] = timeout_fn
         self.next_hard_timeout_ts: int = ULONG_MAX
         self.min_soft_timeout_delta: int = ULONG_MAX
-        self.zstream: Optional[ZstdCompressionWriter] = None
+        self.ostream: Optional[Union[ZstdCompressionWriter, IO[bytes]]] = None
         self.hard_timeout_thread: Optional[Timer] = None
         self.soft_timeout_thread: Optional[Timer] = None
 
-    def set_zstream(self, zstream: ZstdCompressionWriter) -> None:
-        self.zstream = zstream
+    def set_ostream(self, ostream: Union[ZstdCompressionWriter, IO[bytes]]) -> None:
+        self.ostream = ostream
 
     def timeout(self) -> None:
         """
         Wraps the call to the user supplied `timeout_fn` ensuring that any
         existing timeout threads are cancelled, `next_hard_timeout_ts` and
         `min_soft_timeout_delta` are reset, and the zstandard frame is flushed.
         """
         if self.hard_timeout_thread:
             self.hard_timeout_thread.cancel()
         if self.soft_timeout_thread:
             self.soft_timeout_thread.cancel()
         self.next_hard_timeout_ts = ULONG_MAX
         self.min_soft_timeout_delta = ULONG_MAX
 
-        if self.zstream:
-            self.zstream.flush(FLUSH_FRAME)
+        if self.ostream:
+            if isinstance(self.ostream, ZstdCompressionWriter):
+                self.ostream.flush(FLUSH_FRAME)
+            else:
+                self.ostream.flush()
         self.timeout_fn()
 
     def update(self, loglevel: int, log_timestamp_ms: int, log_fn: Callable[[str], None]) -> None:
         """
         Carries out the logic to schedule the next timeout based on the current
         log.
 
@@ -360,74 +370,87 @@
     @staticmethod
     def _aggregator(
         log_path: Path,
         log_queue: "Queue[Tuple[int, bytes]]",
         timestamp_format: Optional[str],
         timezone: Optional[str],
         timeout: int,
+        enable_compression: bool,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> int:
         """
         Continuously receive encoded messages from
         `CLPSockListener._handle_client` threads and write them to a Zstandard
         stream.
         :param log_path: Path to log file and used to derive socket name.
         :param log_queue: Queue with `CLPSockListener._handle_client` threads
         to write encoded messages.
         :param timestamp_format: Timestamp format written in preamble to be
         used when generating the logs with a reader.
         :param timezone: Timezone written in preamble to be used when
         generating the timestamp from Unix epoch time.
         :param timeout: timeout in seconds to prevent `Queue.get` from never
+        :param enable_compression: use the zstd compress if setting to True
         returning and not closing properly on signal/EOF_CHAR.
         :return: 0 on successful exit
         """
         cctx: ZstdCompressor = ZstdCompressor()
         timestamp_format, timezone = _init_timeinfo(timestamp_format, timezone)
         last_timestamp_ms: int = floor(time.time() * 1000)  # convert to ms and truncate
 
-        with log_path.open("ab") as log, cctx.stream_writer(log) as zstream:
+        with log_path.open("ab") as log:
+            # Since the compression may be disabled, context manager is not used
+            ostream: Union[ZstdCompressionWriter, IO[bytes]] = (
+                cctx.stream_writer(log) if enable_compression else log
+            )
+
             if loglevel_timeout:
-                loglevel_timeout.set_zstream(zstream)
+                loglevel_timeout.set_ostream(ostream)
 
             def log_fn(msg: str) -> None:
                 nonlocal last_timestamp_ms
                 buf: bytearray = bytearray(CLPEncoder.encode_message(msg.encode()))
                 last_timestamp_ms = CLPEncoder.encode_timestamp(last_timestamp_ms, buf)
-                zstream.write(buf)
+                ostream.write(buf)
 
-            zstream.write(CLPEncoder.emit_preamble(last_timestamp_ms, timestamp_format, timezone))
+            ostream.write(CLPEncoder.emit_preamble(last_timestamp_ms, timestamp_format, timezone))
             while not CLPSockListener._signaled:
                 msg: bytes
                 try:
                     loglevel, msg = log_queue.get(timeout=timeout)
                 except Empty:
                     continue
                 if msg == EOF_CHAR:
                     break
                 buf: bytearray = bytearray(msg)
                 last_timestamp_ms = CLPEncoder.encode_timestamp(last_timestamp_ms, buf)
                 if loglevel_timeout:
                     loglevel_timeout.update(loglevel, last_timestamp_ms, log_fn)
-                zstream.write(buf)
+                ostream.write(buf)
             if loglevel_timeout:
                 loglevel_timeout.timeout()
-            zstream.write(EOF_CHAR)
+            ostream.write(EOF_CHAR)
+
+            if enable_compression:
+                # Since we are not using context manager, the ostream should be
+                # explicitly closed.
+                ostream.close()
         # tell _server to exit
         CLPSockListener._signaled = True
         return 0
 
     @staticmethod
     def _server(
         parent_fd: int,
         log_path: Path,
         sock_path: Path,
         timestamp_format: Optional[str],
         timezone: Optional[str],
         timeout: int,
+        enable_compression: bool,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> int:
         """
         The `CLPSockListener` server function run in a new process.
         Writes 1 byte back to parent process for synchronization.
         :param parent_fd: Used to communicate to parent `CLPSockHandler`
         process that `_try_bind` has finished.
@@ -451,15 +474,23 @@
             return ret
 
         signal(SIGINT, CLPSockListener._exit_handler)
         signal(SIGTERM, CLPSockListener._exit_handler)
 
         Thread(
             target=CLPSockListener._aggregator,
-            args=(log_path, log_queue, timestamp_format, timezone, timeout, loglevel_timeout),
+            args=(
+                log_path,
+                log_queue,
+                timestamp_format,
+                timezone,
+                timeout,
+                enable_compression,
+                loglevel_timeout,
+            ),
             daemon=False,
         ).start()
 
         while not CLPSockListener._signaled:
             conn: socket.socket
             addr: Tuple[str, int]
             try:
@@ -476,14 +507,15 @@
 
     @staticmethod
     def fork(
         log_path: Path,
         timestamp_format: Optional[str],
         timezone: Optional[str],
         timeout: int,
+        enable_compression: bool,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> int:
         """
         Fork a process running `CLPSockListener._server` and use `os.setsid()`
         to give it another session id (and process group id). The parent will
         not return until the forked listener has either bound the socket
         or finished trying to.
@@ -501,15 +533,22 @@
         wfd: int
         rfd, wfd = os.pipe()
         pid: int = os.fork()
         if pid == 0:
             os.setsid()
             sys.exit(
                 CLPSockListener._server(
-                    wfd, log_path, sock_path, timestamp_format, timezone, timeout, loglevel_timeout
+                    wfd,
+                    log_path,
+                    sock_path,
+                    timestamp_format,
+                    timezone,
+                    timeout,
+                    enable_compression,
+                    loglevel_timeout,
                 )
             )
         else:
             os.read(rfd, 1)
         return pid
 
 
@@ -524,14 +563,15 @@
     def __init__(
         self,
         log_path: Path,
         create_listener: bool = False,
         timestamp_format: Optional[str] = None,
         timezone: Optional[str] = None,
         timeout: int = 2,
+        enable_compression: bool = True,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> None:
         """
         Constructor method that optionally spawns a `CLPSockListener`.
         :param log_path: Path to log file written by `CLPSockListener` used to
         derive socket name.
         :param create_listener: If true and the handler could not connect to an
@@ -551,15 +591,20 @@
         self.closed: bool = False
         self.sock: socket.socket = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
         self.listener_pid: int = 0
 
         if self.sock.connect_ex(str(self.sock_path)) != 0:
             if create_listener:
                 self.listener_pid = CLPSockListener.fork(
-                    log_path, timestamp_format, timezone, timeout, loglevel_timeout
+                    log_path,
+                    timestamp_format,
+                    timezone,
+                    timeout,
+                    enable_compression,
+                    loglevel_timeout,
                 )
 
             # If we fail to connect again, the listener failed to resolve any
             # issues, so we raise an exception as there is nothing new to try
             try:
                 self.sock.connect(str(self.sock_path))
             except OSError:
@@ -619,57 +664,61 @@
     Similar to `logging.StreamHandler`, but the log is written to `stream`
     in CLP IR encoding rather than bytes or a string.
     :param stream: Output stream of bytes to write CLP encoded log messages to
     """
 
     def init(self, stream: IO[bytes]) -> None:
         self.cctx: ZstdCompressor = ZstdCompressor()
-        self.zstream: ZstdCompressionWriter = self.cctx.stream_writer(stream)
+        self.ostream: Union[ZstdCompressionWriter, IO[bytes]] = (
+            self.cctx.stream_writer(stream) if self.enable_compression else stream
+        )
         self.last_timestamp_ms: int = floor(time.time() * 1000)  # convert to ms and truncate
-        self.zstream.write(
+        self.ostream.write(
             CLPEncoder.emit_preamble(self.last_timestamp_ms, self.timestamp_format, self.timezone)
         )
 
     def __init__(
         self,
         stream: Optional[IO[bytes]],
+        enable_compression: bool = True,
         timestamp_format: Optional[str] = None,
         timezone: Optional[str] = None,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> None:
         super().__init__()
         self.closed: bool = False
+        self.enable_compression: bool = enable_compression
         if stream is None:
             stream = sys.stderr.buffer
         self.stream: IO[bytes] = stream
         self.timestamp_format: str
         self.timezone: str
         self.timestamp_format, self.timezone = _init_timeinfo(timestamp_format, timezone)
         self.init(self.stream)
 
         if loglevel_timeout:
-            loglevel_timeout.set_zstream(self.zstream)
+            loglevel_timeout.set_ostream(self.ostream)
         self.loglevel_timeout = loglevel_timeout
 
     def _direct_write(self, msg: str) -> None:
         if self.closed:
             raise RuntimeError("Stream already closed")
         clp_msg: bytearray = CLPEncoder.encode_message(msg.encode())
         self.last_timestamp_ms = CLPEncoder.encode_timestamp(self.last_timestamp_ms, clp_msg)
-        self.zstream.write(clp_msg)
+        self.ostream.write(clp_msg)
 
     # override
     def _write(self, loglevel: int, msg: str) -> None:
         if self.closed:
             raise RuntimeError("Stream already closed")
         clp_msg: bytearray = CLPEncoder.encode_message(msg.encode())
         self.last_timestamp_ms = CLPEncoder.encode_timestamp(self.last_timestamp_ms, clp_msg)
         if self.loglevel_timeout:
             self.loglevel_timeout.update(loglevel, self.last_timestamp_ms, self._direct_write)
-        self.zstream.write(clp_msg)
+        self.ostream.write(clp_msg)
 
     # Added to logging.StreamHandler in python 3.7
     # override
     def setStream(self, stream: IO[bytes]) -> Optional[IO[bytes]]:
         if not self.stream:
             self.stream = stream
             self.init(stream)
@@ -686,26 +735,29 @@
                 self.release()
             return self.stream
 
     # override
     def close(self) -> None:
         if self.loglevel_timeout:
             self.loglevel_timeout.timeout()
-        self.zstream.write(EOF_CHAR)
-        self.zstream.close()
+        self.ostream.write(EOF_CHAR)
+        self.ostream.close()
         self.closed = True
         super().close()
 
 
 class CLPFileHandler(CLPStreamHandler):
     """Wrapper class that calls `open` for convenience."""
 
     def __init__(
         self,
         fpath: Path,
         mode: str = "ab",
+        enable_compression: bool = True,
         timestamp_format: Optional[str] = None,
         timezone: Optional[str] = None,
         loglevel_timeout: Optional[CLPLogLevelTimeout] = None,
     ) -> None:
         self.fpath: Path = fpath
-        super().__init__(open(fpath, mode), timestamp_format, timezone, loglevel_timeout)
+        super().__init__(
+            open(fpath, mode), enable_compression, timestamp_format, timezone, loglevel_timeout
+        )
```

### Comparing `clp_logging-0.0.8/src/clp_logging/protocol.py` & `clp_logging-0.0.9/src/clp_logging/protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,11 +87,8 @@
     VAR_STR_LEN_INT: (SIZEOF_INT, True),
     LOGTYPE_STR_LEN_UBYTE: (SIZEOF_BYTE, False),
     LOGTYPE_STR_LEN_USHORT: (SIZEOF_SHORT, False),
     LOGTYPE_STR_LEN_INT: (SIZEOF_INT, True),
     TIMESTAMP_DELTA_BYTE: (SIZEOF_BYTE, True),
     TIMESTAMP_DELTA_SHORT: (SIZEOF_SHORT, True),
     TIMESTAMP_DELTA_INT: (SIZEOF_INT, True),
-    # This is used to handle distinguishing null bytes from flushing a
-    # zstandard frame and actual eof
-    EOF_CHAR: (SIZEOF_INT, False),
 }
```

### Comparing `clp_logging-0.0.8/src/clp_logging.egg-info/PKG-INFO` & `clp_logging-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,192 @@
 Metadata-Version: 2.1
-Name: clp-logging
-Version: 0.0.8
+Name: clp_logging
+Version: 0.0.9
 Summary: Logging/encoding/decoding using CLP's IR stream format
 Author-email: david lion <david.lion@yscope.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/y-scope/clp-loglib-py
 Project-URL: Bug Tracker, https://github.com/y-scope/clp-loglib-py/issues
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CLP Python Logging Library
+
 This is a Python `logging` library meant to supplement [CLP (Compressed Log Processor)][0].
 Logs are compressed in a streaming fashion into CLP's Internal Representation (IR) format before written to disk.
-More details are described in this [Uber's blog][1].  
+More details are described in this [Uber's blog][1].
 
-Logs compressed in IR format can be viewed in a [log viewer][2] or programmatically analyzed using 
-APIs provided here. They can also be decompressed back into plain-text log files using [CLP][0] (in a future release).    
+Logs compressed in IR format can be viewed in a [log viewer][2] or programmatically analyzed using
+APIs provided here. They can also be decompressed back into plain-text log files using [CLP][0] (in a future release).
 
 To achieve the best compression ratio, CLP should be used to compress large
 batches of logs, one batch at a time. However, individual log
 files are generally small and are generated across a long period of time.
 
 This logging library helps solve this problem by logging directly in CLP's
 Internal Representation (IR). A log created with a CLP logging handler is first
 parsed and then appended to a compressed output stream in IR form.
 See [README-protocol.md](README-protocol.md) for more details on the format of
 CLP IR.
 
 These log files containing the compressed CLP IR streams can then all be
 ingested into CLP together at a later time.
 
-[0]: https://github.com/y-scope/clp
-[1]: https://www.uber.com/blog/reducing-logging-cost-by-two-orders-of-magnitude-using-clp/
-[2]: https://github.com/y-scope/yscope-log-viewer
-
 ## Quick Start
+
 The package is hosted with pypi (https://pypi.org/project/clp-logging/), so it
 can be installed with `pip`:
 
 `python3 -m pip install --upgrade clp-logging`
 
 ## Logger handlers
+
 ### CLPStreamHandler
+
 - Writes encoded logs directly to a stream
+
 ### CLPFileHandler
+
 - Simple wrapper around CLPStreamHandler that calls open
+
 #### Example: CLPFileHandler
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPFileHandler
 
 clp_handler = CLPFileHandler(Path("example.clp.zst"))
 logger = logging.getLogger(__name__)
 logger.addHandler(clp_handler)
 logger.warn("example warning")
 ```
 
 ### CLPSockHandler + CLPSockListener
 
 This library also supports multiple processes writing to the same log file.
-In this case, all logging processes write to a listener server process through a TCP socket.  
+In this case, all logging processes write to a listener server process through a TCP socket.
 The socket name is the log file path passed to CLPSockHandler with a ".sock" suffix.
 
 A CLPSockListener can be explicitly created (and will run as a daemon) by calling:
  `CLPSockListener.fork(log_path, sock_path, timezone, timestamp_format)`.
 Alternatively CLPSockHandlers can transparently start an associated CLPSockListener
 by calling `CLPSockHandler` with `create_listener=True`.
 
-CLPSockListener must be explicitly stopped once logging is completed. 
+CLPSockListener must be explicitly stopped once logging is completed.
 There are two ways to stop the listener process:
- - Calling `stop_listener()` from an existing handler, e.g., `clp_handler.stop_listener()`, or from a new handler with the same log path, e.g., `CLPSockHandler(Path("example.clp.zst")).stop_listener()`
- - Kill the CLPSockListener process with SIGTERM
+
+- Calling `stop_listener()` from an existing handler, e.g., `clp_handler.stop_listener()`, or from a new handler with the same log path, e.g., `CLPSockHandler(Path("example.clp.zst")).stop_listener()`
+- Kill the CLPSockListener process with SIGTERM
 
 #### Example: CLPSockHandler + CLPSockListener
+
 In the handler processes or threads:
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPSockHandler
 
 clp_handler = CLPSockHandler(Path("example.clp.zst"), create_listener=True)
 logger = logging.getLogger(__name__)
 logger.addHandler(clp_handler)
 logger.warn("example warning")
 ```
+
 In a single process or thread once logging is completed:
+
 ```python
 from pathlib import Path
 from clp_logging.handlers import CLPSockHandler
 
 CLPSockHandler(Path("example.clp.zst")).stop_listener()
 ```
 
 ## CLP readers (decoders)
+
 ### CLPStreamReader
+
 - Read/decode any arbitrary stream
 - Can be used as an iterator that returns each log message as an object
 - Can skip n logs: `clp_reader.skip_nlogs(N)`
 - Can skip to first log after given time (since unix epoch):
-    - `clp_reader.skip_to_time(TIME)`
+  - `clp_reader.skip_to_time(TIME)`
 
 ### CLPFileReader
+
 - Simple wrapper around CLPStreamHandler that calls open
 
 #### Example code: CLPFileReader
+
 ```python
 from pathlib import Path
 from typing import List
 
 from clp_logging.readers import CLPFileReader, Log
 
 # create a list of all Log objects
 log_objects: List[Log] = []
 with CLPFileReader(Path("example.clp.zst")) as clp_reader:
     for log in clp_reader:
         log_objects.append(log)
 ```
 
+### CLPSegmentStreaming
+
+* Classes inheriting CLPBaseReader are only capable of reading a single CLP IR stream from start to finish. This is required as to know the timestamp of an individual log, the starting timestamp (from the IR stream preamble) and all timestamp deltas up to that log must be known. In scenarios where a IR stream is periodically uploaded in chunks, users would need to either continuously read the entire stream or re-read the entire stream from the start.
+* The CLPSegmentStreaming class has the ability to take an input IR stream and segment it, outputting multiple independent IR streams. This makes it possible to read arbitrary segments of the original input IR stream without needing to decode it from the start.
+* In technical terms, the segment streaming reader allows the read operation to start from a non-zero offset, and streams the legal encoded logs from one stream to another.
+* Each read call will return an encoded metadata which can be used to resume from the current call.S
+
+#### Example code: CLPSegmentStreaming
+
+```python
+from clp_logging.readers import CLPSegmentStreaming
+from clp_logging.protocol import Metadata
+
+segment_idx: int = 0
+segment_max_size: int = 8192
+offset: int = 0
+metadata: Metadata = None
+while True:
+	bytes_read: int
+	with open("example.clp", "rb") as fin, open(f"{segment_idx}.clp", "wb") as fout:
+		bytes_read, metadata = CLPSegmentStreaming.read(
+			fin,
+			fout,
+			offset=offset,
+			max_bytes_to_write=segment_max_size,
+			metadata=metadata
+		)
+		segment_idx += 1
+		offset += bytes_read
+	if metadata == None:
+		break
+```
+
+In the example code provided, "example.clp" is streamed into segments named "0.clp", "1.clp", and so on. Each segment is smaller than 8192 bytes and can be decoded independently.
+
 ## Log level timeout feature: CLPLogLevelTimeout
 
 All log handlers support a configurable timeout feature. A (user configurable)
 timeout will be scheduled based on logs' logging level (verbosity) that will
 flush the zstandard frame and allow users to run arbitrary code.
 This feature allows users to automatically perform log related tasks, such as
 periodically uploading their logs for storage. By setting the timeout in
 response to the logs' logging level the responsiveness of a task can be
 adjusted based on the severity of logging level seen.
 An additional timeout is always triggered on closing the logging handler.
 
 See the class documentation for specific details.
 
 #### Example code: CLPLogLevelTimeout
+
 ```python
 import logging
 from pathlib import Path
 from clp_logging.handlers import CLPLogLevelTimeout, CLPSockHandler
 
 class LogTimeoutUploader:
     # Store relevent information/objects to carry out the timeout task
@@ -157,33 +206,44 @@
 uploader = LogTimeoutUploader(log_path)
 loglevel_timeout = CLPLogLevelTimeout(uploader.timeout)
 clp_handler = CLPSockHandler(log_path, create_listener=True, loglevel_timeout=loglevel_timeout)
 logging.getLogger(__name__).addHandler(clp_handler)
 ```
 
 ## Compatibility
+
 Tested on Python 3.6 and 3.8 and should work on any newer version.
 Built/packaged on Python 3.8 for convenience regarding type annotation.
 
 ## Building/Packaging
+
 1. Create and enter a virtual environment:
-    `python3.8 -m venv venv; . ./venv/bin/activate`
+   `python3.8 -m venv venv; . ./venv/bin/activate`
 2. Install development dependencies:
-    `pip install -r requirements-dev.txt`
+   `pip install -r requirements-dev.txt`
 3. Build:
-    `python -m build`
+   `python -m build`
 
 ## Testing
+
 Note the baseline comparison logging handler and the CLP handler both get
 unique timestamps. It is possible for these timestamps to differ, which will
 result in a test reporting a false positive error.
+
 1. Create and enter a virtual environment:
-    `python -m venv venv; .  ./venv/bin/activate`
-2. Install:
-    `pip install dist/clp_logging-*-py3-none-any.whl` or `pip install -e .`
-3. Run unittest:
-    `python -m unittest -bv`
+   `python -m venv venv; .  ./venv/bin/activate`
+2. Install development dependencies:
+   `pip install -r requirements-dev.txt`
+3. Install:
+   `pip install dist/clp_logging-*-py3-none-any.whl` or `pip install -e .`
+4. Run unittest:
+   `python -m unittest -bv`
 
 ## Contributing
+
 Ensure to run `mypy` and `black` (found in
 [requirements-dev.txt](requirements-dev.txt)) during development to ensure
 smooth pull requests.
+
+[0]: https://github.com/y-scope/clp
+[1]: https://www.uber.com/blog/reducing-logging-cost-by-two-orders-of-magnitude-using-clp/
+[2]: https://github.com/y-scope/yscope-log-viewer
```

### Comparing `clp_logging-0.0.8/src/clp_logging.egg-info/SOURCES.txt` & `clp_logging-0.0.9/src/clp_logging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clp_logging-0.0.8/tests/__init__.py` & `clp_logging-0.0.9/tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Iterable, Optional, Union
 
-from tests.test_handlers import TestCLPBase
+from tests.test_handlers import TestCLPBase, TestCLPSegmentStreamingBase
 import unittest
 
 
 def add_tests(suite: unittest.TestSuite, loader: unittest.TestLoader, test_class: type) -> None:
     """Recursively collect tests from concrete classes. Although TestCLPBase*
     classes are functionally abstract to the user we cannot properly make them
     abstract as `unittest` will still create instances of these classes.
@@ -25,8 +25,12 @@
     tests: Iterable[Union[unittest.TestCase, unittest.TestSuite]],
     pattern: Optional[str],
 ) -> unittest.TestSuite:
     suite: unittest.TestSuite = unittest.TestSuite()
 
     for test_class in TestCLPBase.__subclasses__():
         add_tests(suite, loader, test_class)
+
+    for test_class in TestCLPSegmentStreamingBase.__subclasses__():
+        add_tests(suite, loader, test_class)
+
     return suite
```

### Comparing `clp_logging-0.0.8/tests/test_handlers.py` & `clp_logging-0.0.9/tests/test_handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,54 @@
 import logging
 import os
 import time
 import unittest
 from datetime import datetime, timedelta, tzinfo
 from math import floor
 from multiprocessing.sharedctypes import Array, Value, Synchronized, SynchronizedArray
+from smart_open import open, register_compressor
 from pathlib import Path
 from typing import cast, ClassVar, Dict, IO, List, Optional
+from zstandard import ZstdCompressor, ZstdDecompressor
 
 import dateutil.parser
 
 from clp_logging.handlers import (
     CLPBaseHandler,
     CLPFileHandler,
     CLPLogLevelTimeout,
     CLPSockHandler,
     CLPStreamHandler,
     DEFAULT_LOG_FORMAT,
     WARN_PREFIX,
 )
+from clp_logging.protocol import Metadata
 from clp_logging.readers import CLPFileReader
+from clp_logging.readers import CLPSegmentStreaming
+
+
+def _zstd_comppressions_handler(file_obj, mode):
+    if "wb" == mode:
+        cctx = ZstdCompressor()
+        return cctx.stream_writer(file_obj)
+    elif "rb" == mode:
+        dctx = ZstdDecompressor()
+        return dctx.stream_reader(file_obj)
+    else:
+        raise RuntimeError(f"Zstd handler: Unexpected Mode {mode}")
+
+
+# Register .zst with zstandard library compressor
+register_compressor(".zst", _zstd_comppressions_handler)
 
 LOG_DIR: Path = Path("unittest-logs")
 
 
-class DtStreamHandler(logging.StreamHandler):
+# TODO: revisit type ignore if minimum python version increased
+class DtStreamHandler(logging.StreamHandler):  # type: ignore
     """
     `logging` handler using `datetime` for the timestamp rather than `time`
     (used internally by `logging`). Necessary for correct comparison with CLP
     log handlers.
     """
 
     def __init__(self, stream: IO[str]) -> None:
@@ -61,39 +81,42 @@
 class TestCLPBase(unittest.TestCase):
     """
     Functionally abstract as we use `load_tests` to avoid adding
     `TestCLPBase` itself to the test suite. This allows us to share tests
     between different handlers.
     However, we cannot mark it as abstract as `unittest` will still `__init__`
     an instance before `load_tests` is run (and will error out if any method
-    is marked abstract)
+    is marked abstract).
+    Non-base classes have shortened names to avoid errors with socket name
+    length.
     """
 
-    clp_handler: logging.Handler
+    clp_handler: CLPBaseHandler
     raw_log_path: Path
     clp_log_path: Path
+    enable_compression: bool
 
     # override
     @classmethod
     def setUpClass(cls) -> None:
         if not LOG_DIR.exists():
             LOG_DIR.mkdir(parents=True, exist_ok=True)
         assert LOG_DIR.is_dir()
 
     # override
     def setUp(self) -> None:
         self.raw_log_path: Path = LOG_DIR / Path(f"{self.id()}.log")
-        self.clp_log_path: Path = LOG_DIR / Path(f"{self.id()}.clp.zst")
+        self.clp_log_path: Path = LOG_DIR / Path(f"{self.id()}.clp")
         if self.raw_log_path.exists():
             self.raw_log_path.unlink()
         if self.clp_log_path.exists():
             self.clp_log_path.unlink()
 
     def read_clp(self) -> List[str]:
-        with CLPFileReader(self.clp_log_path) as logf:
+        with CLPFileReader(self.clp_log_path, enable_compression=self.enable_compression) as logf:
             return [log.formatted_msg for log in logf]
 
     def read_raw(self) -> List[str]:
         with open(self.raw_log_path, "r") as logf:
             return logf.readlines()
 
     def setup_logging(self) -> None:
@@ -132,15 +155,15 @@
             # must be the same
             if test_time:
                 clp_time_str: str = " ".join(clp_log_split[0:2])
                 raw_time_str: str = " ".join(raw_log_split[0:2])
                 clp_timestamp: datetime = dateutil.parser.isoparse(clp_time_str)
                 raw_timestamp: datetime = dateutil.parser.isoparse(raw_time_str)
                 self.assertAlmostEqual(
-                    clp_timestamp, raw_timestamp, delta=timedelta(milliseconds=8)
+                    clp_timestamp, raw_timestamp, delta=timedelta(milliseconds=32)
                 )
 
             clp_msg: str = " ".join(clp_log_split[2:])
             raw_msg: str = " ".join(raw_log_split[2:])
             msg: Optional[str] = None
             if size_msg:
                 msg = f"len(clp_msg): {len(clp_msg)}, len(raw_msg): {len(raw_msg)}"
@@ -301,15 +324,15 @@
         # TODO: when the issue is closed we should update the typing here
         timeout_ts: SynchronizedArray[c_double] = Array(c_double, [0.0] * expected_timeout_count)
         timeout_count: Synchronized[int] = cast("Synchronized[int]", Value(c_int, 0))
 
         def timeout_fn() -> None:
             nonlocal timeout_ts
             nonlocal timeout_count
-            timeout_ts[timeout_count.value] = time.time()
+            timeout_ts[timeout_count.value] = c_double(time.time())
             timeout_count.value += 1
 
         self.loglevel_timeout = CLPLogLevelTimeout(timeout_fn, hard_deltas, soft_deltas)
         self._setup_handler()
 
         start_ts: float = time.time()
         for i, loglevel in enumerate(loglevels):
@@ -322,17 +345,17 @@
 
         self.logger.log(logging.INFO, f"ensure close flushes correctly")
 
         self.compare_all_logs()
         self.assertEqual(timeout_count.value, expected_timeout_count)
         for i in range(expected_timeout_count):
             self.assertAlmostEqual(
-                datetime.fromtimestamp(timeout_ts[i]),
+                datetime.fromtimestamp(timeout_ts[i]),  # type: ignore
                 datetime.fromtimestamp(start_ts + expected_timeout_deltas[i]),
-                delta=timedelta(milliseconds=128),
+                delta=timedelta(milliseconds=64),
             )
 
     def test_pushback_soft_timeout(self) -> None:
         delta_ms: int = 400
         delta_s: float = delta_ms / 1000
         self._test_timeout(
             loglevels=[logging.INFO, logging.INFO, logging.INFO],
@@ -340,15 +363,15 @@
             hard_deltas={logging.INFO: 30 * 60 * 1000},
             soft_deltas={logging.INFO: delta_ms},
             # delay < soft delta, so timeout push back should occur
             # timeout = final log occurrence + soft delta
             expected_timeout_count=2,
             expected_timeout_deltas=[
                 (0.2 * 2) + delta_s,  # 2 logs * delay + soft delta
-                (0.2 * 2) + delta_s + 1,  # last timeout + 1 second pad
+                (0.2 * 2) + delta_s + 0.256,  # last timeout + 256ms pad
             ],
         )
 
     def test_multiple_soft_timeout(self) -> None:
         delta_ms: int = 100
         delta_s: float = delta_ms / 1000
         self._test_timeout(
@@ -357,16 +380,16 @@
             hard_deltas={logging.INFO: 30 * 60 * 1000},
             soft_deltas={logging.INFO: delta_ms},
             # delay > soft delta, so every log will timeout
             expected_timeout_count=4,
             expected_timeout_deltas=[
                 delta_s,  # soft delta
                 0.2 + delta_s,  # delay + soft delta
-                0.2 * 2 + delta_s,  # 2 * delay + soft delta
-                0.2 * 2 + delta_s + 1,  # last timeout + 1 second pad
+                (0.2 * 2) + delta_s,  # 2 * delay + soft delta
+                (0.2 * 2) + delta_s + 0.256,  # last timeout + 256ms pad
             ],
         )
 
     def test_hard_timeout(self) -> None:
         delta_ms: int = 700
         delta_s: float = delta_ms / 1000
         self._test_timeout(
@@ -375,58 +398,91 @@
             hard_deltas={logging.INFO: delta_ms},
             soft_deltas={logging.INFO: 3 * 60 * 1000},
             # delay < soft delta, so timeout push back should occur
             # timeout = final log occurrence + soft delta
             expected_timeout_count=2,
             expected_timeout_deltas=[
                 delta_s,  # hard delta
-                delta_s + 1,  # last timeout + 1 second pad
+                delta_s + 0.256,  # last timeout + 256ms pad
+            ],
+        )
+
+    def test_end_timeout(self) -> None:
+        self._test_timeout(
+            loglevels=[logging.INFO, logging.INFO, logging.INFO],
+            delay=0.2,
+            hard_deltas={logging.INFO: 30 * 60 * 1000},
+            soft_deltas={logging.INFO: 3 * 60 * 1000},
+            # no deltas occur
+            # timeout = when close is called roughly after last log
+            expected_timeout_count=1,
+            expected_timeout_deltas=[
+                (0.2 * 3) + 0.256,  # last log delay + 256ms pad
             ],
         )
 
 
-class TestCLPSockHandler(TestCLPHandlerBase):
+class TestCLPSockHandlerBase(TestCLPHandlerBase):
     # override
     def setUp(self) -> None:
         super().setUp()
         self.sock_path: Path = self.clp_log_path.with_suffix(".sock")
         if self.sock_path.exists():
             self.sock_path.unlink()
 
         self.clp_handler: CLPSockHandler
         try:
-            self.clp_handler = CLPSockHandler(self.clp_log_path, create_listener=True)
+            self.clp_handler = CLPSockHandler(
+                self.clp_log_path, create_listener=True, enable_compression=self.enable_compression
+            )
         except SystemExit as e:
             self.assertEqual(e.code, 0)
             # hack to exit the forked listener process without being caught and
             # reported by unittest
             os._exit(0)
         self.setup_logging()
 
     # override
     def close(self) -> None:
         self.clp_handler.stop_listener()
         os.waitpid(self.clp_handler.listener_pid, 0)
         super().close()
 
 
-class TestCLPSockHandlerLogLevelTimeout(TestCLPLogLevelTimeoutBase):
+class TestCLPSock_ZSTD(TestCLPSockHandlerBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = True
+        super().setUp()
+
+
+class TestCLPSock_RAW(TestCLPSockHandlerBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = False
+        super().setUp()
+
+
+class TestCLPSockHandlerLogLevelTimeoutBase(TestCLPLogLevelTimeoutBase):
     # override
     def setUp(self) -> None:
         TestCLPLogLevelTimeoutBase.setUp(self)
         self.sock_path: Path = self.clp_log_path.with_suffix(".sock")
         if self.sock_path.exists():
             self.sock_path.unlink()
 
     # override
     def _setup_handler(self) -> None:
         self.clp_handler: CLPSockHandler
         try:
             self.clp_handler = CLPSockHandler(
-                self.clp_log_path, create_listener=True, loglevel_timeout=self.loglevel_timeout
+                self.clp_log_path,
+                create_listener=True,
+                loglevel_timeout=self.loglevel_timeout,
+                enable_compression=self.enable_compression,
             )
         except SystemExit as e:
             self.assertEqual(e.code, 0)
             # hack to exit the forked listener process without being caught and
             # reported by unittest
             os._exit(0)
         self.setup_logging()
@@ -434,26 +490,203 @@
     # override
     def close(self) -> None:
         self.clp_handler.stop_listener()
         os.waitpid(self.clp_handler.listener_pid, 0)
         super().close()
 
 
-class TestCLPStreamHandler(TestCLPHandlerBase):
+class TestCLPSock_LLT(TestCLPSockHandlerLogLevelTimeoutBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = True
+        super().setUp()
+
+
+class TestCLPSock_LLT_RAW(TestCLPSockHandlerLogLevelTimeoutBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = False
+        super().setUp()
+
+
+class TestCLPStream_ZSTD(TestCLPHandlerBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = True
+        super().setUp()
+        self.clp_handler: CLPStreamHandler = CLPFileHandler(
+            self.clp_log_path, enable_compression=True
+        )
+        self.setup_logging()
+
+
+class TestCLPStream_RAW(TestCLPHandlerBase):
     # override
     def setUp(self) -> None:
+        self.enable_compression = False
         super().setUp()
-        self.clp_handler: CLPStreamHandler = CLPFileHandler(self.clp_log_path)
+        self.clp_handler: CLPStreamHandler = CLPFileHandler(
+            self.clp_log_path, enable_compression=False
+        )
         self.setup_logging()
 
 
-class TestCLPStreamHandlerLogLevelTimeout(TestCLPLogLevelTimeoutBase):
+class TestCLPStream_LLT_ZSTD(TestCLPLogLevelTimeoutBase):
     # override
     def _setup_handler(self) -> None:
+        self.enable_compression = True
         self.clp_handler = CLPFileHandler(
-            self.clp_log_path, loglevel_timeout=self.loglevel_timeout
+            self.clp_log_path, loglevel_timeout=self.loglevel_timeout, enable_compression=True
         )
         self.setup_logging()
 
 
+class TestCLPStream_LLT_RAW(TestCLPLogLevelTimeoutBase):
+    # override
+    def _setup_handler(self) -> None:
+        self.enable_compression = False
+        self.clp_handler = CLPFileHandler(
+            self.clp_log_path, loglevel_timeout=self.loglevel_timeout, enable_compression=False
+        )
+        self.setup_logging()
+
+
+class TestCLPSegmentStreamingBase(unittest.TestCase):
+    """
+    Similar to `TestCLPBase`. Functionally abstract as we use `load_tests` to
+    avoid adding `TestCLPSegmentStreamingBase` itself to the test suite. This
+    allows us to share tests between different settings when test against
+    IR segment streaming.
+    """
+
+    clp_handler: CLPBaseHandler
+    clp_log_path: Path
+    segment_path_list: List[Path]
+    segment_idx: int
+    logger: logging.Logger
+    # Configurable:
+    enable_compression: bool
+    segment_size: int
+
+    # override
+    @classmethod
+    def setUpClass(cls) -> None:
+        if not LOG_DIR.exists():
+            LOG_DIR.mkdir(parents=True, exist_ok=True)
+        assert LOG_DIR.is_dir()
+
+    # override
+    def setUp(self) -> None:
+        if self.enable_compression:
+            self.clp_log_path: Path = LOG_DIR / Path(f"{self.id()}.clp.zst")
+        else:
+            self.clp_log_path: Path = LOG_DIR / Path(f"{self.id()}.clp")
+        if self.clp_log_path.exists():
+            self.clp_log_path.unlink()
+        self.segment_path_list: List[Path] = []
+        self.segment_idx = 0
+
+    def generate_segments(self) -> None:
+        meta: Metadata = None
+        offset: int = 0
+        while True:
+            segment_path: Path
+            if self.enable_compression:
+                segment_path: Path = LOG_DIR / Path(f"{self.id()}_seg_{self.segment_idx}.clp.zst")
+            else:
+                segment_path: Path = LOG_DIR / Path(f"{self.id()}_seg_{self.segment_idx}.clp")
+            if segment_path.exists():
+                segment_path.unlink()
+            bytes_read: int
+            with open(self.clp_log_path, "rb") as fin, open(segment_path, "wb") as fout:
+                bytes_read, meta = CLPSegmentStreaming.read(
+                    fin, fout, offset=offset, max_bytes_to_write=self.segment_size, metadata=meta
+                )
+                offset += bytes_read
+                self.segment_idx += 1
+            self.segment_path_list.append(segment_path)
+            if meta == None or bytes_read == 0:
+                break
+
+    def close(self) -> None:
+        logging.shutdown()
+        self.logger.removeHandler(self.clp_handler)
+
+    def read_clp(self) -> List[str]:
+        with CLPFileReader(self.clp_log_path, enable_compression=self.enable_compression) as logf:
+            return [log.formatted_msg for log in logf]
+
+    def read_segments(self) -> List[str]:
+        logs: List[str] = []
+        for segment_path in self.segment_path_list:
+            with CLPFileReader(segment_path, enable_compression=self.enable_compression) as logf:
+                logs.extend([log.formatted_msg for log in logf])
+        return logs
+
+    def compare_all_logs(self) -> None:
+        self.close()
+        self.generate_segments()
+        clp_logs: List[str] = self.read_clp()
+        segment_logs: List[str] = self.read_segments()
+        self.compare_logs(clp_logs, segment_logs)
+
+    def compare_logs(self, clp_logs: List[str], segment_logs: List[str]):
+        self.assertEqual(len(clp_logs), len(segment_logs))
+        for clp_log, segment_log in zip(clp_logs, segment_logs):
+            self.assertEqual(clp_log, segment_log)
+
+    def setup_logging(self) -> None:
+        self.clp_handler: CLPStreamHandler = CLPFileHandler(
+            self.clp_log_path, enable_compression=self.enable_compression
+        )
+        self.logger: logging.Logger = logging.getLogger(self.id())
+        self.logger.setLevel(logging.DEBUG)
+        self.clp_handler.setFormatter(logging.Formatter("[%(levelname)s] %(message)s"))
+        self.logger.addHandler(self.clp_handler)
+
+    def test_log(self) -> None:
+        for i in range(100):
+            self.logger.info(f"Log message #{i}")
+            # Static log
+            self.logger.info("static text log one")
+            self.logger.info("static text log two")
+            # Int
+            self.logger.info("int 3190")
+            self.logger.info("-int -3190")
+            # Float
+            self.logger.info("float 31.90")
+            self.logger.info("-float -31.90")
+            # Dict
+            self.logger.info("textint test1234")
+            self.logger.info("texteq=var")
+            self.logger.info(f">32bit int: {2**32}")
+            # Combo
+            self.logger.info("zxcvbn 1234 asdfgh 12.34 qwerty")
+            self.logger.info("zxcvbn -1234 asdfgh -12.34 qwerty")
+            self.logger.info("zxcvbn foo=bar asdfgh foobar=var321 qwerty")
+            # Level
+            self.logger.debug("zxcvbn 1234 asdfgh 12.34 qwerty")
+            self.logger.debug("zxcvbn -1234 asdfgh -12.34 qwerty")
+            self.logger.debug("zxcvbn foo=bar asdfgh foobar=var321 qwerty")
+        self.compare_all_logs()
+
+
+class TestCLPSegmentStreaming_ZSTD(TestCLPSegmentStreamingBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = True
+        self.segment_size = 4096
+        super().setUp()
+        self.setup_logging()
+
+
+class TestCLPSegmentStreaming_RAW(TestCLPSegmentStreamingBase):
+    # override
+    def setUp(self) -> None:
+        self.enable_compression = False
+        self.segment_size = 4096
+        super().setUp()
+        self.setup_logging()
+
+
 if __name__ == "__main__":
     unittest.main()
```

