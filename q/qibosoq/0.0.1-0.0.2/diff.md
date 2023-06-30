# Comparing `tmp/qibosoq-0.0.1.tar.gz` & `tmp/qibosoq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibosoq-0.0.1.tar", max compression
+gzip compressed data, was "qibosoq-0.0.2.tar", max compression
```

## Comparing `qibosoq-0.0.1.tar` & `qibosoq-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-06-02 08:41:39.471066 qibosoq-0.0.1/LICENSE
--rw-r--r--   0        0        0     2255 2023-06-26 16:12:12.722584 qibosoq-0.0.1/README.md
--rw-r--r--   0        0        0     1540 2023-06-26 16:12:23.086651 qibosoq-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       94 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/__init__.py
--rw-r--r--   0        0        0      428 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/__main__.py
--rw-r--r--   0        0        0     3045 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/components.py
--rw-r--r--   0        0        0     1021 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/configuration.py
--rw-r--r--   0        0        0     1063 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/log.py
--rw-r--r--   0        0        0       23 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/programs/__init__.py
--rw-r--r--   0        0        0    13649 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/programs/base.py
--rw-r--r--   0        0        0     2932 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/programs/flux.py
--rw-r--r--   0        0        0      917 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/programs/pulse_sequence.py
--rw-r--r--   0        0        0     5124 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/programs/sweepers.py
--rw-r--r--   0        0        0     4377 2023-06-26 15:24:51.618464 qibosoq-0.0.1/src/qibosoq/rfsoc_server.py
--rw-r--r--   0        0        0     3073 1970-01-01 00:00:00.000000 qibosoq-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-30 10:59:10.736272 qibosoq-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2363 2023-06-30 10:59:10.736272 qibosoq-0.0.2/README.md
+-rw-r--r--   0        0        0     1547 2023-06-30 10:59:10.740272 qibosoq-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       94 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/__init__.py
+-rw-r--r--   0        0        0      428 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/__main__.py
+-rw-r--r--   0        0        0       22 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/__init__.py
+-rw-r--r--   0        0        0     2176 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/base.py
+-rw-r--r--   0        0        0     1388 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/components/pulses.py
+-rw-r--r--   0        0        0     1021 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/configuration.py
+-rw-r--r--   0        0        0     1063 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/log.py
+-rw-r--r--   0        0        0       23 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/__init__.py
+-rw-r--r--   0        0        0    13726 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/base.py
+-rw-r--r--   0        0        0     2974 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/flux.py
+-rw-r--r--   0        0        0      917 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/pulse_sequence.py
+-rw-r--r--   0        0        0     5166 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/programs/sweepers.py
+-rw-r--r--   0        0        0     4782 2023-06-30 10:59:10.740272 qibosoq-0.0.2/src/qibosoq/rfsoc_server.py
+-rw-r--r--   0        0        0     3181 1970-01-01 00:00:00.000000 qibosoq-0.0.2/PKG-INFO
```

### Comparing `qibosoq-0.0.1/LICENSE` & `qibosoq-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.1/README.md` & `qibosoq-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # Qibosoq
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/zenodo.8083286)
+
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
 The complete documentation can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-# Qibosoq Repository for developing server side of RFSoC fpga boards Qibosoq is
-a server for integrating [Qick](https://github.com/openquantumhardware/qick) in
-the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem for executing
-arbitrary pulses sequences on QPUs. The complete documentation can be found at
-[qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/) ##
-Installation The package can be installed by source: ```sh git clone https://
-github.com/qiboteam/qibosoq.git cd qibosoq pip install . ``` ### Developer
-instructions For development make sure to install the package using [`poetry`]
-(https://python-poetry.org/) and to install the pre-commit hooks: ```sh git
-clone https://github.com/qiboteam/qibosoq.git cd qibosoq poetry install pre-
-commit install ``` ## Configuration parameters In `configuration.py` some
-default qibosoq parameters are hardcoded. They can be changed using environment
-variables ([see documentation](https://qibo.science/qibosoq/stable/getting-
-started/usage.html)). * IP of the server * Port of the server * Paths of log
-files * Name of python loggers * Path of bitstream * Type of readout
-(multiplexed or not, depending on the loaded bitstream) ## Run the server The
-simplest way of executing the server is: ``` sudo -E python -m qibosoq ``` and
-the server can be closed with `Ctrl-C`.\ Note that with this command the script
-will close as soon as the terminal where it's running it's closed. To run the
-server in detached mode you can use: ``` nohup sudo -E python -m qibosoq & ```
-And the server can be closed with `sudo kill ` (PID will be saved in log). ###
-TII boards With TII boards the server can also be executed using the alias
-`server-run-bkg`. Also, two additional command are added in `.bashrc`:
-`serverinfo` and `serverclose`. `serverinfo` will print the PID if the server
-is running, otherwise will print "No running server". `serverclose` will close
-the server, if it is running. All these commands require sudo privileges. ##
-Contributing Contributions, issues and feature requests are welcome! Feel free
-to check [GitHub_issues]
+# Qibosoq [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)]
+(https://doi.org/10.5281/zenodo.8083286) Repository for developing server side
+of RFSoC fpga boards Qibosoq is a server for integrating [Qick](https://
+github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/
+qiboteam/qibolab) ecosystem for executing arbitrary pulses sequences on QPUs.
+The complete documentation can be found at [qibo.science/qibosoq/stable](https:
+//qibo.science/qibosoq/stable/) ## Installation The package can be installed by
+source: ```sh git clone https://github.com/qiboteam/qibosoq.git cd qibosoq pip
+install . ``` ### Developer instructions For development make sure to install
+the package using [`poetry`](https://python-poetry.org/) and to install the
+pre-commit hooks: ```sh git clone https://github.com/qiboteam/qibosoq.git cd
+qibosoq poetry install pre-commit install ``` ## Configuration parameters In
+`configuration.py` some default qibosoq parameters are hardcoded. They can be
+changed using environment variables ([see documentation](https://qibo.science/
+qibosoq/stable/getting-started/usage.html)). * IP of the server * Port of the
+server * Paths of log files * Name of python loggers * Path of bitstream * Type
+of readout (multiplexed or not, depending on the loaded bitstream) ## Run the
+server The simplest way of executing the server is: ``` sudo -E python -
+m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note that with this
+command the script will close as soon as the terminal where it's running it's
+closed. To run the server in detached mode you can use: ``` nohup sudo -
+E python -m qibosoq & ``` And the server can be closed with `sudo kill ` (PID
+will be saved in log). ### TII boards With TII boards the server can also be
+executed using the alias `server-run-bkg`. Also, two additional command are
+added in `.bashrc`: `serverinfo` and `serverclose`. `serverinfo` will print the
+PID if the server is running, otherwise will print "No running server".
+`serverclose` will close the server, if it is running. All these commands
+require sudo privileges. ## Contributing Contributions, issues and feature
+requests are welcome! Feel free to check [GitHub_issues]
```

### Comparing `qibosoq-0.0.1/pyproject.toml` & `qibosoq-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 [tool.poetry]
 name = "qibosoq"
-version = "0.0.1"
+version = "0.0.2"
 description = "QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards"
-authors = ["Rodolfo Carobene <rodolfo.carobene@gmail.com>", "Javier Serrano <javier.serrano@tii.ae>"]
+authors = [
+  "Rodolfo Carobene <rodolfo.carobene@gmail.com>",
+  "Javier Serrano <javier.serrano@tii.ae>",
+]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/qiboteam/qibosoq/"
 documentation = ""
 keywords = []
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `qibosoq-0.0.1/src/qibosoq/components.py` & `qibosoq-0.0.2/src/qibosoq/components/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Various helper objects."""
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from enum import Enum, IntEnum, auto
 from typing import Iterable, List, Union, overload
 
 
 @dataclass
 class Config:
     """General RFSoC Configuration."""
@@ -33,47 +33,14 @@
 
     bias: float = 0.0
     """Amplitude factor, for sweetspot."""
     dac: int = None
     """DAC responsible for flux control."""
 
 
-@dataclass
-class Pulse:
-    """Abstract Pulse object."""
-
-    frequency: float
-    """Freuency of the pulse (MHz)."""
-    amplitude: float
-    """Amplitude factor, multiplied by maximum gain of the DAC."""
-    relative_phase: int
-    """Relative phase (degrees)."""
-    start: float = field(compare=False)
-    """Start time (us)."""
-    duration: float
-    """Duration of the pulse (us)."""
-
-    name: str
-    """Name of the pulse, typically a serial."""
-    type: str
-    """Can be 'readout', 'drive', 'flux'."""
-
-    dac: int
-    """DAC responsible for firing the pulse."""
-    adc: int
-    """ADC to acquire pulse back, for readout pulses."""
-
-    shape: str
-    """Can be 'rectangular', 'gaussian', 'drag'."""
-    rel_sigma: float = None
-    """Sigma for gaussians and drags, fraction of duration."""
-    beta: float = None
-    """Beta for drag pulses."""
-
-
 class Parameter(str, Enum):
     """Available parameters for sweepers."""
 
     FREQUENCY = "freq"
     AMPLITUDE = "gain"
     RELATIVE_PHASE = "phase"
     START = "t"
```

### Comparing `qibosoq-0.0.1/src/qibosoq/configuration.py` & `qibosoq-0.0.2/src/qibosoq/configuration.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.1/src/qibosoq/log.py` & `qibosoq-0.0.2/src/qibosoq/log.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.1/src/qibosoq/programs/base.py` & `qibosoq-0.0.2/src/qibosoq/programs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import List, Tuple
 
 import numpy as np
 import numpy.typing as npt
 from qick import QickProgram, QickSoc
 
 import qibosoq.configuration as qibosoq_cfg
-from qibosoq.components import Config, Pulse, Qubit
+from qibosoq.components.base import Config, Qubit
+from qibosoq.components.pulses import Drag, Gaussian, Pulse, Rectangular
 
 logger = logging.getLogger(qibosoq_cfg.MAIN_LOGGER_NAME)
 
 
 class BaseProgram(ABC, QickProgram):
     """Abstract class for QickPrograms."""
 
@@ -102,17 +103,17 @@
         gain = int(pulse.amplitude * max_gain)
         phase = self.deg2reg(pulse.relative_phase, gen_ch=gen_ch)
 
         # pulse length converted with DAC CLK
         us_length = pulse.duration
         soc_length = self.soc.us2cycles(us_length, gen_ch=gen_ch)
 
-        is_drag = pulse.shape == "drag"
-        is_gaus = pulse.shape == "gaussian"
-        is_rect = pulse.shape == "rectangular"
+        is_drag = isinstance(pulse, Drag)
+        is_gaus = isinstance(pulse, Gaussian)
+        is_rect = isinstance(pulse, Rectangular)
 
         # pulse freq converted with frequency matching
         freq = self.soc.freq2reg(pulse.frequency, gen_ch=gen_ch, ro_ch=pulse.adc)
 
         # if pulse is drag or gauss first define the i-q shape and then set reg
         if is_drag or is_gaus:
             name = pulse.name
```

### Comparing `qibosoq-0.0.1/src/qibosoq/programs/flux.py` & `qibosoq-0.0.2/src/qibosoq/programs/flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import logging
 from typing import List
 
 import numpy as np
 from qick import QickSoc
 
 import qibosoq.configuration as qibosoq_cfg
-from qibosoq.components import Config, Pulse, Qubit
+from qibosoq.components.base import Config, Qubit
+from qibosoq.components.pulses import Pulse
 from qibosoq.programs.base import BaseProgram
 
 logger = logging.getLogger(qibosoq_cfg.MAIN_LOGGER_NAME)
 
 
 class FluxProgram(BaseProgram):
     """Abstract class for flux-tunable qubits programs."""
```

### Comparing `qibosoq-0.0.1/src/qibosoq/programs/pulse_sequence.py` & `qibosoq-0.0.2/src/qibosoq/programs/pulse_sequence.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.0.1/src/qibosoq/programs/sweepers.py` & `qibosoq-0.0.2/src/qibosoq/programs/sweepers.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from typing import Iterable, List, Tuple, Union
 
 import numpy as np
 from qick import NDAveragerProgram, QickSoc
 from qick.averager_program import QickSweep, merge_sweeps
 
 import qibosoq.configuration as qibosoq_cfg
-from qibosoq.components import Config, Parameter, Pulse, Qubit, Sweeper
+from qibosoq.components.base import Config, Parameter, Qubit, Sweeper
+from qibosoq.components.pulses import Pulse
 from qibosoq.programs.flux import FluxProgram
 
 logger = logging.getLogger(qibosoq_cfg.MAIN_LOGGER_NAME)
 
 
 def reversed_sweepers(sweepers: Union[Sweeper, Iterable[Sweeper]]) -> List[Sweeper]:
     """Ensure that sweepers is a list and reverse it.
```

### Comparing `qibosoq-0.0.1/src/qibosoq/rfsoc_server.py` & `qibosoq-0.0.2/src/qibosoq/rfsoc_server.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,26 +7,38 @@
 
 import json
 import logging
 import os
 import socket
 import traceback
 from socketserver import BaseRequestHandler, TCPServer
+from typing import Dict, List
 
 from qick import QickSoc
 
 import qibosoq.configuration as cfg
-from qibosoq.components import Config, OperationCode, Pulse, Qubit, Sweeper
+from qibosoq.components.base import Config, OperationCode, Qubit, Sweeper
+from qibosoq.components.pulses import Pulse, Shape
 from qibosoq.programs.pulse_sequence import ExecutePulseSequence
 from qibosoq.programs.sweepers import ExecuteSweeps
 
 logger = logging.getLogger(cfg.MAIN_LOGGER_NAME)
 qick_logger = logging.getLogger(cfg.PROGRAM_LOGGER_NAME)
 
 
+def load_pulses(list_sequence: List[Dict]) -> List[Pulse]:
+    """Convert a list of pulses (in dict form) to a list of Pulse objects."""
+    obj_sequence = []
+    for pulse in list_sequence:
+        cls = Shape[pulse["shape"]].value
+        converted_pulse = cls(**pulse)
+        obj_sequence.append(converted_pulse)
+    return obj_sequence
+
+
 def execute_program(data: dict, qick_soc: QickSoc) -> dict:
     """Create and execute qick programs.
 
     Returns:
         (dict): dictionary with two keys (i, q) to lists of values
     """
     opcode = OperationCode(data["operation_code"])
@@ -42,15 +54,15 @@
         args = tuple(Sweeper(**sweeper) for sweeper in data["sweepers"])
     else:
         raise NotImplementedError(f"Operation code {data['operation_code']} not supported")
 
     program = programcls(
         qick_soc,
         Config(**data["cfg"]),
-        [Pulse(**pulse) for pulse in data["sequence"]],
+        load_pulses(data["sequence"]),
         [Qubit(**qubit) for qubit in data["qubits"]],
         *args,
     )
 
     asm_prog = program.asm()
     qick_logger.handlers[0].doRollover()
     qick_logger.info(asm_prog)
```

### Comparing `qibosoq-0.0.1/PKG-INFO` & `qibosoq-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibosoq
-Version: 0.0.1
+Version: 0.0.2
 Summary: QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards
 Home-page: https://github.com/qiboteam/qibosoq/
 License: Apache-2.0
 Author: Rodolfo Carobene
 Author-email: rodolfo.carobene@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,14 +15,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: qick (==0.2.135)
 Project-URL: Repository, https://github.com/qiboteam/qibosoq/
 Description-Content-Type: text/markdown
 
 # Qibosoq
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/zenodo.8083286)
+
 Repository for developing server side of RFSoC fpga boards
 Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
 for executing arbitrary pulses sequences on QPUs.
 
 The complete documentation can be found at [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
 
 ## Installation
```

#### html2text {}

```diff
@@ -1,38 +1,40 @@
-Metadata-Version: 2.1 Name: qibosoq Version: 0.0.1 Summary: QIBO Server On Qick
+Metadata-Version: 2.1 Name: qibosoq Version: 0.0.2 Summary: QIBO Server On Qick
 (qibosoq) is the server component of qibolab to be run on RFSoC boards Home-
 page: https://github.com/qiboteam/qibosoq/ License: Apache-2.0 Author: Rodolfo
 Carobene Author-email: rodolfo.carobene@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Physics Requires-
 Dist: qick (==0.2.135) Project-URL: Repository, https://github.com/qiboteam/
-qibosoq/ Description-Content-Type: text/markdown # Qibosoq Repository for
-developing server side of RFSoC fpga boards Qibosoq is a server for integrating
-[Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://
-github.com/qiboteam/qibolab) ecosystem for executing arbitrary pulses sequences
-on QPUs. The complete documentation can be found at [qibo.science/qibosoq/
-stable](https://qibo.science/qibosoq/stable/) ## Installation The package can
-be installed by source: ```sh git clone https://github.com/qiboteam/qibosoq.git
-cd qibosoq pip install . ``` ### Developer instructions For development make
-sure to install the package using [`poetry`](https://python-poetry.org/) and to
-install the pre-commit hooks: ```sh git clone https://github.com/qiboteam/
-qibosoq.git cd qibosoq poetry install pre-commit install ``` ## Configuration
-parameters In `configuration.py` some default qibosoq parameters are hardcoded.
-They can be changed using environment variables ([see documentation](https://
-qibo.science/qibosoq/stable/getting-started/usage.html)). * IP of the server *
-Port of the server * Paths of log files * Name of python loggers * Path of
-bitstream * Type of readout (multiplexed or not, depending on the loaded
-bitstream) ## Run the server The simplest way of executing the server is: ```
-sudo -E python -m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note
-that with this command the script will close as soon as the terminal where it's
-running it's closed. To run the server in detached mode you can use: ``` nohup
-sudo -E python -m qibosoq & ``` And the server can be closed with `sudo kill `
-(PID will be saved in log). ### TII boards With TII boards the server can also
-be executed using the alias `server-run-bkg`. Also, two additional command are
+qibosoq/ Description-Content-Type: text/markdown # Qibosoq [![DOI](https://
+zenodo.org/badge/DOI/10.5281/zenodo.8083286.svg)](https://doi.org/10.5281/
+zenodo.8083286) Repository for developing server side of RFSoC fpga boards
+Qibosoq is a server for integrating [Qick](https://github.com/
+openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab)
+ecosystem for executing arbitrary pulses sequences on QPUs. The complete
+documentation can be found at [qibo.science/qibosoq/stable](https://
+qibo.science/qibosoq/stable/) ## Installation The package can be installed by
+source: ```sh git clone https://github.com/qiboteam/qibosoq.git cd qibosoq pip
+install . ``` ### Developer instructions For development make sure to install
+the package using [`poetry`](https://python-poetry.org/) and to install the
+pre-commit hooks: ```sh git clone https://github.com/qiboteam/qibosoq.git cd
+qibosoq poetry install pre-commit install ``` ## Configuration parameters In
+`configuration.py` some default qibosoq parameters are hardcoded. They can be
+changed using environment variables ([see documentation](https://qibo.science/
+qibosoq/stable/getting-started/usage.html)). * IP of the server * Port of the
+server * Paths of log files * Name of python loggers * Path of bitstream * Type
+of readout (multiplexed or not, depending on the loaded bitstream) ## Run the
+server The simplest way of executing the server is: ``` sudo -E python -
+m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note that with this
+command the script will close as soon as the terminal where it's running it's
+closed. To run the server in detached mode you can use: ``` nohup sudo -
+E python -m qibosoq & ``` And the server can be closed with `sudo kill ` (PID
+will be saved in log). ### TII boards With TII boards the server can also be
+executed using the alias `server-run-bkg`. Also, two additional command are
 added in `.bashrc`: `serverinfo` and `serverclose`. `serverinfo` will print the
 PID if the server is running, otherwise will print "No running server".
 `serverclose` will close the server, if it is running. All these commands
 require sudo privileges. ## Contributing Contributions, issues and feature
 requests are welcome! Feel free to check [GitHub_issues]
```

