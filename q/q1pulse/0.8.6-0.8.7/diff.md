# Comparing `tmp/q1pulse-0.8.6.tar.gz` & `tmp/q1pulse-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1pulse-0.8.6.tar", last modified: Fri Jun 30 11:35:49 2023, max compression
+gzip compressed data, was "dist\q1pulse-0.8.7.tar", last modified: Fri Jun 30 12:43:52 2023, max compression
```

## Comparing `q1pulse-0.8.6.tar` & `q1pulse-0.8.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/
--rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.6/LICENSE
--rw-rw-rw-   0        0        0      193 2023-06-30 11:35:49.000000 q1pulse-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/
--rw-rw-rw-   0        0        0      139 2023-06-30 11:35:13.000000 q1pulse-0.8.6/q1pulse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/assembler/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/assembler/__init__.py
--rw-rw-rw-   0        0        0    28695 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/assembler/generator.py
--rw-rw-rw-   0        0        0     1813 2021-12-15 13:49:20.000000 q1pulse-0.8.6/q1pulse/assembler/generator_data.py
--rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/assembler/instruction_queue.py
--rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.6/q1pulse/assembler/registers.py
--rw-rw-rw-   0        0        0    10775 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/instrument.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/lang/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/lang/__init__.py
--rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.6/q1pulse/lang/base.py
--rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/lang/exceptions.py
--rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.6/q1pulse/lang/expression.py
--rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.6/q1pulse/lang/flow_statements.py
--rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/lang/generator.py
--rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.6/q1pulse/lang/loops.py
--rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.6/q1pulse/lang/math_expressions.py
--rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.6/q1pulse/lang/register.py
--rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.6/q1pulse/lang/register_statements.py
--rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.6/q1pulse/lang/registers.py
--rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.6/q1pulse/lang/sequence.py
--rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.6/q1pulse/lang/simulator_statements.py
--rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/lang/timed_statements.py
--rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.6/q1pulse/lang/timeline.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/modules/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/modules/__init__.py
--rw-rw-rw-   0        0        0     8732 2023-06-30 07:44:08.000000 q1pulse-0.8.6/q1pulse/modules/modules.py
--rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/modules/sequencer_states.py
--rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.6/q1pulse/program.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/sequencer/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/sequencer/__init__.py
--rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.6/q1pulse/sequencer/builderbase.py
--rw-rw-rw-   0        0        0    14021 2023-06-30 08:39:46.000000 q1pulse-0.8.6/q1pulse/sequencer/control.py
--rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/sequencer/readout.py
--rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/sequencer/sequencer.py
--rw-rw-rw-   0        0        0     3389 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/sequencer/sequencer_data.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/util/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/util/__init__.py
--rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/util/qblox_version.py
-drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/
--rw-rw-rw-   0        0        0      193 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-06-30 11:35:49.000000 q1pulse-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-06-30 11:35:13.000000 q1pulse-0.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/
+-rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.7/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-06-30 12:43:52.000000 q1pulse-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/
+-rw-rw-rw-   0        0        0      139 2023-06-30 12:43:30.000000 q1pulse-0.8.7/q1pulse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/assembler/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/assembler/__init__.py
+-rw-rw-rw-   0        0        0    28695 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/assembler/generator.py
+-rw-rw-rw-   0        0        0     1813 2021-12-15 13:49:20.000000 q1pulse-0.8.7/q1pulse/assembler/generator_data.py
+-rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/assembler/instruction_queue.py
+-rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.7/q1pulse/assembler/registers.py
+-rw-rw-rw-   0        0        0    11312 2023-06-30 12:40:00.000000 q1pulse-0.8.7/q1pulse/instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/lang/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/lang/__init__.py
+-rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.7/q1pulse/lang/base.py
+-rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.7/q1pulse/lang/exceptions.py
+-rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.7/q1pulse/lang/expression.py
+-rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.7/q1pulse/lang/flow_statements.py
+-rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/lang/generator.py
+-rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.7/q1pulse/lang/loops.py
+-rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.7/q1pulse/lang/math_expressions.py
+-rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.7/q1pulse/lang/register.py
+-rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.7/q1pulse/lang/register_statements.py
+-rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.7/q1pulse/lang/registers.py
+-rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.7/q1pulse/lang/sequence.py
+-rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.7/q1pulse/lang/simulator_statements.py
+-rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/lang/timed_statements.py
+-rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.7/q1pulse/lang/timeline.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/modules/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/modules/__init__.py
+-rw-rw-rw-   0        0        0     8732 2023-06-30 11:37:00.000000 q1pulse-0.8.7/q1pulse/modules/modules.py
+-rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/modules/sequencer_states.py
+-rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.7/q1pulse/program.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/sequencer/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/sequencer/__init__.py
+-rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.7/q1pulse/sequencer/builderbase.py
+-rw-rw-rw-   0        0        0    14021 2023-06-30 11:37:00.000000 q1pulse-0.8.7/q1pulse/sequencer/control.py
+-rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/sequencer/readout.py
+-rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/sequencer/sequencer.py
+-rw-rw-rw-   0        0        0     3389 2022-12-22 08:51:07.000000 q1pulse-0.8.7/q1pulse/sequencer/sequencer_data.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse/util/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.7/q1pulse/util/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.7/q1pulse/util/qblox_version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-06-30 12:43:51.000000 q1pulse-0.8.7/q1pulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 12:43:51.000000 q1pulse-0.8.7/q1pulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 12:43:52.000000 q1pulse-0.8.7/q1pulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-06-30 12:43:52.000000 q1pulse-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-06-30 12:43:30.000000 q1pulse-0.8.7/setup.py
```

### Comparing `q1pulse-0.8.6/LICENSE` & `q1pulse-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/README.md` & `q1pulse-0.8.7/README.md`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/assembler/generator.py` & `q1pulse-0.8.7/q1pulse/assembler/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/assembler/generator_data.py` & `q1pulse-0.8.7/q1pulse/assembler/generator_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/assembler/instruction_queue.py` & `q1pulse-0.8.7/q1pulse/assembler/instruction_queue.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/assembler/registers.py` & `q1pulse-0.8.7/q1pulse/assembler/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/instrument.py` & `q1pulse-0.8.7/q1pulse/instrument.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .lang.exceptions import Q1InputOverloaded
 from .sequencer.sequencer import SequenceBuilder
 from .sequencer.control import ControlBuilder
 from .sequencer.readout import ReadoutBuilder
 from .modules.modules import QcmModule, QrmModule
 from .util.qblox_version import check_qblox_instrument_version
 from qblox_instruments import InstrumentType
+from qcodes.utils import DelayedKeyboardInterrupt
 
 logger = logging.getLogger(__name__)
 
 
 class Q1Instrument:
     # Postpone error checking till the end to save communication overhead.
     # System errors are only reported for SCPI errors. It's almost impossible to
@@ -95,109 +96,113 @@
         self.start_program(program)
         self.wait_stopped()
 
     def start_program(self, program):
         t_start = time.perf_counter()
 
         for instrument in self.root_instruments:
-            check_instrument_status(instrument)
-            if Q1Instrument._i_feel_lucky and hasattr(instrument, '_debug'):
-                # Change the debug level to speed up communication.
-                # Errors will be checked before start of the sequence.
-                instrument._debug = 2
+            with DelayedKeyboardInterrupt():
+                check_instrument_status(instrument)
+                if Q1Instrument._i_feel_lucky and hasattr(instrument, '_debug'):
+                    # Change the debug level to speed up communication.
+                    # Errors will be checked before start of the sequence.
+                    instrument._debug = 2
 
         instruments_with_sequence = set()
         sequencers = { **self.controllers, **self.readouts }
         for name,seq in sequencers.items():
-            module = self.modules[seq.module_name]
+            with DelayedKeyboardInterrupt():
+                module = self.modules[seq.module_name]
 
-            q1asm = program.q1asm(name)
-            self._loaded_q1asm[name] = q1asm
-            if q1asm is None:
-                module.disable_seq(seq)
-                logger.debug(f'Sequencer {name} no sequence')
-                continue
-            instruments_with_sequence.add(module.pulsar.root_instrument)
-            module.upload(seq.seq_nr, q1asm)
-            t = (time.perf_counter() - t_start) * 1000
-            # logger.debug(f'Sequencer {name} loaded ({t:5.3f} ms)')
-
-            module.enable_seq(seq)
-            prog_seq = program[name]
-            module.set_nco(seq.seq_nr, prog_seq.nco_frequency)
-            if prog_seq.modifies_frequency:
-                module.invalidate_cache(seq.seq_nr, 'nco_freq')
-            if prog_seq.mixer_gain_ratio is not None:
-                module.set_mixer_gain_ratio(seq.seq_nr, prog_seq.mixer_gain_ratio)
-            if prog_seq.mixer_phase_offset_degree is not None:
-                module.set_mixer_phase_offset_degree(seq.seq_nr, prog_seq.mixer_phase_offset_degree)
+                q1asm = program.q1asm(name)
+                self._loaded_q1asm[name] = q1asm
+                if q1asm is None:
+                    module.disable_seq(seq)
+                    logger.debug(f'Sequencer {name} no sequence')
+                    continue
+                instruments_with_sequence.add(module.pulsar.root_instrument)
+                module.upload(seq.seq_nr, q1asm)
+                t = (time.perf_counter() - t_start) * 1000
+                # logger.debug(f'Sequencer {name} loaded ({t:5.3f} ms)')
+
+                module.enable_seq(seq)
+                prog_seq = program[name]
+                module.set_nco(seq.seq_nr, prog_seq.nco_frequency)
+                if prog_seq.modifies_frequency:
+                    module.invalidate_cache(seq.seq_nr, 'nco_freq')
+                if prog_seq.mixer_gain_ratio is not None:
+                    module.set_mixer_gain_ratio(seq.seq_nr, prog_seq.mixer_gain_ratio)
+                if prog_seq.mixer_phase_offset_degree is not None:
+                    module.set_mixer_phase_offset_degree(seq.seq_nr, prog_seq.mixer_phase_offset_degree)
 
         t = (time.perf_counter() - t_start) * 1000
         # logger.debug(f'Configure QRMs ({t:5.3f} ms)')
         for name,seq in self.readouts.items():
-            readout = program[name]
-            module = self.modules[seq.module_name]
-            if not module.enabled(seq.seq_nr):
-                continue
-            module.thresholded_acq_rotation(seq.seq_nr, readout.thresholded_acq_rotation)
-            module.thresholded_acq_threshold(seq.seq_nr, readout.thresholded_acq_threshold)
-            module.integration_length_acq(seq.seq_nr, int(readout.integration_length_acq))
-            module.delete_acquisition_data(seq.seq_nr)
-
-        # Note: arm per sequencer. Arm on the cluster still gives red leds on the modules.
-        for module in self.modules.values():
-            module.arm_sequencers()
-#        for instrument in instruments_with_sequence:
-#            instrument.arm_sequencer()
-
-        if Q1Instrument._i_feel_lucky:
-            t = (time.perf_counter() - t_start) * 1000
-            # logger.debug(f'Check status  ({t:5.3f} ms)')
-            self.check_system_errors()
-
-        for instrument in instruments_with_sequence:
-            t = (time.perf_counter() - t_start) * 1000
-            # logger.debug(f'Start  ({t:5.3f} ms)')
-            instrument.start_sequencer()
+            with DelayedKeyboardInterrupt():
+                readout = program[name]
+                module = self.modules[seq.module_name]
+                if not module.enabled(seq.seq_nr):
+                    continue
+                module.thresholded_acq_rotation(seq.seq_nr, readout.thresholded_acq_rotation)
+                module.thresholded_acq_threshold(seq.seq_nr, readout.thresholded_acq_threshold)
+                module.integration_length_acq(seq.seq_nr, int(readout.integration_length_acq))
+                module.delete_acquisition_data(seq.seq_nr)
+
+        with DelayedKeyboardInterrupt():
+            # Note: arm per sequencer. Arm on the cluster still gives red leds on the modules.
+            for module in self.modules.values():
+                module.arm_sequencers()
+
+            if Q1Instrument._i_feel_lucky:
+                t = (time.perf_counter() - t_start) * 1000
+                # logger.debug(f'Check status  ({t:5.3f} ms)')
+                self.check_system_errors()
+
+            for instrument in instruments_with_sequence:
+                t = (time.perf_counter() - t_start) * 1000
+                # logger.debug(f'Start  ({t:5.3f} ms)')
+                instrument.start_sequencer()
 
         t = (time.perf_counter() - t_start) * 1000
         logger.info(f'Duration upload/start: ({t:5.3f}ms)')
 
     def wait_stopped(self, timeout_minutes=1):
         # Wait for completion
         errors = {}
         msg_level = 0
         sequencers = { **self.controllers, **self.readouts }
         for name,seq in sequencers.items():
-            module = self.modules[seq.module_name]
-            if not module.enabled(seq.seq_nr):
-                continue
-            state = module.get_sequencer_state(seq.seq_nr, timeout_minutes)
-            logger.log(state.level,
-                        f'Status {name} ({module.pulsar.name}:{seq.seq_nr}):'
-                         f'{state}')
-            msg_level = max(msg_level, state.level)
-            if state.input_overloaded:
-                if Q1Instrument._exception_on_overload:
-                    raise Q1InputOverloaded(
-                            f'INPUT OVERLOAD on {name}.'
-                            '\nException can be suppressed with q1pulse.set_exception_on_overload(False)')
-                else:
-                    print(f'WARNING: input overload on {name}')
-            if state.status != 'STOPPED' or state.level >= logging.WARNING:
-                errors[name] = str(state)
+            with DelayedKeyboardInterrupt():
+                module = self.modules[seq.module_name]
+                if not module.enabled(seq.seq_nr):
+                    continue
+                state = module.get_sequencer_state(seq.seq_nr, timeout_minutes)
+                logger.log(state.level,
+                            f'Status {name} ({module.pulsar.name}:{seq.seq_nr}):'
+                             f'{state}')
+                msg_level = max(msg_level, state.level)
+                if state.input_overloaded:
+                    if Q1Instrument._exception_on_overload:
+                        raise Q1InputOverloaded(
+                                f'INPUT OVERLOAD on {name}.'
+                                '\nException can be suppressed with q1pulse.set_exception_on_overload(False)')
+                    else:
+                        print(f'WARNING: input overload on {name}')
+                if state.status != 'STOPPED' or state.level >= logging.WARNING:
+                    errors[name] = str(state)
         if msg_level == logging.ERROR:
             logger.error('*** Program errors ***')
             for name,state in errors.items():
                 logger.error(f'  {name}: {state}')
             raise Exception(f'Q1 failures (see logger):\n {errors}')
 
-        for instrument in self.root_instruments:
-            logger.info(f'Stop sequencers')
-            instrument.stop_sequencer()
+        with DelayedKeyboardInterrupt():
+            for instrument in self.root_instruments:
+                logger.info(f'Stop sequencers')
+                instrument.stop_sequencer()
 
     def check_system_errors(self):
         for instrument in self.root_instruments:
             errors = []
             while instrument.get_num_system_error() != 0:
                 errors.append(instrument.get_system_error())
 
@@ -211,18 +216,19 @@
     def get_acquisition_bins(self, sequencer_name, bins):
         seq = self.readouts[sequencer_name]
         q1asm = self._loaded_q1asm[sequencer_name]
         if q1asm is None or len(q1asm['acquisitions']) == 0:
             logger.warning(f'No acquisitions for {sequencer_name}')
             return None
         module = self.modules[seq.module_name]
-        state = module.pulsar.get_acquisition_state(seq.seq_nr, 1)
-        logger.info(f'Acquisition status {sequencer_name} ({module.pulsar.name}:'
-                     f'{seq.seq_nr}): {state}')
-        return module.pulsar.get_acquisitions(seq.seq_nr)[bins]['acquisition']['bins']
+        with DelayedKeyboardInterrupt():
+            state = module.pulsar.get_acquisition_state(seq.seq_nr, 1)
+            logger.info(f'Acquisition status {sequencer_name} ({module.pulsar.name}:'
+                         f'{seq.seq_nr}): {state}')
+            return module.pulsar.get_acquisitions(seq.seq_nr)[bins]['acquisition']['bins']
 
     def get_input_ranges(self, sequencer_name):
         ''' Returns input range for both channels of sequencer.
         Value is in Vpp.
         '''
         seq = self.readouts[sequencer_name]
         module = self.modules[seq.module_name]
```

### Comparing `q1pulse-0.8.6/q1pulse/lang/exceptions.py` & `q1pulse-0.8.7/q1pulse/lang/exceptions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/flow_statements.py` & `q1pulse-0.8.7/q1pulse/lang/flow_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/generator.py` & `q1pulse-0.8.7/q1pulse/lang/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/loops.py` & `q1pulse-0.8.7/q1pulse/lang/loops.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/math_expressions.py` & `q1pulse-0.8.7/q1pulse/lang/math_expressions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/register.py` & `q1pulse-0.8.7/q1pulse/lang/register.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/register_statements.py` & `q1pulse-0.8.7/q1pulse/lang/register_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/registers.py` & `q1pulse-0.8.7/q1pulse/lang/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/sequence.py` & `q1pulse-0.8.7/q1pulse/lang/sequence.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/simulator_statements.py` & `q1pulse-0.8.7/q1pulse/lang/simulator_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/timed_statements.py` & `q1pulse-0.8.7/q1pulse/lang/timed_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/lang/timeline.py` & `q1pulse-0.8.7/q1pulse/lang/timeline.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/modules/modules.py` & `q1pulse-0.8.7/q1pulse/modules/modules.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/modules/sequencer_states.py` & `q1pulse-0.8.7/q1pulse/modules/sequencer_states.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/program.py` & `q1pulse-0.8.7/q1pulse/program.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/sequencer/control.py` & `q1pulse-0.8.7/q1pulse/sequencer/control.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/sequencer/readout.py` & `q1pulse-0.8.7/q1pulse/sequencer/readout.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/sequencer/sequencer.py` & `q1pulse-0.8.7/q1pulse/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/sequencer/sequencer_data.py` & `q1pulse-0.8.7/q1pulse/sequencer/sequencer_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse/util/qblox_version.py` & `q1pulse-0.8.7/q1pulse/util/qblox_version.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.6/q1pulse.egg-info/SOURCES.txt` & `q1pulse-0.8.7/q1pulse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

