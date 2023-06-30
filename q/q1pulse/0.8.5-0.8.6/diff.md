# Comparing `tmp/q1pulse-0.8.5.tar.gz` & `tmp/q1pulse-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1pulse-0.8.5.tar", last modified: Mon Mar 13 17:12:17 2023, max compression
+gzip compressed data, was "dist\q1pulse-0.8.6.tar", last modified: Fri Jun 30 11:35:49 2023, max compression
```

## Comparing `q1pulse-0.8.5.tar` & `q1pulse-0.8.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/
--rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.5/LICENSE
--rw-rw-rw-   0        0        0      193 2023-03-13 17:12:17.000000 q1pulse-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/
--rw-rw-rw-   0        0        0      139 2023-03-13 17:11:40.000000 q1pulse-0.8.5/q1pulse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/assembler/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.5/q1pulse/assembler/__init__.py
--rw-rw-rw-   0        0        0    28695 2023-02-08 14:26:47.000000 q1pulse-0.8.5/q1pulse/assembler/generator.py
--rw-rw-rw-   0        0        0     1813 2021-12-15 13:49:20.000000 q1pulse-0.8.5/q1pulse/assembler/generator_data.py
--rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.5/q1pulse/assembler/instruction_queue.py
--rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.5/q1pulse/assembler/registers.py
--rw-rw-rw-   0        0        0    10775 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/instrument.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/lang/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.5/q1pulse/lang/__init__.py
--rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.5/q1pulse/lang/base.py
--rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.5/q1pulse/lang/exceptions.py
--rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.5/q1pulse/lang/expression.py
--rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.5/q1pulse/lang/flow_statements.py
--rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.5/q1pulse/lang/generator.py
--rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.5/q1pulse/lang/loops.py
--rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.5/q1pulse/lang/math_expressions.py
--rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.5/q1pulse/lang/register.py
--rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.5/q1pulse/lang/register_statements.py
--rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.5/q1pulse/lang/registers.py
--rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.5/q1pulse/lang/sequence.py
--rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.5/q1pulse/lang/simulator_statements.py
--rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.5/q1pulse/lang/timed_statements.py
--rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.5/q1pulse/lang/timeline.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/modules/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.5/q1pulse/modules/__init__.py
--rw-rw-rw-   0        0        0     8536 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/modules/modules.py
--rw-rw-rw-   0        0        0     2924 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/modules/sequencer_states.py
--rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.5/q1pulse/program.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/sequencer/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.5/q1pulse/sequencer/__init__.py
--rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.5/q1pulse/sequencer/builderbase.py
--rw-rw-rw-   0        0        0    14027 2023-01-23 11:03:43.000000 q1pulse-0.8.5/q1pulse/sequencer/control.py
--rw-rw-rw-   0        0        0     6224 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/sequencer/readout.py
--rw-rw-rw-   0        0        0     9429 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/sequencer/sequencer.py
--rw-rw-rw-   0        0        0     3389 2022-12-22 08:51:07.000000 q1pulse-0.8.5/q1pulse/sequencer/sequencer_data.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse/util/
--rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.5/q1pulse/util/__init__.py
--rw-rw-rw-   0        0        0      543 2023-03-13 17:09:48.000000 q1pulse-0.8.5/q1pulse/util/qblox_version.py
-drwxrwxrwx   0        0        0        0 2023-03-13 17:12:17.000000 q1pulse-0.8.5/q1pulse.egg-info/
--rw-rw-rw-   0        0        0      193 2023-03-13 17:12:16.000000 q1pulse-0.8.5/q1pulse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1172 2023-03-13 17:12:16.000000 q1pulse-0.8.5/q1pulse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 17:12:16.000000 q1pulse-0.8.5/q1pulse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-03-13 17:12:16.000000 q1pulse-0.8.5/q1pulse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-13 17:12:16.000000 q1pulse-0.8.5/q1pulse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-03-13 17:12:17.000000 q1pulse-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0      310 2023-03-13 17:11:40.000000 q1pulse-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/
+-rw-rw-rw-   0        0        0     1092 2021-11-11 10:01:53.000000 q1pulse-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0      193 2023-06-30 11:35:49.000000 q1pulse-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11766 2023-01-23 11:03:43.000000 q1pulse-0.8.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/
+-rw-rw-rw-   0        0        0      139 2023-06-30 11:35:13.000000 q1pulse-0.8.6/q1pulse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/assembler/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/assembler/__init__.py
+-rw-rw-rw-   0        0        0    28695 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/assembler/generator.py
+-rw-rw-rw-   0        0        0     1813 2021-12-15 13:49:20.000000 q1pulse-0.8.6/q1pulse/assembler/generator_data.py
+-rw-rw-rw-   0        0        0     9745 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/assembler/instruction_queue.py
+-rw-rw-rw-   0        0        0     3362 2022-11-16 09:08:45.000000 q1pulse-0.8.6/q1pulse/assembler/registers.py
+-rw-rw-rw-   0        0        0    10775 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/lang/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/lang/__init__.py
+-rw-rw-rw-   0        0        0      148 2021-11-28 16:59:16.000000 q1pulse-0.8.6/q1pulse/lang/base.py
+-rw-rw-rw-   0        0        0     1478 2023-02-08 14:26:47.000000 q1pulse-0.8.6/q1pulse/lang/exceptions.py
+-rw-rw-rw-   0        0        0       58 2021-10-29 08:53:34.000000 q1pulse-0.8.6/q1pulse/lang/expression.py
+-rw-rw-rw-   0        0        0     3690 2021-12-15 16:47:33.000000 q1pulse-0.8.6/q1pulse/lang/flow_statements.py
+-rw-rw-rw-   0        0        0     3115 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/lang/generator.py
+-rw-rw-rw-   0        0        0     3548 2021-12-13 20:45:54.000000 q1pulse-0.8.6/q1pulse/lang/loops.py
+-rw-rw-rw-   0        0        0     7850 2022-07-08 12:12:01.000000 q1pulse-0.8.6/q1pulse/lang/math_expressions.py
+-rw-rw-rw-   0        0        0      690 2021-12-12 23:23:38.000000 q1pulse-0.8.6/q1pulse/lang/register.py
+-rw-rw-rw-   0        0        0     1011 2021-12-12 23:43:16.000000 q1pulse-0.8.6/q1pulse/lang/register_statements.py
+-rw-rw-rw-   0        0        0     1407 2021-12-13 20:49:12.000000 q1pulse-0.8.6/q1pulse/lang/registers.py
+-rw-rw-rw-   0        0        0     2494 2021-12-14 14:34:49.000000 q1pulse-0.8.6/q1pulse/lang/sequence.py
+-rw-rw-rw-   0        0        0      603 2021-12-13 19:51:31.000000 q1pulse-0.8.6/q1pulse/lang/simulator_statements.py
+-rw-rw-rw-   0        0        0     4557 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/lang/timed_statements.py
+-rw-rw-rw-   0        0        0      994 2021-12-13 20:51:09.000000 q1pulse-0.8.6/q1pulse/lang/timeline.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/modules/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/modules/__init__.py
+-rw-rw-rw-   0        0        0     8732 2023-06-30 07:44:08.000000 q1pulse-0.8.6/q1pulse/modules/modules.py
+-rw-rw-rw-   0        0        0     2924 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/modules/sequencer_states.py
+-rw-rw-rw-   0        0        0     5377 2022-12-19 08:32:38.000000 q1pulse-0.8.6/q1pulse/program.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/sequencer/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/sequencer/__init__.py
+-rw-rw-rw-   0        0        0      269 2021-11-12 10:32:12.000000 q1pulse-0.8.6/q1pulse/sequencer/builderbase.py
+-rw-rw-rw-   0        0        0    14021 2023-06-30 08:39:46.000000 q1pulse-0.8.6/q1pulse/sequencer/control.py
+-rw-rw-rw-   0        0        0     6224 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/sequencer/readout.py
+-rw-rw-rw-   0        0        0     9429 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/sequencer/sequencer.py
+-rw-rw-rw-   0        0        0     3389 2022-12-22 08:51:07.000000 q1pulse-0.8.6/q1pulse/sequencer/sequencer_data.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse/util/
+-rw-rw-rw-   0        0        0        0 2021-10-29 10:16:24.000000 q1pulse-0.8.6/q1pulse/util/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-03-13 17:20:01.000000 q1pulse-0.8.6/q1pulse/util/qblox_version.py
+drwxrwxrwx   0        0        0        0 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/
+-rw-rw-rw-   0        0        0      193 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1172 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 11:35:48.000000 q1pulse-0.8.6/q1pulse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 11:35:49.000000 q1pulse-0.8.6/q1pulse.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-06-30 11:35:49.000000 q1pulse-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0      310 2023-06-30 11:35:13.000000 q1pulse-0.8.6/setup.py
```

### Comparing `q1pulse-0.8.5/LICENSE` & `q1pulse-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/README.md` & `q1pulse-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/assembler/generator.py` & `q1pulse-0.8.6/q1pulse/assembler/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/assembler/generator_data.py` & `q1pulse-0.8.6/q1pulse/assembler/generator_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/assembler/instruction_queue.py` & `q1pulse-0.8.6/q1pulse/assembler/instruction_queue.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/assembler/registers.py` & `q1pulse-0.8.6/q1pulse/assembler/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/instrument.py` & `q1pulse-0.8.6/q1pulse/instrument.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/exceptions.py` & `q1pulse-0.8.6/q1pulse/lang/exceptions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/flow_statements.py` & `q1pulse-0.8.6/q1pulse/lang/flow_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/generator.py` & `q1pulse-0.8.6/q1pulse/lang/generator.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/loops.py` & `q1pulse-0.8.6/q1pulse/lang/loops.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/math_expressions.py` & `q1pulse-0.8.6/q1pulse/lang/math_expressions.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/register.py` & `q1pulse-0.8.6/q1pulse/lang/register.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/register_statements.py` & `q1pulse-0.8.6/q1pulse/lang/register_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/registers.py` & `q1pulse-0.8.6/q1pulse/lang/registers.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/sequence.py` & `q1pulse-0.8.6/q1pulse/lang/sequence.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/simulator_statements.py` & `q1pulse-0.8.6/q1pulse/lang/simulator_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/timed_statements.py` & `q1pulse-0.8.6/q1pulse/lang/timed_statements.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/lang/timeline.py` & `q1pulse-0.8.6/q1pulse/lang/timeline.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/modules/modules.py` & `q1pulse-0.8.6/q1pulse/modules/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 class QbloxModule:
     verbose = False
     n_sequencers = 6
 
     def __init__(self, pulsar):
         self.name = pulsar.name
+        # check module is present in slot.
+        if hasattr(pulsar, 'present'):
+            if not pulsar.present():
+                raise Exception('No module in slot {pulsar.slot_idx()}')
         self.pulsar = pulsar
         self._allocated_seq = 0
         self.disable_all_out()
         # disable all sequencers
         for seq_nr in range(0, self.n_sequencers):
             self.enable_sync(seq_nr, False)
```

### Comparing `q1pulse-0.8.5/q1pulse/modules/sequencer_states.py` & `q1pulse-0.8.6/q1pulse/modules/sequencer_states.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/program.py` & `q1pulse-0.8.6/q1pulse/program.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/sequencer/control.py` & `q1pulse-0.8.6/q1pulse/sequencer/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,15 @@
                         self.set_offset(self.Rs._ramp_offset)
                         self.play(w_ramp)
                         self.Rs._ramp_offset += step
                         self.wait(ramp_loop_time)
                     self.set_offset(self.Rs._ramp_offset)
                     self.play(w_ramp)
                     self.wait(rem)
+                    self.set_gain(0.0)
                 else:
                     # steps of 1 LSB
                     min_step = lsb
                     n_steps = int(abs(v_end - v_start) / min_step)
                     if n_steps == 0:
                         n = 0
                         rem = duration
@@ -245,17 +246,16 @@
                             self.wait(t_step)
                     self.set_offset(self.Rs._ramp_offset)
                     self.wait(rem)
 
             if v_after is not None:
                 # set constant value
                 self.set_offset(v_after)
-                self.set_gain(0.0)
             else:
-                # assume there will be another instruction setting offset and gain.
+                # assume there will be another instruction setting offset
                 pass
 
     def chirp(self, duration, amplitude, f_start, f_end, t_offset=0):
         if isinstance(duration, (Register, Expression)):
             raise Q1TypeError('Chirp duration cannot be a variable or expression; '
                               'Unroll loop using Python for-loop.')
         if (isinstance(f_start, (Register, Expression))
```

### Comparing `q1pulse-0.8.5/q1pulse/sequencer/readout.py` & `q1pulse-0.8.6/q1pulse/sequencer/readout.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/sequencer/sequencer.py` & `q1pulse-0.8.6/q1pulse/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/sequencer/sequencer_data.py` & `q1pulse-0.8.6/q1pulse/sequencer/sequencer_data.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse/util/qblox_version.py` & `q1pulse-0.8.6/q1pulse/util/qblox_version.py`

 * *Files identical despite different names*

### Comparing `q1pulse-0.8.5/q1pulse.egg-info/SOURCES.txt` & `q1pulse-0.8.6/q1pulse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

