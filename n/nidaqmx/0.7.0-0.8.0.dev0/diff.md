# Comparing `tmp/nidaqmx-0.7.0.tar.gz` & `tmp/nidaqmx-0.8.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nidaqmx-0.7.0.tar", max compression
+gzip compressed data, was "nidaqmx-0.8.0.dev0.tar", max compression
```

## Comparing `nidaqmx-0.7.0.tar` & `nidaqmx-0.8.0.dev0.tar`

### file list

```diff
@@ -1,63 +1,74 @@
--rw-r--r--   0        0        0      467 2023-04-03 18:57:20.408212 nidaqmx-0.7.0/generated/nidaqmx/__init__.py
--rw-r--r--   0        0        0     7398 2023-04-05 15:42:42.315923 nidaqmx-0.7.0/generated/nidaqmx/_lib.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.409211 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/__init__.py
--rw-r--r--   0        0        0   208331 2023-04-05 15:42:42.317919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ai_channel_collection.py
--rw-r--r--   0        0        0     8810 2023-04-05 15:42:42.318918 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ao_channel_collection.py
--rw-r--r--   0        0        0     4971 2023-04-05 15:42:42.319918 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channel_collection.py
--rw-r--r--   0        0        0      512 2023-04-03 18:57:20.410211 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/__init__.py
--rw-r--r--   0        0        0   342852 2023-04-05 20:08:29.824486 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/ai_channel.py
--rw-r--r--   0        0        0    81010 2023-04-05 15:42:42.324919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/ao_channel.py
--rw-r--r--   0        0        0    16195 2023-04-05 15:42:42.325920 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/channel.py
--rw-r--r--   0        0        0   469245 2023-04-05 20:08:29.827485 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/ci_channel.py
--rw-r--r--   0        0        0    64324 2023-04-05 15:42:42.329920 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/co_channel.py
--rw-r--r--   0        0        0    29334 2023-04-05 15:42:42.330919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/di_channel.py
--rw-r--r--   0        0        0    32347 2023-04-05 15:42:42.331920 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/do_channel.py
--rw-r--r--   0        0        0    53188 2023-04-05 15:42:42.332919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ci_channel_collection.py
--rw-r--r--   0        0        0     9874 2023-04-05 15:42:42.333918 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/co_channel_collection.py
--rw-r--r--   0        0        0     4390 2023-04-05 15:42:42.334918 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/di_channel_collection.py
--rw-r--r--   0        0        0     4388 2023-04-05 15:42:42.335920 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/do_channel_collection.py
--rw-r--r--   0        0        0    95912 2023-04-05 15:42:42.336919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/export_signals.py
--rw-r--r--   0        0        0    91612 2023-04-05 15:42:42.337919 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/in_stream.py
--rw-r--r--   0        0        0    40829 2023-04-05 15:42:42.338920 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/out_stream.py
--rw-r--r--   0        0        0    24950 2023-04-03 18:57:20.411212 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/read_functions.py
--rw-r--r--   0        0        0   116423 2023-04-05 15:42:42.340977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/timing.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.411212 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/__init__.py
--rw-r--r--   0        0        0    21204 2023-04-05 15:42:42.341977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py
--rw-r--r--   0        0        0     5769 2023-04-05 15:42:42.342983 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py
--rw-r--r--   0        0        0    58735 2023-04-05 15:42:42.343977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py
--rw-r--r--   0        0        0    97681 2023-04-05 15:42:42.344977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py
--rw-r--r--   0        0        0    94939 2023-04-05 15:42:42.345977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggering/start_trigger.py
--rw-r--r--   0        0        0     4452 2023-04-05 15:42:42.346977 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/triggers.py
--rw-r--r--   0        0        0    15876 2023-04-03 18:57:20.412212 nidaqmx-0.7.0/generated/nidaqmx/_task_modules/write_functions.py
--rw-r--r--   0        0        0    50249 2023-04-03 19:47:30.482012 nidaqmx-0.7.0/generated/nidaqmx/constants.py
--rw-r--r--   0        0        0    93605 2023-04-03 19:47:30.466051 nidaqmx-0.7.0/generated/nidaqmx/error_codes.py
--rw-r--r--   0        0        0     6261 2023-04-05 15:42:42.347979 nidaqmx-0.7.0/generated/nidaqmx/errors.py
--rw-r--r--   0        0        0    36338 2023-04-05 15:42:42.348982 nidaqmx-0.7.0/generated/nidaqmx/scale.py
--rw-r--r--   0        0        0   116823 2023-04-05 15:42:42.350979 nidaqmx-0.7.0/generated/nidaqmx/stream_readers.py
--rw-r--r--   0        0        0    67211 2023-04-05 15:42:42.350979 nidaqmx-0.7.0/generated/nidaqmx/stream_writers.py
--rw-r--r--   0        0        0      426 2023-04-03 18:57:20.415213 nidaqmx-0.7.0/generated/nidaqmx/system/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.415213 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/__init__.py
--rw-r--r--   0        0        0     4020 2023-04-05 15:42:42.352980 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/device_collection.py
--rw-r--r--   0        0        0     4272 2023-04-05 15:42:42.353980 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/persisted_channel_collection.py
--rw-r--r--   0        0        0     4138 2023-04-05 15:42:42.354980 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/persisted_scale_collection.py
--rw-r--r--   0        0        0     4074 2023-04-05 15:42:42.354980 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/persisted_task_collection.py
--rw-r--r--   0        0        0    13588 2023-04-05 15:42:42.355977 nidaqmx-0.7.0/generated/nidaqmx/system/_collections/physical_channel_collection.py
--rw-r--r--   0        0        0        0 2023-04-03 18:57:20.419223 nidaqmx-0.7.0/generated/nidaqmx/system/_watchdog_modules/__init__.py
--rw-r--r--   0        0        0    10418 2023-04-05 15:42:42.355977 nidaqmx-0.7.0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py
--rw-r--r--   0        0        0     1376 2023-04-05 15:42:42.356977 nidaqmx-0.7.0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py
--rw-r--r--   0        0        0    91456 2023-04-05 20:08:29.829494 nidaqmx-0.7.0/generated/nidaqmx/system/device.py
--rw-r--r--   0        0        0    43419 2023-04-05 20:08:29.830489 nidaqmx-0.7.0/generated/nidaqmx/system/physical_channel.py
--rw-r--r--   0        0        0      275 2023-04-03 18:57:20.420224 nidaqmx-0.7.0/generated/nidaqmx/system/storage/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-03 18:57:20.421213 nidaqmx-0.7.0/generated/nidaqmx/system/storage/_alternate_task_constructor.py
--rw-r--r--   0        0        0     3913 2023-04-05 15:42:42.359977 nidaqmx-0.7.0/generated/nidaqmx/system/storage/persisted_channel.py
--rw-r--r--   0        0        0     4136 2023-04-05 15:42:42.360978 nidaqmx-0.7.0/generated/nidaqmx/system/storage/persisted_scale.py
--rw-r--r--   0        0        0     4770 2023-04-05 15:42:42.361977 nidaqmx-0.7.0/generated/nidaqmx/system/storage/persisted_task.py
--rw-r--r--   0        0        0    35069 2023-04-05 15:42:42.361977 nidaqmx-0.7.0/generated/nidaqmx/system/system.py
--rw-r--r--   0        0        0    25625 2023-04-05 20:08:29.831494 nidaqmx-0.7.0/generated/nidaqmx/system/watchdog.py
--rw-r--r--   0        0        0    57288 2023-04-05 15:42:42.364981 nidaqmx-0.7.0/generated/nidaqmx/task.py
--rw-r--r--   0        0        0     1430 2023-04-03 18:57:20.423214 nidaqmx-0.7.0/generated/nidaqmx/types.py
--rw-r--r--   0        0        0     8896 2023-04-05 15:42:42.365980 nidaqmx-0.7.0/generated/nidaqmx/utils.py
--rw-r--r--   0        0        0     1213 2022-05-26 20:15:36.274851 nidaqmx-0.7.0/LICENSE
--rw-r--r--   0        0        0     2480 2023-04-06 16:16:13.859658 nidaqmx-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7076 2023-04-05 15:42:42.306919 nidaqmx-0.7.0/README.rst
--rw-r--r--   0        0        0     8916 1970-01-01 00:00:00.000000 nidaqmx-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      640 2023-06-30 20:45:34.816394 nidaqmx-0.8.0.dev0/generated/nidaqmx/__init__.py
+-rw-r--r--   0        0        0    61393 2023-06-30 20:45:34.817435 nidaqmx-0.8.0.dev0/generated/nidaqmx/_base_interpreter.py
+-rw-r--r--   0        0        0     1505 2023-06-30 20:45:34.818394 nidaqmx-0.8.0.dev0/generated/nidaqmx/_bitfield_utils.py
+-rw-r--r--   0        0        0   167908 2023-06-30 20:45:34.819411 nidaqmx-0.8.0.dev0/generated/nidaqmx/_grpc_interpreter.py
+-rw-r--r--   0        0        0     6060 2023-06-30 20:45:34.819411 nidaqmx-0.8.0.dev0/generated/nidaqmx/_lib.py
+-rw-r--r--   0        0        0   259462 2023-06-30 20:45:34.820394 nidaqmx-0.8.0.dev0/generated/nidaqmx/_library_interpreter.py
+-rw-r--r--   0        0        0       34 2023-06-30 20:45:34.821432 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/__init__.py
+-rw-r--r--   0        0        0   573921 2023-06-30 20:45:34.824422 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.py
+-rw-r--r--   0        0        0  1643650 2023-06-30 20:45:34.831990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2.pyi
+-rw-r--r--   0        0        0   671385 2023-06-30 20:45:34.836990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.py
+-rw-r--r--   0        0        0   158814 2023-06-30 20:45:34.838017 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/nidaqmx_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4248 2023-06-30 20:45:34.838991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.py
+-rw-r--r--   0        0        0     8974 2023-06-30 20:45:34.838991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2.pyi
+-rw-r--r--   0        0        0     9124 2023-06-30 20:45:34.839991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.py
+-rw-r--r--   0        0        0     2923 2023-06-30 20:45:34.839991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_stubs/session_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.409211 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/__init__.py
+-rw-r--r--   0        0        0   178850 2023-06-30 20:45:34.842018 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ai_channel_collection.py
+-rw-r--r--   0        0        0     7596 2023-06-30 20:45:34.842018 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ao_channel_collection.py
+-rw-r--r--   0        0        0     4276 2023-06-30 20:45:34.842991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channel_collection.py
+-rw-r--r--   0        0        0      512 2023-04-03 18:57:20.410211 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/__init__.py
+-rw-r--r--   0        0        0   142396 2023-06-30 20:45:34.844009 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ai_channel.py
+-rw-r--r--   0        0        0    33120 2023-06-30 20:45:34.845010 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ao_channel.py
+-rw-r--r--   0        0        0    10280 2023-06-30 20:45:34.845989 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/channel.py
+-rw-r--r--   0        0        0   181156 2023-06-30 20:45:34.847009 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/ci_channel.py
+-rw-r--r--   0        0        0    26347 2023-06-30 20:45:34.847991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/co_channel.py
+-rw-r--r--   0        0        0    12499 2023-06-30 20:45:34.847991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/di_channel.py
+-rw-r--r--   0        0        0    13754 2023-06-30 20:45:34.848991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/do_channel.py
+-rw-r--r--   0        0        0    46387 2023-06-30 20:45:34.848991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ci_channel_collection.py
+-rw-r--r--   0        0        0     8612 2023-06-30 20:45:34.849990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/co_channel_collection.py
+-rw-r--r--   0        0        0     4096 2023-06-30 20:45:34.849990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/di_channel_collection.py
+-rw-r--r--   0        0        0     4094 2023-06-30 20:45:34.850991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/do_channel_collection.py
+-rw-r--r--   0        0        0    36299 2023-06-30 20:45:34.850991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/export_signals.py
+-rw-r--r--   0        0        0    48904 2023-06-30 20:45:34.851991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/in_stream.py
+-rw-r--r--   0        0        0    21499 2023-06-30 20:45:34.852990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/out_stream.py
+-rw-r--r--   0        0        0    53479 2023-06-30 20:45:34.852990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/timing.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.411212 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/__init__.py
+-rw-r--r--   0        0        0     7885 2023-06-30 20:45:34.853991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/arm_start_trigger.py
+-rw-r--r--   0        0        0     2118 2023-06-30 20:45:34.853991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/handshake_trigger.py
+-rw-r--r--   0        0        0    22198 2023-06-30 20:45:34.854991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/pause_trigger.py
+-rw-r--r--   0        0        0    42343 2023-06-30 20:45:34.854991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/reference_trigger.py
+-rw-r--r--   0        0        0    39696 2023-06-30 20:45:34.855991 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggering/start_trigger.py
+-rw-r--r--   0        0        0     3368 2023-06-30 20:45:34.856990 nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/triggers.py
+-rw-r--r--   0        0        0    50249 2023-04-03 19:47:30.482012 nidaqmx-0.8.0.dev0/generated/nidaqmx/constants.py
+-rw-r--r--   0        0        0    93605 2023-04-03 19:47:30.466051 nidaqmx-0.8.0.dev0/generated/nidaqmx/error_codes.py
+-rw-r--r--   0        0        0     5869 2023-06-30 20:45:34.856990 nidaqmx-0.8.0.dev0/generated/nidaqmx/errors.py
+-rw-r--r--   0        0        0     3587 2023-06-30 20:45:34.857990 nidaqmx-0.8.0.dev0/generated/nidaqmx/grpc_session_options.py
+-rw-r--r--   0        0        0    22198 2023-06-30 20:45:34.857990 nidaqmx-0.8.0.dev0/generated/nidaqmx/scale.py
+-rw-r--r--   0        0        0   119899 2023-06-30 20:45:34.858991 nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_readers.py
+-rw-r--r--   0        0        0    68185 2023-06-30 20:45:34.859991 nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_writers.py
+-rw-r--r--   0        0        0      426 2023-04-03 18:57:20.415213 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.415213 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/__init__.py
+-rw-r--r--   0        0        0     3579 2023-06-30 20:45:34.860991 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/device_collection.py
+-rw-r--r--   0        0        0     3840 2023-06-30 20:45:34.860991 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_channel_collection.py
+-rw-r--r--   0        0        0     3700 2023-06-30 20:45:34.861989 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_scale_collection.py
+-rw-r--r--   0        0        0     3635 2023-06-30 20:45:34.861989 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_task_collection.py
+-rw-r--r--   0        0        0     7366 2023-06-30 20:45:34.862990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/physical_channel_collection.py
+-rw-r--r--   0        0        0        0 2023-04-03 18:57:20.419223 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/__init__.py
+-rw-r--r--   0        0        0     6072 2023-06-30 20:45:34.862990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_state.py
+-rw-r--r--   0        0        0     1473 2023-06-30 20:45:34.863990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py
+-rw-r--r--   0        0        0    39429 2023-06-30 20:45:34.863990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/device.py
+-rw-r--r--   0        0        0    24660 2023-06-30 20:45:34.864990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/physical_channel.py
+-rw-r--r--   0        0        0      275 2023-04-03 18:57:20.420224 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/__init__.py
+-rw-r--r--   0        0        0     3159 2023-06-30 20:45:34.864990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_channel.py
+-rw-r--r--   0        0        0     3426 2023-06-30 20:45:34.865990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_scale.py
+-rw-r--r--   0        0        0     3560 2023-06-30 20:45:34.865990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/storage/persisted_task.py
+-rw-r--r--   0        0        0    26836 2023-06-30 20:45:34.866990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/system.py
+-rw-r--r--   0        0        0    16001 2023-06-30 20:45:34.866990 nidaqmx-0.8.0.dev0/generated/nidaqmx/system/watchdog.py
+-rw-r--r--   0        0        0    54236 2023-06-30 20:45:34.867990 nidaqmx-0.8.0.dev0/generated/nidaqmx/task.py
+-rw-r--r--   0        0        0     1430 2023-04-03 18:57:20.423214 nidaqmx-0.8.0.dev0/generated/nidaqmx/types.py
+-rw-r--r--   0        0        0     9543 2023-06-30 20:45:34.868989 nidaqmx-0.8.0.dev0/generated/nidaqmx/utils.py
+-rw-r--r--   0        0        0     1213 2022-05-26 20:15:36.274851 nidaqmx-0.8.0.dev0/LICENSE
+-rw-r--r--   0        0        0     5029 2023-06-30 20:45:34.869989 nidaqmx-0.8.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7076 2023-04-05 15:42:42.306919 nidaqmx-0.8.0.dev0/README.rst
+-rw-r--r--   0        0        0     8901 1970-01-01 00:00:00.000000 nidaqmx-0.8.0.dev0/PKG-INFO
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_lib.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ctypes.util import find_library
 import ctypes
 from numpy.ctypeslib import ndpointer
 import platform
 import sys
 import threading
+from typing import cast
 
 from nidaqmx.errors import Error
 
 
 class DaqNotFoundError(Error):
     pass
 
@@ -21,105 +22,62 @@
 
 
 class c_bool32(ctypes.c_uint):
     """
     Specifies a custom ctypes data type to represent 32-bit booleans.
     """
 
+    # typeshed specifies that _SimpleCData[_T].value is an instance variable with type _T, so
+    # accessing it with the descriptor protocol via its class results in "error: Access to generic
+    # instance variables via class is ambiguous".
+
     def _getter(self):
-        return bool(ctypes.c_uint.value.__get__(self))
+        return bool(ctypes.c_uint.value.__get__(self))  # type: ignore
 
     def _setter(self, val):
-        ctypes.c_uint.value.__set__(self, int(val))
+        ctypes.c_uint.value.__set__(self, int(val))  # type: ignore
 
-    value = property(_getter, _setter)
+    value: bool = cast(bool, property(_getter, _setter))
 
     del _getter, _setter
 
 
 class CtypesByteString:
     """
     Custom argtype that automatically converts unicode strings to ASCII
     strings in Python 3.
     """
-    def from_param(self, param):
+    @classmethod
+    def from_param(cls, param):
         if isinstance(param, str):
             param = param.encode('ascii')
         return ctypes.c_char_p(param)
 
 
-ctypes_byte_str = CtypesByteString()
+ctypes_byte_str = CtypesByteString
 
 
 def wrapped_ndpointer(*args, **kwargs):
     """
     Specifies an ndpointer type that wraps numpy.ctypeslib.ndpointer and
     allows a value of None to be passed to an argument of that type.
 
     Taken from http://stackoverflow.com/questions/32120178
     """
-    if sys.version_info < (3,):
-        if 'flags' in kwargs:
-            kwargs['flags'] = tuple(
-                f.encode('ascii') for f in kwargs['flags'])
-
     base = ndpointer(*args, **kwargs)
 
     def from_param(cls, obj):
         if obj is None:
             return obj
         return base.from_param(obj)
 
     return type(base.__name__, (base,),
                 {'from_param': classmethod(from_param)})
 
 
-def enum_bitfield_to_list(bitfield_value, bitfield_enum_type,
-                          actual_enum_type):
-    """
-    Converts a bitfield value to a list of enums.
-
-    Args:
-        bitfield_value (int): Specifies the value of the bitfield.
-        bitfield_enum_type (enum.Enum): Specifies the bitfield enum type
-            from which to mask and extract the enum values.
-        actual_enum_type (enum.Enum): Specifies the actual enum type.
-    Returns:
-        List[enum.Enum]: Indicates the converted list of enums.
-    """
-    supported_values = []
-    for bitfield_mask in bitfield_enum_type:
-        if bitfield_value & bitfield_mask.value:
-            enum_value = next(
-                e for e in actual_enum_type if e.name == bitfield_mask.name)
-            supported_values.append(enum_value)
-
-    return supported_values
-
-
-def enum_list_to_bitfield(enum_list, bitfield_enum_type):
-    """
-    Converts a list of enums to a bitfield value.
-
-    Args:
-        enum_list (List[enum.Enum]): Specifies the list of enums.
-        bitfield_enum_type (enum.Enum): Specifies the bitfield enum type
-            from which to mask and extract the enum values.
-    Returns:
-        int: Indicates the value of the bitfield.
-    """
-    bitfield_value = 0
-    for enum_value in enum_list:
-        bitfield_mask = next(
-            b for b in bitfield_enum_type if b.name == enum_value.name)
-        bitfield_value |= bitfield_mask.value
-
-    return bitfield_value
-
-
 class DaqFunctionImporter:
     """
     Wraps the function getter function of a ctypes library.
 
     Allows the NI-DAQmx Python API to fail elegantly if a function is not
     supported in the current version of the API.
     """
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ai_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ai_channel_collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
 import numpy
 
-from nidaqmx._lib import (
-    lib_importer, wrapped_ndpointer, ctypes_byte_str, c_bool32)
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.ai_channel import AIChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     ACExcitWireMode, AccelChargeSensitivityUnits, AccelSensitivityUnits,
     AccelUnits, AngleUnits, BridgeConfiguration, BridgeElectricalUnits,
     BridgePhysicalUnits, BridgeUnits, CJCSource, ChargeUnits,
@@ -24,16 +20,19 @@
     VelocityUnits, VoltageUnits)
 
 
 class AIChannelCollection(ChannelCollection):
     """
     Contains the collection of analog input channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.ai_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, physical_channel, name_to_assign_to_channel=''):
         """
         Creates and returns an AIChannel object.
 
         Args:
             physical_channel (str): Specifies the names of the physical
@@ -52,15 +51,15 @@
                 name = '{}0:{}'.format(
                     name_to_assign_to_channel, num_channels-1)
             else:
                 name = name_to_assign_to_channel
         else:
             name = physical_channel
 
-        return AIChannel(self._handle, name)
+        return AIChannel(self._handle, name, self._interpreter)
 
     def add_ai_accel_4_wire_dc_voltage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=AccelUnits.G, sensitivity=1000.0,
             sensitivity_units=AccelSensitivityUnits.MILLIVOLTS_PER_G,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -115,31 +114,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIAccel4WireDCVoltageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double, c_bool32,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_accel4_wire_dc_voltage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, voltage_excit_source.value,
             voltage_excit_val, use_excit_for_scaling, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_accel_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=AccelUnits.G, sensitivity=1000.0,
@@ -187,31 +175,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIAccelChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_accel_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, current_excit_source.value,
             current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_accel_charge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=AccelUnits.G, sensitivity=100.0,
@@ -253,29 +230,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIAccelChargeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_accel_charge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_bridge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.002, max_val=0.002, units=BridgeUnits.VOLTS_PER_VOLT,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -321,30 +288,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIBridgeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_bridge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
             nominal_bridge_resistance, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_charge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT,
             min_val=-0.000000001, max_val=0.000000001,
@@ -378,28 +335,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIChargeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_charge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_current_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-0.01,
             max_val=0.01, units=CurrentUnits.AMPS,
@@ -443,30 +391,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAICurrentChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_current_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             shunt_resistor_loc.value, ext_shunt_resistor_val,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_current_rms_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-0.01,
             max_val=0.01, units=CurrentUnits.AMPS,
@@ -511,30 +449,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAICurrentRMSChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_current_rms_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             shunt_resistor_loc.value, ext_shunt_resistor_val,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_force_bridge_polynomial_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=ForceUnits.POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -610,37 +538,21 @@
 
         if reverse_coeffs is None:
             reverse_coeffs = []
 
         forward_coeffs = numpy.float64(forward_coeffs)
         reverse_coeffs = numpy.float64(reverse_coeffs)
 
-        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgePolynomialChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_force_bridge_polynomial_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, forward_coeffs, len(forward_coeffs),
-            reverse_coeffs, len(reverse_coeffs), electrical_units.value,
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, forward_coeffs, reverse_coeffs,
+            electrical_units.value, physical_units.value, custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_force_bridge_table_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=ForceUnits.POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -716,37 +628,22 @@
 
         if physical_vals is None:
             physical_vals = []
 
         electrical_vals = numpy.float64(electrical_vals)
         physical_vals = numpy.float64(physical_vals)
 
-        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgeTableChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_force_bridge_table_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, electrical_vals, len(electrical_vals),
-            electrical_units.value, physical_vals, len(physical_vals),
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, electrical_vals,
+            electrical_units.value, physical_vals, physical_units.value,
+            custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_force_bridge_two_point_lin_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=ForceUnits.POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -816,34 +713,22 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgeTwoPointLinChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_force_bridge_two_point_lin_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
             nominal_bridge_resistance, first_electrical_val,
             second_electrical_val, electrical_units.value, first_physical_val,
             second_physical_val, physical_units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_force_iepe_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-2000.0,
             max_val=2000.0, units=ForceUnits.NEWTONS, sensitivity=2.25,
@@ -891,31 +776,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIForceIEPEChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_force_iepe_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, current_excit_source.value,
             current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_freq_voltage_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=1,
             max_val=100, units=FrequencyUnits.HZ, threshold_level=0.0,
             hysteresis=0.0, custom_scale_name=""):
@@ -958,29 +832,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIFreqVoltageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_freq_voltage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, threshold_level, hysteresis,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_microphone_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT,
             units=SoundPressureUnits.PA, mic_sensitivity=10.0,
@@ -1024,30 +888,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIMicrophoneChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_microphone_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, units.value, mic_sensitivity,
             max_snd_press_level, current_excit_source.value,
             current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pos_eddy_curr_prox_probe_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=0.00254, units=LengthUnits.METERS, sensitivity=200.0,
             sensitivity_units=EddyCurrentProxProbeSensitivityUnits.MILLIVOLTS_PER_MIL,
@@ -1085,29 +939,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIPosEddyCurrProxProbeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pos_eddy_curr_prox_probe_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pos_lvdt_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.1, max_val=0.1, units=LengthUnits.METERS,
             sensitivity=50.0,
@@ -1162,32 +1006,21 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIPosLVDTChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pos_lvdt_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, voltage_excit_source.value,
             voltage_excit_val, voltage_excit_freq, ac_excit_wire_mode.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pos_rvdt_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-70.0, max_val=70.0, units=AngleUnits.DEGREES,
             sensitivity=50.0,
@@ -1242,32 +1075,21 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIPosRVDTChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pos_rvdt_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, voltage_excit_source.value,
             voltage_excit_val, voltage_excit_freq, ac_excit_wire_mode.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_power_chan(
             self, physical_channel, voltage_setpoint, current_setpoint,
             output_enable, name_to_assign_to_channel=""):
         """
@@ -1290,27 +1112,18 @@
                 uses the physical channel name as the virtual channel
                 name.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIPowerChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        c_bool32]
 
-        error_code = cfunc(
-            self._handle, physical_channel, name_to_assign_to_channel,
-            voltage_setpoint, current_setpoint, output_enable)
-        check_for_error(error_code)
+        self._interpreter.create_ai_power_chan(
+            self._handle, physical_channel, voltage_setpoint,
+            current_setpoint, output_enable, name_to_assign_to_channel)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pressure_bridge_polynomial_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0,
             units=PressureUnits.POUNDS_PER_SQ_INCH,
@@ -1388,37 +1201,21 @@
 
         if reverse_coeffs is None:
             reverse_coeffs = []
 
         forward_coeffs = numpy.float64(forward_coeffs)
         reverse_coeffs = numpy.float64(reverse_coeffs)
 
-        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgePolynomialChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pressure_bridge_polynomial_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, forward_coeffs, len(forward_coeffs),
-            reverse_coeffs, len(reverse_coeffs), electrical_units.value,
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, forward_coeffs, reverse_coeffs,
+            electrical_units.value, physical_units.value, custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pressure_bridge_table_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0,
             units=PressureUnits.POUNDS_PER_SQ_INCH,
@@ -1496,37 +1293,22 @@
 
         if physical_vals is None:
             physical_vals = []
 
         electrical_vals = numpy.float64(electrical_vals)
         physical_vals = numpy.float64(physical_vals)
 
-        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgeTableChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pressure_bridge_table_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, electrical_vals, len(electrical_vals),
-            electrical_units.value, physical_vals, len(physical_vals),
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, electrical_vals,
+            electrical_units.value, physical_vals, physical_units.value,
+            custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_pressure_bridge_two_point_lin_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0,
             units=PressureUnits.POUNDS_PER_SQ_INCH,
@@ -1598,34 +1380,22 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgeTwoPointLinChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_pressure_bridge_two_point_lin_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
             nominal_bridge_resistance, first_electrical_val,
             second_electrical_val, electrical_units.value, first_physical_val,
             second_physical_val, physical_units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_resistance_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=100.0, max_val=1000.0, units=ResistanceUnits.OHMS,
             resistance_config=ResistanceConfiguration.TWO_WIRE,
@@ -1665,29 +1435,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIResistanceChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_resistance_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             current_excit_source.value, current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_rosette_strain_gage_chan(
             self, physical_channel, rosette_type, gage_orientation,
             rosette_meas_types, name_to_assign_to_channel="", min_val=-0.001,
             max_val=0.001,
@@ -1745,34 +1505,21 @@
             Indicates the newly created channel object.
         """
         if rosette_meas_types is None:
             rosette_meas_types = []
 
         rosette_meas_types = numpy.int32(rosette_meas_types)
 
-        cfunc = lib_importer.windll.DAQmxCreateAIRosetteStrainGageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.int32, flags=('C','W')),
-                        ctypes.c_uint, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
-            self._handle, physical_channel, name_to_assign_to_channel,
-            min_val, max_val, rosette_type.value, gage_orientation,
-            rosette_meas_types, len(rosette_meas_types), strain_config.value,
-            voltage_excit_source.value, voltage_excit_val, gage_factor,
-            nominal_gage_resistance, poisson_ratio, lead_wire_resistance)
-        check_for_error(error_code)
+        self._interpreter.create_ai_rosette_strain_gage_chan(
+            self._handle, physical_channel, rosette_type.value,
+            gage_orientation, rosette_meas_types, name_to_assign_to_channel,
+            min_val, max_val, strain_config.value, voltage_excit_source.value,
+            voltage_excit_val, gage_factor, nominal_gage_resistance,
+            poisson_ratio, lead_wire_resistance)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_rtd_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             rtd_type=RTDType.PT_3750,
@@ -1814,30 +1561,20 @@
                 requires this value. Refer to the sensor documentation
                 to determine this value.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIRTDChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_int, ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_airtd_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, rtd_type.value,
             resistance_config.value, current_excit_source.value,
             current_excit_val, r_0)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_strain_gage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.001, max_val=0.001, units=StrainUnits.STRAIN,
             strain_config=StrainGageBridgeType.FULL_BRIDGE_I,
@@ -1891,33 +1628,21 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIStrainGageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_strain_gage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, strain_config.value,
             voltage_excit_source.value, voltage_excit_val, gage_factor,
             initial_bridge_voltage, nominal_gage_resistance, poisson_ratio,
             lead_wire_resistance, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_temp_built_in_sensor_chan(
             self, physical_channel, name_to_assign_to_channel="",
             units=TemperatureUnits.DEG_C):
         """
@@ -1939,26 +1664,18 @@
                 Specifies the units to use to return temperature
                 measurements.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAITempBuiltInSensorChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_temp_built_in_sensor_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             units.value)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_thrmcpl_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             thermocouple_type=ThermocoupleType.J,
@@ -1998,29 +1715,19 @@
                 acquires the temperature of the thermocouple cold-
                 junction if you set **cjc_source** to **CHANNEL**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIThrmcplChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_thrmcpl_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, thermocouple_type.value,
             cjc_source.value, cjc_val, cjc_channel)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_thrmstr_chan_iex(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             resistance_config=ResistanceConfiguration.FOUR_WIRE,
@@ -2067,30 +1774,19 @@
                 Steinhart-Hart thermistor equation. Refer to the sensor
                 documentation to determine values for these constants.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIThrmstrChanIex
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_thrmstr_chan_iex(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             current_excit_source.value, current_excit_val, a, b, c)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_thrmstr_chan_vex(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             resistance_config=ResistanceConfiguration.FOUR_WIRE,
@@ -2140,30 +1836,19 @@
             r_1 (Optional[float]): Specifies in ohms the value of the
                 reference resistor.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIThrmstrChanVex
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_thrmstr_chan_vex(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             voltage_excit_source.value, voltage_excit_val, a, b, c, r_1)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_torque_bridge_polynomial_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=TorqueUnits.INCH_POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -2240,37 +1925,21 @@
 
         if reverse_coeffs is None:
             reverse_coeffs = []
 
         forward_coeffs = numpy.float64(forward_coeffs)
         reverse_coeffs = numpy.float64(reverse_coeffs)
 
-        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgePolynomialChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_torque_bridge_polynomial_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, forward_coeffs, len(forward_coeffs),
-            reverse_coeffs, len(reverse_coeffs), electrical_units.value,
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, forward_coeffs, reverse_coeffs,
+            electrical_units.value, physical_units.value, custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_torque_bridge_table_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=TorqueUnits.INCH_POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -2347,37 +2016,22 @@
 
         if physical_vals is None:
             physical_vals = []
 
         electrical_vals = numpy.float64(electrical_vals)
         physical_vals = numpy.float64(physical_vals)
 
-        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgeTableChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_torque_bridge_table_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
-            nominal_bridge_resistance, electrical_vals, len(electrical_vals),
-            electrical_units.value, physical_vals, len(physical_vals),
-            physical_units.value, custom_scale_name)
-        check_for_error(error_code)
+            nominal_bridge_resistance, electrical_vals,
+            electrical_units.value, physical_vals, physical_units.value,
+            custom_scale_name)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_torque_bridge_two_point_lin_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=TorqueUnits.INCH_POUNDS,
             bridge_config=BridgeConfiguration.FULL_BRIDGE,
@@ -2448,34 +2102,22 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgeTwoPointLinChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_torque_bridge_two_point_lin_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, bridge_config.value,
             voltage_excit_source.value, voltage_excit_val,
             nominal_bridge_resistance, first_electrical_val,
             second_electrical_val, electrical_units.value, first_physical_val,
             second_physical_val, physical_units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_velocity_iepe_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-50.0,
             max_val=50.0, units=VelocityUnits.INCHES_PER_SECOND,
@@ -2524,31 +2166,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIVelocityIEPEChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_velocity_iepe_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value, sensitivity,
             sensitivity_units.value, current_excit_source.value,
             current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_voltage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=VoltageUnits.VOLTS, custom_scale_name=""):
@@ -2583,28 +2214,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIVoltageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_voltage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_voltage_chan_with_excit(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-10.0,
             max_val=10.0, units=VoltageUnits.VOLTS,
@@ -2656,31 +2278,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIVoltageChanWithExcit
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_int, ctypes.c_double, c_bool32,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_voltage_chan_with_excit(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             bridge_config.value, voltage_excit_source.value,
             voltage_excit_val, use_excit_for_scaling, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ai_voltage_rms_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=VoltageUnits.VOLTS, custom_scale_name=""):
@@ -2713,28 +2324,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAIVoltageRMSChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ai_voltage_rms_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_accel_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=AccelUnits.G,
@@ -2776,29 +2378,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIAccelChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_accel_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             current_excit_source.value, current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_bridge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.002, max_val=0.002, units=TEDSUnits.FROM_TEDS,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -2838,29 +2430,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIBridgeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_bridge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_current_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-0.01,
             max_val=0.01, units=TEDSUnits.FROM_TEDS,
@@ -2905,30 +2487,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAICurrentChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_current_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             shunt_resistor_loc.value, ext_shunt_resistor_val,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_force_bridge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=ForceUnits.POUNDS,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -2968,29 +2540,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIForceBridgeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_force_bridge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_force_iepe_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-2000.0,
             max_val=2000.0, units=ForceUnits.NEWTONS,
@@ -3032,29 +2594,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIForceIEPEChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_force_iepe_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             current_excit_source.value, current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_microphone_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT,
             units=SoundPressureUnits.PA, max_snd_press_level=100.0,
@@ -3098,29 +2650,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIMicrophoneChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_microphone_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, units.value, max_snd_press_level,
             current_excit_source.value, current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_pos_lvdt_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.1, max_val=0.1, units=LengthUnits.METERS,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -3169,30 +2711,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPosLVDTChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_pos_lvdt_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, voltage_excit_freq, ac_excit_wire_mode.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_pos_rvdt_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-70.0, max_val=70.0, units=AngleUnits.DEGREES,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -3241,30 +2773,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPosRVDTChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_pos_rvdt_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, voltage_excit_freq, ac_excit_wire_mode.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_pressure_bridge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0,
             units=PressureUnits.POUNDS_PER_SQ_INCH,
@@ -3305,29 +2827,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPressureBridgeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_pressure_bridge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_resistance_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=100.0, max_val=1000.0, units=TEDSUnits.FROM_TEDS,
             resistance_config=ResistanceConfiguration.TWO_WIRE,
@@ -3367,29 +2879,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIResistanceChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_resistance_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             current_excit_source.value, current_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_rtd_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             resistance_config=ResistanceConfiguration.TWO_WIRE,
@@ -3426,29 +2928,19 @@
                 the amount of excitation to supply to the sensor. Refer
                 to the sensor documentation to determine this value.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIRTDChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsairtd_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             current_excit_source.value, current_excit_val)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_strain_gage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-0.001, max_val=0.001, units=StrainUnits.STRAIN,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -3491,30 +2983,20 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIStrainGageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_strain_gage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, initial_bridge_voltage, lead_wire_resistance,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_thrmcpl_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             cjc_source=CJCSource.CONSTANT_USER_VALUE, cjc_val=25.0,
@@ -3550,29 +3032,19 @@
                 acquires the temperature of the thermocouple cold-
                 junction if you set **cjc_source** to **CHANNEL**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmcplChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_thrmcpl_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, cjc_source.value, cjc_val,
             cjc_channel)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_thrmstr_chan_iex(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             resistance_config=ResistanceConfiguration.FOUR_WIRE,
@@ -3610,29 +3082,19 @@
                 the amount of excitation to supply to the sensor. Refer
                 to the sensor documentation to determine this value.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmstrChanIex
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_thrmstr_chan_iex(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             current_excit_source.value, current_excit_val)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_thrmstr_chan_vex(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=100.0, units=TemperatureUnits.DEG_C,
             resistance_config=ResistanceConfiguration.FOUR_WIRE,
@@ -3673,29 +3135,19 @@
             r_1 (Optional[float]): Specifies in ohms the value of the
                 reference resistor.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmstrChanVex
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_thrmstr_chan_vex(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, resistance_config.value,
             voltage_excit_source.value, voltage_excit_val, r_1)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_torque_bridge_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-100.0, max_val=100.0, units=TorqueUnits.INCH_POUNDS,
             voltage_excit_source=ExcitationSource.INTERNAL,
@@ -3735,29 +3187,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAITorqueBridgeChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_torque_bridge_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, voltage_excit_source.value,
             voltage_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_voltage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-5.0,
             max_val=5.0, units=TEDSUnits.FROM_TEDS, custom_scale_name=""):
@@ -3793,28 +3235,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIVoltageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_voltage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_teds_ai_voltage_chan_with_excit(
             self, physical_channel, name_to_assign_to_channel="",
             terminal_config=TerminalConfiguration.DEFAULT, min_val=-10.0,
             max_val=10.0, units=TEDSUnits.FROM_TEDS,
@@ -3857,25 +3290,15 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ai_channel.AIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateTEDSAIVoltageChanWithExcit
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_tedsai_voltage_chan_with_excit(
             self._handle, physical_channel, name_to_assign_to_channel,
             terminal_config.value, min_val, max_val, units.value,
             voltage_excit_source.value, voltage_excit_val, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ao_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ao_channel_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
-
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.ao_channel import AOChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     CurrentUnits, FuncGenType, VoltageUnits)
 
 
 class AOChannelCollection(ChannelCollection):
     """
     Contains the collection of analog output channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.ao_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, physical_channel, name_to_assign_to_channel=''):
         """
         Creates and returns an AOChannel object.
 
         Args:
             physical_channel (str): Specifies the names of the physical
@@ -39,15 +38,15 @@
                 name = '{}0:{}'.format(
                     name_to_assign_to_channel, num_channels-1)
             else:
                 name = name_to_assign_to_channel
         else:
             name = physical_channel
 
-        return AOChannel(self._handle, name)
+        return AOChannel(self._handle, name, self._interpreter)
 
     def add_ao_current_chan(
             self, physical_channel, name_to_assign_to_channel="", min_val=0.0,
             max_val=0.02, units=CurrentUnits.AMPS, custom_scale_name=""):
         """
         Creates channel(s) to generate current.
 
@@ -73,27 +72,18 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ao_channel.AOChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAOCurrentChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ao_current_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ao_func_gen_chan(
             self, physical_channel, name_to_assign_to_channel="",
             type=FuncGenType.SINE, freq=1000.0, amplitude=5.0, offset=0.0):
         """
@@ -120,27 +110,18 @@
             offset (Optional[float]): Is the voltage offset of the
                 waveform to generate.
         Returns:
             nidaqmx._task_modules.channels.ao_channel.AOChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAOFuncGenChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
-                        ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_ao_func_gen_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             type.value, freq, amplitude, offset)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
 
     def add_ao_voltage_chan(
             self, physical_channel, name_to_assign_to_channel="",
             min_val=-10.0, max_val=10.0, units=VoltageUnits.VOLTS,
             custom_scale_name=""):
@@ -169,23 +150,14 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ao_channel.AOChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateAOVoltageChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ao_voltage_chan(
             self._handle, physical_channel, name_to_assign_to_channel,
             min_val, max_val, units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(physical_channel, name_to_assign_to_channel)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channel_collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import ctypes
 from collections.abc import Sequence
 
-from nidaqmx._lib import lib_importer, ctypes_byte_str
 from nidaqmx._task_modules.channels.channel import Channel
-from nidaqmx.errors import (
-    check_for_error, is_string_buffer_too_small, is_array_buffer_too_small,
-    DaqError)
+from nidaqmx.errors import DaqError
 from nidaqmx.error_codes import DAQmxErrors
 from nidaqmx.utils import unflatten_channel_string, flatten_channel_string
 
 
 class ChannelCollection(Sequence):
     """
     Contains the collection of channels for a DAQmx Task.
     
     This class defines methods that implements a container object.
     """
-    def __init__(self, task_handle):
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the appropriate property, such as task.ai_channels.
+        """
         self._handle = task_handle
+        self._interpreter = interpreter
 
     def __contains__(self, item):
         channel_names = self.channel_names
 
         if isinstance(item, str):
             items = unflatten_channel_string(item)
         elif isinstance(item, Channel):
@@ -63,76 +63,51 @@
             channel_names = index
         else:
             raise DaqError(
                 'Invalid index type "{}" used to access channels.'
                 .format(type(index)), DAQmxErrors.UNKNOWN)
 
         if channel_names:
-            return Channel._factory(self._handle, channel_names)
+            return Channel._factory(self._handle, channel_names, self._interpreter)
         else:
             raise DaqError(
                 'You cannot specify an empty index when indexing channels.\n'
                 'Index used: {}'.format(index), DAQmxErrors.UNKNOWN)
 
     def __hash__(self):
-        return hash(self._handle.value)
+        return self._interpreter.hash_task_handle(self._handle)
 
     def __iter__(self):
         for channel_name in self.channel_names:
-            yield Channel._factory(self._handle, channel_name)
+            yield Channel._factory(self._handle, channel_name, self._interpreter)
 
     def __len__(self):
         return len(self.channel_names)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __reversed__(self):
         channel_names = self.channel_names
         channel_names.reverse()
 
         for channel_name in channel_names:
-            yield Channel._factory(self._handle, channel_name)
+            yield Channel._factory(self._handle, channel_name, self._interpreter)
 
     @property
     def all(self):
         """
         :class:`nidaqmx._task_modules.channels.channel.Channel`:
             Specifies a channel object that represents the entire list of 
             virtual channels on this channel collection.
         """
         # Passing a blank string means all channels.
-        return Channel._factory(self._handle, '')
+        return Channel._factory(self._handle, '', self._interpreter)
 
     @property
     def channel_names(self):
         """
         List[str]: Specifies the entire list of virtual channels on this
             channel collection.
         """
-        cfunc = lib_importer.windll.DAQmxGetTaskChannels
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.c_char_p,
-                        ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return unflatten_channel_string(val.value.decode('ascii'))
+        val = self._interpreter.get_task_attribute_string(self._handle, 0x1273)
+        return unflatten_channel_string(val)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/__init__.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/channels/ai_channel.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_library_interpreter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9466 +1,6044 @@
 # Do not edit this file; it was automatically generated.
 
 import ctypes
+import logging
+import warnings
+from typing import Optional
+
 import numpy
-import deprecation
+from typing import List
 
-from nidaqmx._lib import (
-    lib_importer, wrapped_ndpointer, ctypes_byte_str, c_bool32)
-from nidaqmx.scale import Scale
-from nidaqmx.errors import (
-    check_for_error, is_string_buffer_too_small, is_array_buffer_too_small)
-from nidaqmx._task_modules.channels.channel import Channel
-from nidaqmx.utils import unflatten_channel_string
-from nidaqmx.constants import (
-    ACExcitWireMode, ADCTimingMode, AccelChargeSensitivityUnits,
-    AccelSensitivityUnits, AccelUnits, AngleUnits, AutoZeroType,
-    BridgeConfiguration, BridgeElectricalUnits, BridgePhysicalUnits,
-    BridgeShuntCalSource, BridgeUnits, CJCSource, ChargeUnits, Coupling,
-    CurrentShuntResistorLocation, CurrentUnits, DataJustification,
-    DataTransferActiveTransferMode, DigitalWidthUnits,
-    EddyCurrentProxProbeSensitivityUnits, ExcitationDCorAC,
-    ExcitationIdleOutputBehavior, ExcitationSource,
-    ExcitationVoltageOrCurrent, FilterResponse, FilterType,
-    ForceIEPESensorSensitivityUnits, ForceUnits, FrequencyUnits, Impedance1,
-    InputDataTransferCondition, LVDTSensitivityUnits, LengthUnits,
-    PowerIdleOutputBehavior, PowerOutputState, PressureUnits, RTDType,
-    RVDTSensitivityUnits, RawDataCompressionType, ResistanceConfiguration,
-    ResistanceUnits, ResolutionType, ScaleType, Sense, SensorPowerCfg,
-    SensorPowerType, ShuntCalSelect, SoundPressureUnits, SourceSelection,
-    StrainGageBridgeType, StrainGageRosetteMeasurementType,
-    StrainGageRosetteType, StrainUnits, TemperatureUnits,
-    TerminalConfiguration, ThermocoupleType, TorqueUnits, UsageTypeAI,
-    VelocityIEPESensorSensitivityUnits, VelocityUnits, VoltageUnits)
+from nidaqmx._base_interpreter import BaseEventHandler, BaseInterpreter
+from nidaqmx._lib import lib_importer, ctypes_byte_str, c_bool32, wrapped_ndpointer
+from nidaqmx.error_codes import DAQmxErrors, DAQmxWarnings
+from nidaqmx.errors import DaqError, DaqReadError, DaqWarning, DaqWriteError
 
 
-class AIChannel(Channel):
-    """
-    Represents one or more analog input virtual channels and their properties.
-    """
-    __slots__ = []
+_logger = logging.getLogger(__name__)
 
-    def __repr__(self):
-        return f'AIChannel(name={self._name})'
 
-    @property
-    def ai_ac_excit_freq(self):
-        """
-        float: Specifies the AC excitation frequency in Hertz.
-        """
-        val = ctypes.c_double()
+class LibraryEventHandler(BaseEventHandler):
+    """Manage the lifetime of a ctypes callback method pointer.
 
-        cfunc = lib_importer.windll.DAQmxGetAIACExcitFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+    If DAQmx invokes a callback method pointer that has been garbage collected, the Python
+    interpreter will crash.
+    """
+    __slots__ = ["_callback_method_ptr"]
 
-        return val.value
+    def __init__(self, callback_method_ptr: object) -> None:
+        self._callback_method_ptr = callback_method_ptr
 
-    @ai_ac_excit_freq.setter
-    def ai_ac_excit_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIACExcitFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+    def close(self) -> None:
+        self._callback_method_ptr = None
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
 
-    @ai_ac_excit_freq.deleter
-    def ai_ac_excit_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIACExcitFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_ac_excit_sync_enable(self):
-        """
-        bool: Specifies whether to synchronize the AC excitation source
-            of the channel to that of another channel. Synchronize the
-            excitation sources of multiple channels to use multichannel
-            sensors. Set this property to False for the master channel
-            and to True for the slave channels.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIACExcitSyncEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+class LibraryInterpreter(BaseInterpreter):
+    """
+    Library C<->Python interpreter.
+    This class is responsible for interpreting the Library's C API.
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+    """
+    # Do not add per-task state to the interpreter class.
+    __slots__ = ()
 
-        return val.value
+    def __init__(self):
+        pass
 
-    @ai_ac_excit_sync_enable.setter
-    def ai_ac_excit_sync_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIACExcitSyncEnable
+    def add_cdaq_sync_connection(self, port_list):
+        cfunc = lib_importer.windll.DAQmxAddCDAQSyncConnection
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            port_list)
+        self.check_for_error(error_code)
 
-    @ai_ac_excit_sync_enable.deleter
-    def ai_ac_excit_sync_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIACExcitSyncEnable
+    def add_global_chans_to_task(self, task, channel_names):
+        cfunc = lib_importer.windll.DAQmxAddGlobalChansToTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_ac_excit_wire_mode(self):
-        """
-        :class:`nidaqmx.constants.ACExcitWireMode`: Specifies the number
-            of leads on the LVDT or RVDT. Some sensors require you to
-            tie leads together to create a four- or five- wire sensor.
-            Refer to the sensor documentation for more information.
-        """
-        val = ctypes.c_int()
+            task, channel_names)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIACExcitWireMode
+    def add_network_device(
+            self, ip_address, device_name, attempt_reservation, timeout):
+        cfunc = lib_importer.windll.DAQmxAddNetworkDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+                        ctypes_byte_str, ctypes_byte_str, c_bool32,
+                        ctypes.c_double, ctypes.c_char_p, ctypes.c_uint]
 
-        return ACExcitWireMode(val.value)
-
-    @ai_ac_excit_wire_mode.setter
-    def ai_ac_excit_wire_mode(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIACExcitWireMode
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        temp_size = 0
+        while True:
+            device_name_out = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                ip_address, device_name, attempt_reservation, timeout,
+                device_name_out, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return device_name_out.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def are_configured_cdaq_sync_ports_disconnected(
+            self, chassis_devices_ports, timeout):
+        disconnected_ports_exist = c_bool32()
 
-    @ai_ac_excit_wire_mode.deleter
-    def ai_ac_excit_wire_mode(self):
-        cfunc = lib_importer.windll.DAQmxResetAIACExcitWireMode
+        cfunc = lib_importer.windll.DAQmxAreConfiguredCDAQSyncPortsDisconnected
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double,
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            chassis_devices_ports, timeout,
+            ctypes.byref(disconnected_ports_exist))
+        self.check_for_error(error_code)
+        return disconnected_ports_exist.value
 
-    @property
-    def ai_accel_4_wire_dc_voltage_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the 4 wire DC voltage
-            acceleration sensor connected to the channel. This value is
-            the units you specify with
-            AI.Accel.4WireDCVoltage.SensitivityUnits. Refer to the
-            sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIAccel4WireDCVoltageSensitivity
+    def auto_configure_cdaq_sync_connections(
+            self, chassis_devices_ports, timeout):
+        cfunc = lib_importer.windll.DAQmxAutoConfigureCDAQSyncConnections
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            chassis_devices_ports, timeout)
+        self.check_for_error(error_code)
 
-        return val.value
+    def calculate_reverse_poly_coeff(
+            self, forward_coeffs, min_val_x, max_val_x, num_points_to_compute,
+            reverse_poly_order):
+        size = len(forward_coeffs) if reverse_poly_order < 0 else reverse_poly_order + 1
+        reverse_coeffs = numpy.zeros(size, dtype=numpy.float64)
 
-    @ai_accel_4_wire_dc_voltage_sensitivity.setter
-    def ai_accel_4_wire_dc_voltage_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAccel4WireDCVoltageSensitivity
+        cfunc = lib_importer.windll.DAQmxCalculateReversePolyCoeff
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W'))]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            forward_coeffs, len(forward_coeffs), min_val_x, max_val_x,
+            num_points_to_compute, reverse_poly_order, reverse_coeffs)
+        self.check_for_error(error_code)
+        return reverse_coeffs.tolist()
 
-    @ai_accel_4_wire_dc_voltage_sensitivity.deleter
-    def ai_accel_4_wire_dc_voltage_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccel4WireDCVoltageSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_accel_4_wire_dc_voltage_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.AccelSensitivityUnits`: Specifies the
-            units of AI.Accel.4WireDCVoltage.Sensitivity.
-        """
-        val = ctypes.c_int()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIAccel4WireDCVoltageSensitivityUnits)
+    def cfg_anlg_edge_ref_trig(
+            self, task, trigger_source, pretrigger_samples, trigger_slope,
+            trigger_level):
+        cfunc = lib_importer.windll.DAQmxCfgAnlgEdgeRefTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int, ctypes.c_double, ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return AccelSensitivityUnits(val.value)
+            task, trigger_source, trigger_slope, trigger_level,
+            pretrigger_samples)
+        self.check_for_error(error_code)
 
-    @ai_accel_4_wire_dc_voltage_sensitivity_units.setter
-    def ai_accel_4_wire_dc_voltage_sensitivity_units(self, val):
-        val = val.value
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIAccel4WireDCVoltageSensitivityUnits)
+    def cfg_anlg_edge_start_trig(
+            self, task, trigger_source, trigger_slope, trigger_level):
+        cfunc = lib_importer.windll.DAQmxCfgAnlgEdgeStartTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_accel_4_wire_dc_voltage_sensitivity_units.deleter
-    def ai_accel_4_wire_dc_voltage_sensitivity_units(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIAccel4WireDCVoltageSensitivityUnits)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+            task, trigger_source, trigger_slope, trigger_level)
+        self.check_for_error(error_code)
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+    def cfg_anlg_multi_edge_ref_trig(
+            self, task, trigger_sources, trigger_slope_array,
+            trigger_level_array, pretrigger_samples):
+        raise NotImplementedError
 
-    @property
-    def ai_accel_charge_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the charge acceleration
-            sensor connected to the channel. This value is the units you
-            specify with AI.Accel.Charge.SensitivityUnits. Refer to the
-            sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
+    def cfg_anlg_multi_edge_start_trig(
+            self, task, trigger_sources, trigger_slope_array,
+            trigger_level_array):
+        raise NotImplementedError
 
-        cfunc = lib_importer.windll.DAQmxGetAIAccelChargeSensitivity
+    def cfg_anlg_window_ref_trig(
+            self, task, trigger_source, window_top, window_bottom,
+            pretrigger_samples, trigger_when):
+        cfunc = lib_importer.windll.DAQmxCfgAnlgWindowRefTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, trigger_source, trigger_when, window_top, window_bottom,
+            pretrigger_samples)
+        self.check_for_error(error_code)
 
-    @ai_accel_charge_sensitivity.setter
-    def ai_accel_charge_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAccelChargeSensitivity
+    def cfg_anlg_window_start_trig(
+            self, task, window_top, window_bottom, trigger_source,
+            trigger_when):
+        cfunc = lib_importer.windll.DAQmxCfgAnlgWindowStartTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, trigger_source, trigger_when, window_top, window_bottom)
+        self.check_for_error(error_code)
 
-    @ai_accel_charge_sensitivity.deleter
-    def ai_accel_charge_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccelChargeSensitivity
+    def cfg_burst_handshaking_timing_export_clock(
+            self, task, sample_clk_rate, sample_clk_outp_term, sample_mode,
+            samps_per_chan, sample_clk_pulse_polarity, pause_when,
+            ready_event_active_level):
+        cfunc = lib_importer.windll.DAQmxCfgBurstHandshakingTimingExportClock
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_ulonglong, ctypes.c_double, ctypes_byte_str,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_accel_charge_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.AccelChargeSensitivityUnits`:
-            Specifies the units of AI.Accel.Charge.Sensitivity.
-        """
-        val = ctypes.c_int()
+            task, sample_mode, samps_per_chan, sample_clk_rate,
+            sample_clk_outp_term, sample_clk_pulse_polarity, pause_when,
+            ready_event_active_level)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIAccelChargeSensitivityUnits
+    def cfg_burst_handshaking_timing_import_clock(
+            self, task, sample_clk_rate, sample_clk_src, sample_mode,
+            samps_per_chan, sample_clk_active_edge, pause_when,
+            ready_event_active_level):
+        cfunc = lib_importer.windll.DAQmxCfgBurstHandshakingTimingImportClock
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_ulonglong, ctypes.c_double, ctypes_byte_str,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, sample_mode, samps_per_chan, sample_clk_rate,
+            sample_clk_src, sample_clk_active_edge, pause_when,
+            ready_event_active_level)
+        self.check_for_error(error_code)
 
-        return AccelChargeSensitivityUnits(val.value)
-
-    @ai_accel_charge_sensitivity_units.setter
-    def ai_accel_charge_sensitivity_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIAccelChargeSensitivityUnits
+    def cfg_change_detection_timing(
+            self, task, rising_edge_chan, falling_edge_chan, sample_mode,
+            samps_per_chan):
+        cfunc = lib_importer.windll.DAQmxCfgChangeDetectionTiming
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_accel_charge_sensitivity_units.deleter
-    def ai_accel_charge_sensitivity_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccelChargeSensitivityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_ulonglong]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_accel_db_ref(self):
-        """
-        float: Specifies the decibel reference level in the units of the
-            channel. When you read samples as a waveform, the decibel
-            reference level is included in the waveform attributes.
-        """
-        val = ctypes.c_double()
+            task, rising_edge_chan, falling_edge_chan, sample_mode,
+            samps_per_chan)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIAcceldBRef
+    def cfg_dig_edge_ref_trig(
+            self, task, trigger_source, pretrigger_samples, trigger_edge):
+        cfunc = lib_importer.windll.DAQmxCfgDigEdgeRefTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int, ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, trigger_source, trigger_edge, pretrigger_samples)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_accel_db_ref.setter
-    def ai_accel_db_ref(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAcceldBRef
+    def cfg_dig_edge_start_trig(self, task, trigger_source, trigger_edge):
+        cfunc = lib_importer.windll.DAQmxCfgDigEdgeStartTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_accel_db_ref.deleter
-    def ai_accel_db_ref(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAcceldBRef
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, trigger_source, trigger_edge)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_accel_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the accelerometer. This
-            value is in the units you specify with
-            **ai_accel_sensitivity_units**. Refer to the sensor
-            documentation to determine this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIAccelSensitivity
+    def cfg_dig_pattern_ref_trig(
+            self, task, trigger_source, trigger_pattern, pretrigger_samples,
+            trigger_when):
+        cfunc = lib_importer.windll.DAQmxCfgDigPatternRefTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, trigger_source, trigger_pattern, trigger_when,
+            pretrigger_samples)
+        self.check_for_error(error_code)
 
-    @ai_accel_sensitivity.setter
-    def ai_accel_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAccelSensitivity
+    def cfg_dig_pattern_start_trig(
+            self, task, trigger_source, trigger_pattern, trigger_when):
+        cfunc = lib_importer.windll.DAQmxCfgDigPatternStartTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, trigger_source, trigger_pattern, trigger_when)
+        self.check_for_error(error_code)
 
-    @ai_accel_sensitivity.deleter
-    def ai_accel_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccelSensitivity
+    def cfg_handshaking_timing(self, task, sample_mode, samps_per_chan):
+        cfunc = lib_importer.windll.DAQmxCfgHandshakingTiming
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_ulonglong]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_accel_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.AccelSensitivityUnits`: Specifies the
-            units of **ai_accel_sensitivity**.
-        """
-        val = ctypes.c_int()
+            task, sample_mode, samps_per_chan)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIAccelSensitivityUnits
+    def cfg_implicit_timing(self, task, sample_mode, samps_per_chan):
+        cfunc = lib_importer.windll.DAQmxCfgImplicitTiming
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_ulonglong]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return AccelSensitivityUnits(val.value)
+            task, sample_mode, samps_per_chan)
+        self.check_for_error(error_code)
 
-    @ai_accel_sensitivity_units.setter
-    def ai_accel_sensitivity_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIAccelSensitivityUnits
+    def cfg_pipelined_samp_clk_timing(
+            self, task, rate, source, active_edge, sample_mode,
+            samps_per_chan):
+        cfunc = lib_importer.windll.DAQmxCfgPipelinedSampClkTiming
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_ulonglong]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, source, rate, active_edge, sample_mode, samps_per_chan)
+        self.check_for_error(error_code)
 
-    @ai_accel_sensitivity_units.deleter
-    def ai_accel_sensitivity_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccelSensitivityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_accel_units(self):
-        """
-        :class:`nidaqmx.constants.AccelUnits`: Specifies the units to
-            use to return acceleration measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIAccelUnits
+    def cfg_samp_clk_timing(
+            self, task, rate, source, active_edge, sample_mode,
+            samps_per_chan):
+        cfunc = lib_importer.windll.DAQmxCfgSampClkTiming
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_ulonglong]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return AccelUnits(val.value)
+            task, source, rate, active_edge, sample_mode, samps_per_chan)
+        self.check_for_error(error_code)
 
-    @ai_accel_units.setter
-    def ai_accel_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIAccelUnits
+    def cfg_watchdog_ao_expir_states(
+            self, task, channel_names, expir_state_array, output_type_array):
+        cfunc = lib_importer.windll.DAQmxCfgWatchdogAOExpirStates
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_accel_units.deleter
-    def ai_accel_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAccelUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
+                        ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_adc_custom_timing_mode(self):
-        """
-        int: Specifies the timing mode of the ADC when
-            **ai_adc_timing_mode** is **ADCTimingMode.CUSTOM**.
-        """
-        val = ctypes.c_uint()
+            task, channel_names, expir_state_array, output_type_array,
+            len(output_type_array))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIADCCustomTimingMode
+    def cfg_watchdog_co_expir_states(
+            self, task, channel_names, expir_state_array):
+        cfunc = lib_importer.windll.DAQmxCfgWatchdogCOExpirStates
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
+                        ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, channel_names, expir_state_array, len(expir_state_array))
+        self.check_for_error(error_code)
 
-    @ai_adc_custom_timing_mode.setter
-    def ai_adc_custom_timing_mode(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIADCCustomTimingMode
+    def cfg_watchdog_do_expir_states(
+            self, task, channel_names, expir_state_array):
+        cfunc = lib_importer.windll.DAQmxCfgWatchdogDOExpirStates
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
                         ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, channel_names, expir_state_array, len(expir_state_array))
+        self.check_for_error(error_code)
 
-    @ai_adc_custom_timing_mode.deleter
-    def ai_adc_custom_timing_mode(self):
-        cfunc = lib_importer.windll.DAQmxResetAIADCCustomTimingMode
+    def clear_task(self, task):
+        cfunc = lib_importer.windll.DAQmxClearTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_adc_timing_mode(self):
-        """
-        :class:`nidaqmx.constants.ADCTimingMode`: Specifies the ADC
-            timing mode, controlling the tradeoff between speed and
-            effective resolution. Some ADC timing modes provide
-            increased powerline noise rejection. On devices that have an
-            AI Convert clock, this setting affects both the maximum and
-            default values for **ai_conv_rate**. You must use the same
-            ADC timing mode for all channels on a device, but you can
-            use different ADC timing modes for different devices in the
-            same task.
-        """
-        val = ctypes.c_int()
+            task)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIADCTimingMode
+    def clear_teds(self, physical_channel):
+        cfunc = lib_importer.windll.DAQmxClearTEDS
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ADCTimingMode(val.value)
+            physical_channel)
+        self.check_for_error(error_code)
 
-    @ai_adc_timing_mode.setter
-    def ai_adc_timing_mode(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIADCTimingMode
+    def configure_logging(
+            self, task, file_path, logging_mode, group_name, operation):
+        cfunc = lib_importer.windll.DAQmxConfigureLogging
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int, ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, file_path, logging_mode, group_name, operation)
+        self.check_for_error(error_code)
 
-    @ai_adc_timing_mode.deleter
-    def ai_adc_timing_mode(self):
-        cfunc = lib_importer.windll.DAQmxResetAIADCTimingMode
+    def configure_teds(self, physical_channel, file_path):
+        cfunc = lib_importer.windll.DAQmxConfigureTEDS
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_atten(self):
-        """
-        float: Specifies the amount of attenuation to use.
-        """
-        val = ctypes.c_double()
+            physical_channel, file_path)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIAtten
+    def connect_terms(
+            self, source_terminal, destination_terminal, signal_modifiers):
+        cfunc = lib_importer.windll.DAQmxConnectTerms
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            source_terminal, destination_terminal, signal_modifiers)
+        self.check_for_error(error_code)
 
-    @ai_atten.setter
-    def ai_atten(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAtten
+    def control_watchdog_task(self, task, action):
+        cfunc = lib_importer.windll.DAQmxControlWatchdogTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, action)
+        self.check_for_error(error_code)
 
-    @ai_atten.deleter
-    def ai_atten(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAtten
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_auto_zero_mode(self):
-        """
-        :class:`nidaqmx.constants.AutoZeroType`: Specifies how often to
-            measure ground. NI-DAQmx subtracts the measured ground
-            voltage from every sample.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIAutoZeroMode
+    def create_ai_accel4_wire_dc_voltage_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, voltage_excit_source, voltage_excit_val,
+            use_excit_for_scaling, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIAccel4WireDCVoltageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double, c_bool32,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return AutoZeroType(val.value)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, voltage_excit_source, voltage_excit_val,
+            use_excit_for_scaling, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_auto_zero_mode.setter
-    def ai_auto_zero_mode(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIAutoZeroMode
+    def create_ai_accel_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIAccelChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_auto_zero_mode.deleter
-    def ai_auto_zero_mode(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAutoZeroMode
+    def create_ai_accel_charge_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIAccelChargeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_averaging_win_size(self):
-        """
-        int: Specifies the number of samples to average while acquiring
-            data. Increasing the number of samples to average reduces
-            noise in your measurement.
-        """
-        val = ctypes.c_uint()
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIAveragingWinSize
+    def create_ai_bridge_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIBridgeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_averaging_win_size.setter
-    def ai_averaging_win_size(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIAveragingWinSize
+    def create_ai_charge_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIChargeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_averaging_win_size.deleter
-    def ai_averaging_win_size(self):
-        cfunc = lib_importer.windll.DAQmxResetAIAveragingWinSize
+    def create_ai_current_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAICurrentChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_bridge_balance_coarse_pot(self):
-        """
-        int: Specifies by how much to compensate for offset in the
-            signal. This value can be between 0 and 127.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeBalanceCoarsePot
+    def create_ai_current_rms_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAICurrentRMSChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_balance_coarse_pot.setter
-    def ai_bridge_balance_coarse_pot(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeBalanceCoarsePot
+    def create_ai_force_bridge_polynomial_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            reverse_coeffs, electrical_units, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgePolynomialChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            len(forward_coeffs), reverse_coeffs, len(reverse_coeffs),
+            electrical_units, physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_balance_coarse_pot.deleter
-    def ai_bridge_balance_coarse_pot(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeBalanceCoarsePot
+    def create_ai_force_bridge_table_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            electrical_units, physical_vals, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgeTableChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            len(electrical_vals), electrical_units, physical_vals,
+            len(physical_vals), physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_bridge_balance_fine_pot(self):
-        """
-        int: Specifies by how much to compensate for offset in the
-            signal. This value can be between 0 and 4095.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeBalanceFinePot
+    def create_ai_force_bridge_two_point_lin_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIForceBridgeTwoPointLinChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_balance_fine_pot.setter
-    def ai_bridge_balance_fine_pot(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeBalanceFinePot
+    def create_ai_force_iepe_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIForceIEPEChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_balance_fine_pot.deleter
-    def ai_bridge_balance_fine_pot(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeBalanceFinePot
+    def create_ai_freq_voltage_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, threshold_level, hysteresis, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIFreqVoltageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_cfg(self):
-        """
-        :class:`nidaqmx.constants.BridgeConfiguration`: Specifies the
-            type of Wheatstone bridge connected to the channel.
-        """
-        val = ctypes.c_int()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, threshold_level, hysteresis, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeCfg
+    def create_ai_microphone_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, units, mic_sensitivity, max_snd_press_level,
+            current_excit_source, current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIMicrophoneChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return BridgeConfiguration(val.value)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, units, mic_sensitivity, max_snd_press_level,
+            current_excit_source, current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_cfg.setter
-    def ai_bridge_cfg(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeCfg
+    def create_ai_pos_eddy_curr_prox_probe_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPosEddyCurrProxProbeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_cfg.deleter
-    def ai_bridge_cfg(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeCfg
+    def create_ai_pos_lvdt_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units,
+            voltage_excit_source, voltage_excit_val, voltage_excit_freq,
+            ac_excit_wire_mode, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPosLVDTChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_electrical_units(self):
-        """
-        :class:`nidaqmx.constants.BridgeElectricalUnits`: Specifies from
-            which electrical unit to scale data. Select  the same unit
-            that the sensor data sheet or calibration certificate uses
-            for electrical values.
-        """
-        val = ctypes.c_int()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units,
+            voltage_excit_source, voltage_excit_val, voltage_excit_freq,
+            ac_excit_wire_mode, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeElectricalUnits
+    def create_ai_pos_rvdt_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units,
+            voltage_excit_source, voltage_excit_val, voltage_excit_freq,
+            ac_excit_wire_mode, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPosRVDTChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_int,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, sensitivity, sensitivity_units,
+            voltage_excit_source, voltage_excit_val, voltage_excit_freq,
+            ac_excit_wire_mode, custom_scale_name)
+        self.check_for_error(error_code)
 
-        return BridgeElectricalUnits(val.value)
-
-    @ai_bridge_electrical_units.setter
-    def ai_bridge_electrical_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeElectricalUnits
+    def create_ai_power_chan(
+            self, task, physical_channel, voltage_setpoint, current_setpoint,
+            output_enable, name_to_assign_to_channel):
+        cfunc = lib_importer.windll.DAQmxCreateAIPowerChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        c_bool32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            voltage_setpoint, current_setpoint, output_enable)
+        self.check_for_error(error_code)
 
-    @ai_bridge_electrical_units.deleter
-    def ai_bridge_electrical_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeElectricalUnits
+    def create_ai_pressure_bridge_polynomial_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            reverse_coeffs, electrical_units, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgePolynomialChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_initial_ratio(self):
-        """
-        float: Specifies in volts per volt the ratio of output voltage
-            from the bridge to excitation voltage supplied to the bridge
-            while not under load. NI-DAQmx subtracts this value from any
-            measurements before applying scaling equations. If you set
-            **ai_bridge_initial_voltage**, NI-DAQmx coerces this
-            property  to **ai_bridge_initial_voltage** divided by
-            **ai_excit_actual_val**. If you set this property, NI-DAQmx
-            coerces **ai_bridge_initial_voltage** to the value of this
-            property times **ai_excit_actual_val**. If you set both this
-            property and **ai_bridge_initial_voltage**, and their values
-            conflict, NI-DAQmx returns an error.  To avoid this error,
-            reset one property to its default value before setting the
-            other.
-        """
-        val = ctypes.c_double()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            len(forward_coeffs), reverse_coeffs, len(reverse_coeffs),
+            electrical_units, physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeInitialRatio
+    def create_ai_pressure_bridge_table_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            electrical_units, physical_vals, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgeTableChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            len(electrical_vals), electrical_units, physical_vals,
+            len(physical_vals), physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_initial_ratio.setter
-    def ai_bridge_initial_ratio(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeInitialRatio
+    def create_ai_pressure_bridge_two_point_lin_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIPressureBridgeTwoPointLinChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_initial_ratio.deleter
-    def ai_bridge_initial_ratio(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeInitialRatio
+    def create_ai_resistance_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIResistanceChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_initial_voltage(self):
-        """
-        float: Specifies in volts the output voltage of the bridge while
-            not under load. NI-DAQmx subtracts this value from any
-            measurements before applying scaling equations.  If you set
-            **ai_bridge_initial_ratio**, NI-DAQmx coerces this property
-            to **ai_bridge_initial_ratio** times
-            **ai_excit_actual_val**. This property is set by DAQmx
-            Perform Bridge Offset Nulling Calibration. If you set this
-            property, NI-DAQmx coerces **ai_bridge_initial_ratio** to
-            the value of this property divided by
-            **ai_excit_actual_val**. If you set both this property and
-            **ai_bridge_initial_ratio**, and their values conflict, NI-
-            DAQmx returns an error. To avoid this error, reset one
-            property to its default value before setting the other.
-        """
-        val = ctypes.c_double()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeInitialVoltage
+    def create_ai_rosette_strain_gage_chan(
+            self, task, physical_channel, rosette_type, gage_orientation,
+            rosette_meas_types, name_to_assign_to_channel, min_val, max_val,
+            strain_config, voltage_excit_source, voltage_excit_val,
+            gage_factor, nominal_gage_resistance, poisson_ratio,
+            lead_wire_resistance):
+        cfunc = lib_importer.windll.DAQmxCreateAIRosetteStrainGageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, rosette_type, gage_orientation, rosette_meas_types,
+            len(rosette_meas_types), strain_config, voltage_excit_source,
+            voltage_excit_val, gage_factor, nominal_gage_resistance,
+            poisson_ratio, lead_wire_resistance)
+        self.check_for_error(error_code)
 
-    @ai_bridge_initial_voltage.setter
-    def ai_bridge_initial_voltage(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeInitialVoltage
+    def create_ai_strain_gage_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, strain_config, voltage_excit_source,
+            voltage_excit_val, gage_factor, initial_bridge_voltage,
+            nominal_gage_resistance, poisson_ratio, lead_wire_resistance,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIStrainGageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, strain_config, voltage_excit_source,
+            voltage_excit_val, gage_factor, initial_bridge_voltage,
+            nominal_gage_resistance, poisson_ratio, lead_wire_resistance,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_initial_voltage.deleter
-    def ai_bridge_initial_voltage(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeInitialVoltage
+    def create_ai_temp_built_in_sensor_chan(
+            self, task, physical_channel, name_to_assign_to_channel, units):
+        cfunc = lib_importer.windll.DAQmxCreateAITempBuiltInSensorChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_nom_resistance(self):
-        """
-        float: Specifies in ohms the resistance of the bridge while not
-            under load.
-        """
-        val = ctypes.c_double()
+            task, physical_channel, name_to_assign_to_channel, units)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeNomResistance
+    def create_ai_thrmcpl_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, thermocouple_type, cjc_source, cjc_val,
+            cjc_channel):
+        cfunc = lib_importer.windll.DAQmxCreateAIThrmcplChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, thermocouple_type, cjc_source, cjc_val,
+            cjc_channel)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_bridge_nom_resistance.setter
-    def ai_bridge_nom_resistance(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeNomResistance
+    def create_ai_thrmstr_chan_iex(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, a, b, c):
+        cfunc = lib_importer.windll.DAQmxCreateAIThrmstrChanIex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
                         ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, a, b, c)
+        self.check_for_error(error_code)
 
-    @ai_bridge_nom_resistance.deleter
-    def ai_bridge_nom_resistance(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeNomResistance
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_physical_units(self):
-        """
-        :class:`nidaqmx.constants.BridgePhysicalUnits`: Specifies to
-            which physical unit to scale electrical data. Select the
-            same unit that the sensor data sheet or calibration
-            certificate uses for physical values.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIBridgePhysicalUnits
+    def create_ai_thrmstr_chan_vex(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, voltage_excit_source,
+            voltage_excit_val, a, b, c, r_1):
+        cfunc = lib_importer.windll.DAQmxCreateAIThrmstrChanVex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return BridgePhysicalUnits(val.value)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, voltage_excit_source,
+            voltage_excit_val, a, b, c, r_1)
+        self.check_for_error(error_code)
 
-    @ai_bridge_physical_units.setter
-    def ai_bridge_physical_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgePhysicalUnits
+    def create_ai_torque_bridge_polynomial_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            reverse_coeffs, electrical_units, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgePolynomialChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_bridge_physical_units.deleter
-    def ai_bridge_physical_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgePhysicalUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_poly_forward_coeff(self):
-        """
-        List[float]: Specifies an list of coefficients for the
-            polynomial that converts electrical values to physical
-            values. Each element of the list corresponds to a term of
-            the equation. For example, if index three of the list is 9,
-            the fourth term of the equation is 9x^3.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIBridgePolyForwardCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, forward_coeffs,
+            len(forward_coeffs), reverse_coeffs, len(reverse_coeffs),
+            electrical_units, physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @ai_bridge_poly_forward_coeff.setter
-    def ai_bridge_poly_forward_coeff(self, val):
-        val = numpy.float64(val)
-        cfunc = lib_importer.windll.DAQmxSetAIBridgePolyForwardCoeff
+    def create_ai_torque_bridge_table_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            electrical_units, physical_vals, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgeTableChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val, len(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance, electrical_vals,
+            len(electrical_vals), electrical_units, physical_vals,
+            len(physical_vals), physical_units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_poly_forward_coeff.deleter
-    def ai_bridge_poly_forward_coeff(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgePolyForwardCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_poly_reverse_coeff(self):
-        """
-        List[float]: Specifies an list of coefficients for the
-            polynomial that converts physical values to electrical
-            values. Each element of the list corresponds to a term of
-            the equation. For example, if index three of the list is 9,
-            the fourth term of the equation is 9x^3.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIBridgePolyReverseCoeff
+    def create_ai_torque_bridge_two_point_lin_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAITorqueBridgeTwoPointLinChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @ai_bridge_poly_reverse_coeff.setter
-    def ai_bridge_poly_reverse_coeff(self, val):
-        val = numpy.float64(val)
-        cfunc = lib_importer.windll.DAQmxSetAIBridgePolyReverseCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val, len(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, bridge_config, voltage_excit_source,
+            voltage_excit_val, nominal_bridge_resistance,
+            first_electrical_val, second_electrical_val, electrical_units,
+            first_physical_val, second_physical_val, physical_units,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_poly_reverse_coeff.deleter
-    def ai_bridge_poly_reverse_coeff(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgePolyReverseCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_scale_type(self):
-        """
-        :class:`nidaqmx.constants.ScaleType`: Specifies the scaling type
-            to use when scaling electrical values from the sensor to
-            physical units.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeScaleType
+    def create_ai_velocity_iepe_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIVelocityIEPEChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ScaleType(val.value)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, sensitivity,
+            sensitivity_units, current_excit_source, current_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_scale_type.setter
-    def ai_bridge_scale_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeScaleType
+    def create_ai_voltage_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIVoltageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_scale_type.deleter
-    def ai_bridge_scale_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeScaleType
+    def create_ai_voltage_chan_with_excit(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, bridge_config,
+            voltage_excit_source, voltage_excit_val, use_excit_for_scaling,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIVoltageChanWithExcit
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_int, ctypes.c_double, c_bool32,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_enable(self):
-        """
-        bool: Specifies whether to enable a shunt calibration switch.
-            Use **ai_bridge_shunt_cal_select** to select the switch(es)
-            to enable.
-        """
-        val = c_bool32()
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, bridge_config,
+            voltage_excit_source, voltage_excit_val, use_excit_for_scaling,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeShuntCalEnable
+    def create_ai_voltage_rms_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAIVoltageRMSChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_bridge_shunt_cal_enable.setter
-    def ai_bridge_shunt_cal_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeShuntCalEnable
+    def create_airtd_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, rtd_type, resistance_config, current_excit_source,
+            current_excit_val, r_0):
+        cfunc = lib_importer.windll.DAQmxCreateAIRTDChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_int, ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, rtd_type, resistance_config, current_excit_source,
+            current_excit_val, r_0)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_enable.deleter
-    def ai_bridge_shunt_cal_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeShuntCalEnable
+    def create_ao_current_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAOCurrentChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_gain_adjust(self):
-        """
-        float: Specifies the result of a shunt calibration. This
-            property is set by DAQmx Perform Shunt Calibration. NI-DAQmx
-            multiplies data read from the channel by the value of this
-            property. This value should be close to 1.0.
-        """
-        val = ctypes.c_double()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeShuntCalGainAdjust
+    def create_ao_func_gen_chan(
+            self, task, physical_channel, name_to_assign_to_channel, type,
+            freq, amplitude, offset):
+        cfunc = lib_importer.windll.DAQmxCreateAOFuncGenChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, type, freq,
+            amplitude, offset)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_bridge_shunt_cal_gain_adjust.setter
-    def ai_bridge_shunt_cal_gain_adjust(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeShuntCalGainAdjust
+    def create_ao_voltage_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateAOVoltageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_gain_adjust.deleter
-    def ai_bridge_shunt_cal_gain_adjust(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeShuntCalGainAdjust
+    def create_ci_ang_encoder_chan(
+            self, task, counter, name_to_assign_to_channel, decoding_type,
+            zidx_enable, zidx_val, zidx_phase, units, pulses_per_rev,
+            initial_angle, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIAngEncoderChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_uint, ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_select(self):
-        """
-        :class:`nidaqmx.constants.ShuntCalSelect`: Specifies which shunt
-            calibration switch(es) to enable.  Use
-            **ai_bridge_shunt_cal_enable** to enable the switch(es) you
-            specify with this property.
-        """
-        val = ctypes.c_int()
+            task, counter, name_to_assign_to_channel, decoding_type,
+            zidx_enable, zidx_val, zidx_phase, units, pulses_per_rev,
+            initial_angle, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeShuntCalSelect
+    def create_ci_ang_velocity_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            decoding_type, units, pulses_per_rev, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIAngVelocityChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_uint,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ShuntCalSelect(val.value)
+            task, counter, name_to_assign_to_channel, min_val, max_val,
+            decoding_type, units, pulses_per_rev, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_select.setter
-    def ai_bridge_shunt_cal_select(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeShuntCalSelect
+    def create_ci_count_edges_chan(
+            self, task, counter, name_to_assign_to_channel, edge,
+            initial_count, count_direction):
+        cfunc = lib_importer.windll.DAQmxCreateCICountEdgesChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_uint,
                         ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_bridge_shunt_cal_select.deleter
-    def ai_bridge_shunt_cal_select(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeShuntCalSelect
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_shunt_cal_a_actual_resistance(self):
-        """
-        float: Specifies in ohms the actual value of the internal shunt
-            calibration A resistor.
-        """
-        val = ctypes.c_double()
+            task, counter, name_to_assign_to_channel, edge, initial_count,
+            count_direction)
+        self.check_for_error(error_code)
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeShuntCalShuntCalAActualResistance)
+    def create_ci_duty_cycle_chan(
+            self, task, counter, name_to_assign_to_channel, min_freq,
+            max_freq, edge, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIDutyCycleChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, min_freq, max_freq,
+            edge, custom_scale_name)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_bridge_shunt_cal_shunt_cal_a_actual_resistance.setter
-    def ai_bridge_shunt_cal_shunt_cal_a_actual_resistance(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeShuntCalShuntCalAActualResistance)
+    def create_ci_freq_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units, edge, meas_method, meas_time, divisor, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIFreqChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_uint, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, min_val, max_val, units,
+            edge, meas_method, meas_time, divisor, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_a_actual_resistance.deleter
-    def ai_bridge_shunt_cal_shunt_cal_a_actual_resistance(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeShuntCalShuntCalAActualResistance)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_shunt_cal_a_resistance(self):
-        """
-        float: Specifies in ohms the desired value of the internal shunt
-            calibration A resistor.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeShuntCalShuntCalAResistance)
+    def create_ci_lin_encoder_chan(
+            self, task, counter, name_to_assign_to_channel, decoding_type,
+            zidx_enable, zidx_val, zidx_phase, units, dist_per_pulse,
+            initial_pos, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCILinEncoderChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, counter, name_to_assign_to_channel, decoding_type,
+            zidx_enable, zidx_val, zidx_phase, units, dist_per_pulse,
+            initial_pos, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_a_resistance.setter
-    def ai_bridge_shunt_cal_shunt_cal_a_resistance(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeShuntCalShuntCalAResistance)
+    def create_ci_lin_velocity_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            decoding_type, units, dist_per_pulse, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCILinVelocityChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_bridge_shunt_cal_shunt_cal_a_resistance.deleter
-    def ai_bridge_shunt_cal_shunt_cal_a_resistance(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeShuntCalShuntCalAResistance)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_shunt_cal_a_src(self):
-        """
-        :class:`nidaqmx.constants.BridgeShuntCalSource`: Specifies
-            whether to use internal or external shunt when Shunt Cal A
-            is selected.
-        """
-        val = ctypes.c_int()
+            task, counter, name_to_assign_to_channel, min_val, max_val,
+            decoding_type, units, dist_per_pulse, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeShuntCalShuntCalASrc
+    def create_ci_period_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units, edge, meas_method, meas_time, divisor, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIPeriodChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_uint, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return BridgeShuntCalSource(val.value)
+            task, counter, name_to_assign_to_channel, min_val, max_val, units,
+            edge, meas_method, meas_time, divisor, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_a_src.setter
-    def ai_bridge_shunt_cal_shunt_cal_a_src(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeShuntCalShuntCalASrc
+    def create_ci_pulse_chan_freq(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units):
+        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanFreq
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
                         ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_bridge_shunt_cal_shunt_cal_a_src.deleter
-    def ai_bridge_shunt_cal_shunt_cal_a_src(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeShuntCalShuntCalASrc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, min_val, max_val, units)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_bridge_shunt_cal_shunt_cal_b_actual_resistance(self):
-        """
-        float: Specifies in ohms the actual value of the internal shunt
-            calibration B resistor.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeShuntCalShuntCalBActualResistance)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_bridge_shunt_cal_shunt_cal_b_actual_resistance.setter
-    def ai_bridge_shunt_cal_shunt_cal_b_actual_resistance(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeShuntCalShuntCalBActualResistance)
+    def create_ci_pulse_chan_ticks(
+            self, task, counter, name_to_assign_to_channel, source_terminal,
+            min_val, max_val):
+        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanTicks
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes_byte_str, ctypes.c_double,
                         ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, source_terminal,
+            min_val, max_val)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_b_actual_resistance.deleter
-    def ai_bridge_shunt_cal_shunt_cal_b_actual_resistance(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeShuntCalShuntCalBActualResistance)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_shunt_cal_shunt_cal_b_resistance(self):
-        """
-        float: Specifies in ohms the desired value of the internal shunt
-            calibration B resistor.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeShuntCalShuntCalBResistance)
+    def create_ci_pulse_chan_time(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units):
+        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanTime
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, counter, name_to_assign_to_channel, min_val, max_val, units)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_b_resistance.setter
-    def ai_bridge_shunt_cal_shunt_cal_b_resistance(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeShuntCalShuntCalBResistance)
+    def create_ci_pulse_width_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units, starting_edge, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIPulseWidthChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, min_val, max_val, units,
+            starting_edge, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_shunt_cal_shunt_cal_b_resistance.deleter
-    def ai_bridge_shunt_cal_shunt_cal_b_resistance(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeShuntCalShuntCalBResistance)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_table_electrical_vals(self):
-        """
-        List[float]: Specifies the list of electrical values that map to
-            the values in **ai_bridge_table_physical_vals**. Specify
-            this value in the unit indicated by
-            **ai_bridge_electrical_units**.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeTableElectricalVals
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @ai_bridge_table_electrical_vals.setter
-    def ai_bridge_table_electrical_vals(self, val):
-        val = numpy.float64(val)
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeTableElectricalVals
+    def create_ci_semi_period_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCISemiPeriodChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val, len(val))
-        check_for_error(error_code)
-
-    @ai_bridge_table_electrical_vals.deleter
-    def ai_bridge_table_electrical_vals(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeTableElectricalVals
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_table_physical_vals(self):
-        """
-        List[float]: Specifies the list of physical values that map to
-            the values in **ai_bridge_table_electrical_vals**. Specify
-            this value in the unit indicated by
-            **ai_bridge_physical_units**.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeTablePhysicalVals
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.tolist()
+            task, counter, name_to_assign_to_channel, min_val, max_val, units,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_table_physical_vals.setter
-    def ai_bridge_table_physical_vals(self, val):
-        val = numpy.float64(val)
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeTablePhysicalVals
+    def create_ci_two_edge_sep_chan(
+            self, task, counter, name_to_assign_to_channel, min_val, max_val,
+            units, first_edge, second_edge, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCITwoEdgeSepChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val, len(val))
-        check_for_error(error_code)
-
-    @ai_bridge_table_physical_vals.deleter
-    def ai_bridge_table_physical_vals(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeTablePhysicalVals
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_two_point_lin_first_electrical_val(self):
-        """
-        float: Specifies the first electrical value, corresponding to
-            **ai_bridge_two_point_lin_first_physical_val**. Specify this
-            value in the unit indicated by
-            **ai_bridge_electrical_units**.
-        """
-        val = ctypes.c_double()
+            task, counter, name_to_assign_to_channel, min_val, max_val, units,
+            first_edge, second_edge, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeTwoPointLinFirstElectricalVal)
+    def create_cigps_timestamp_chan(
+            self, task, counter, name_to_assign_to_channel, units,
+            sync_method, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateCIGPSTimestampChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, counter, name_to_assign_to_channel, units, sync_method,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_first_electrical_val.setter
-    def ai_bridge_two_point_lin_first_electrical_val(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeTwoPointLinFirstElectricalVal)
+    def create_co_pulse_chan_freq(
+            self, task, counter, name_to_assign_to_channel, units, idle_state,
+            initial_delay, freq, duty_cycle):
+        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanFreq
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, units, idle_state,
+            initial_delay, freq, duty_cycle)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_first_electrical_val.deleter
-    def ai_bridge_two_point_lin_first_electrical_val(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeTwoPointLinFirstElectricalVal)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_two_point_lin_first_physical_val(self):
-        """
-        float: Specifies the first physical value, corresponding to
-            **ai_bridge_two_point_lin_first_electrical_val**. Specify
-            this value in the unit indicated by
-            **ai_bridge_physical_units**.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeTwoPointLinFirstPhysicalVal)
+    def create_co_pulse_chan_ticks(
+            self, task, counter, source_terminal, name_to_assign_to_channel,
+            idle_state, initial_delay, low_ticks, high_ticks):
+        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanTicks
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes_byte_str, ctypes.c_int,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, counter, name_to_assign_to_channel, source_terminal,
+            idle_state, initial_delay, low_ticks, high_ticks)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_first_physical_val.setter
-    def ai_bridge_two_point_lin_first_physical_val(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeTwoPointLinFirstPhysicalVal)
+    def create_co_pulse_chan_time(
+            self, task, counter, name_to_assign_to_channel, units, idle_state,
+            initial_delay, low_time, high_time):
+        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanTime
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, counter, name_to_assign_to_channel, units, idle_state,
+            initial_delay, low_time, high_time)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_first_physical_val.deleter
-    def ai_bridge_two_point_lin_first_physical_val(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeTwoPointLinFirstPhysicalVal)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_bridge_two_point_lin_second_electrical_val(self):
-        """
-        float: Specifies the second electrical value, corresponding to
-            **ai_bridge_two_point_lin_second_physical_val**. Specify
-            this value in the unit indicated by
-            **ai_bridge_electrical_units**.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeTwoPointLinSecondElectricalVal)
+    def create_di_chan(
+            self, task, lines, name_to_assign_to_lines, line_grouping):
+        cfunc = lib_importer.windll.DAQmxCreateDIChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, lines, name_to_assign_to_lines, line_grouping)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_second_electrical_val.setter
-    def ai_bridge_two_point_lin_second_electrical_val(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeTwoPointLinSecondElectricalVal)
+    def create_do_chan(
+            self, task, lines, name_to_assign_to_lines, line_grouping):
+        cfunc = lib_importer.windll.DAQmxCreateDOChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, lines, name_to_assign_to_lines, line_grouping)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_second_electrical_val.deleter
-    def ai_bridge_two_point_lin_second_electrical_val(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeTwoPointLinSecondElectricalVal)
+    def create_lin_scale(
+            self, name, slope, y_intercept, pre_scaled_units, scaled_units):
+        cfunc = lib_importer.windll.DAQmxCreateLinScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            name, slope, y_intercept, pre_scaled_units, scaled_units)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_bridge_two_point_lin_second_physical_val(self):
-        """
-        float: Specifies the second physical value, corresponding to
-            **ai_bridge_two_point_lin_second_electrical_val**. Specify
-            this value in the unit indicated by
-            **ai_bridge_physical_units**.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIBridgeTwoPointLinSecondPhysicalVal)
+    def create_map_scale(
+            self, name, prescaled_min, prescaled_max, scaled_min, scaled_max,
+            pre_scaled_units, scaled_units):
+        cfunc = lib_importer.windll.DAQmxCreateMapScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            name, prescaled_min, prescaled_max, scaled_min, scaled_max,
+            pre_scaled_units, scaled_units)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_bridge_two_point_lin_second_physical_val.setter
-    def ai_bridge_two_point_lin_second_physical_val(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIBridgeTwoPointLinSecondPhysicalVal)
+    def create_polynomial_scale(
+            self, name, forward_coeffs, reverse_coeffs, pre_scaled_units,
+            scaled_units):
+        cfunc = lib_importer.windll.DAQmxCreatePolynomialScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            name, forward_coeffs, len(forward_coeffs), reverse_coeffs,
+            len(reverse_coeffs), pre_scaled_units, scaled_units)
+        self.check_for_error(error_code)
 
-    @ai_bridge_two_point_lin_second_physical_val.deleter
-    def ai_bridge_two_point_lin_second_physical_val(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIBridgeTwoPointLinSecondPhysicalVal)
+    def create_table_scale(
+            self, name, prescaled_vals, scaled_vals, pre_scaled_units,
+            scaled_units):
+        cfunc = lib_importer.windll.DAQmxCreateTableScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.c_uint, wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            name, prescaled_vals, len(prescaled_vals), scaled_vals,
+            len(scaled_vals), pre_scaled_units, scaled_units)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_bridge_units(self):
-        """
-        :class:`nidaqmx.constants.BridgeUnits`: Specifies in which unit
-            to return voltage ratios from the channel.
-        """
-        val = ctypes.c_int()
+    def create_task(self, session_name):
+        new_session_initialized = True
+        task = lib_importer.task_handle(0)
 
-        cfunc = lib_importer.windll.DAQmxGetAIBridgeUnits
+        cfunc = lib_importer.windll.DAQmxCreateTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str,
+                        ctypes.POINTER(lib_importer.task_handle)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            session_name, ctypes.byref(task))
+        self.check_for_error(error_code)
+        return task, new_session_initialized
 
-        return BridgeUnits(val.value)
-
-    @ai_bridge_units.setter
-    def ai_bridge_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIBridgeUnits
+    def create_tedsai_accel_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, current_excit_source,
+            current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIAccelChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_bridge_units.deleter
-    def ai_bridge_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIBridgeUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_charge_units(self):
-        """
-        :class:`nidaqmx.constants.ChargeUnits`: Specifies the units to
-            use to return charge measurements from the channel.
-        """
-        val = ctypes.c_int()
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, current_excit_source,
+            current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIChargeUnits
+    def create_tedsai_bridge_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIBridgeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ChargeUnits(val.value)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_charge_units.setter
-    def ai_charge_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIChargeUnits
+    def create_tedsai_current_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAICurrentChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, shunt_resistor_loc,
+            ext_shunt_resistor_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_charge_units.deleter
-    def ai_charge_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIChargeUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_chop_enable(self):
-        """
-        bool: Specifies whether the device will chop its inputs.
-            Chopping removes offset voltages and other low frequency
-            errors.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIChopEnable
+    def create_tedsai_force_bridge_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIForceBridgeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_chop_enable.setter
-    def ai_chop_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIChopEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_chop_enable.deleter
-    def ai_chop_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIChopEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_coupling(self):
-        """
-        :class:`nidaqmx.constants.Coupling`: Specifies the coupling for
-            the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAICoupling
+    def create_tedsai_force_iepe_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, current_excit_source,
+            current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIForceIEPEChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return Coupling(val.value)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, current_excit_source,
+            current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_coupling.setter
-    def ai_coupling(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAICoupling
+    def create_tedsai_microphone_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, units, max_snd_press_level, current_excit_source,
+            current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIMicrophoneChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_coupling.deleter
-    def ai_coupling(self):
-        cfunc = lib_importer.windll.DAQmxResetAICoupling
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_current_acrms_units(self):
-        """
-        :class:`nidaqmx.constants.CurrentUnits`: Specifies the units to
-            use to return current RMS measurements from the channel.
-        """
-        val = ctypes.c_int()
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, units, max_snd_press_level, current_excit_source,
+            current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAICurrentACRMSUnits
+    def create_tedsai_pos_lvdt_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            voltage_excit_freq, ac_excit_wire_mode, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPosLVDTChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            voltage_excit_freq, ac_excit_wire_mode, custom_scale_name)
+        self.check_for_error(error_code)
 
-        return CurrentUnits(val.value)
-
-    @ai_current_acrms_units.setter
-    def ai_current_acrms_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAICurrentACRMSUnits
+    def create_tedsai_pos_rvdt_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            voltage_excit_freq, ac_excit_wire_mode, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPosRVDTChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            voltage_excit_freq, ac_excit_wire_mode, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_current_acrms_units.deleter
-    def ai_current_acrms_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAICurrentACRMSUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_current_shunt_loc(self):
-        """
-        :class:`nidaqmx.constants.CurrentShuntResistorLocation`:
-            Specifies the shunt resistor location for current
-            measurements.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAICurrentShuntLoc
+    def create_tedsai_pressure_bridge_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIPressureBridgeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return CurrentShuntResistorLocation(val.value)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_current_shunt_loc.setter
-    def ai_current_shunt_loc(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAICurrentShuntLoc
+    def create_tedsai_resistance_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIResistanceChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_current_shunt_loc.deleter
-    def ai_current_shunt_loc(self):
-        cfunc = lib_importer.windll.DAQmxResetAICurrentShuntLoc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_current_shunt_resistance(self):
-        """
-        float: Specifies in ohms the external shunt resistance for
-            current measurements.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAICurrentShuntResistance
+    def create_tedsai_strain_gage_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            initial_bridge_voltage, lead_wire_resistance, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIStrainGageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            initial_bridge_voltage, lead_wire_resistance, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_current_shunt_resistance.setter
-    def ai_current_shunt_resistance(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAICurrentShuntResistance
+    def create_tedsai_thrmcpl_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, cjc_source, cjc_val, cjc_channel):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmcplChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_current_shunt_resistance.deleter
-    def ai_current_shunt_resistance(self):
-        cfunc = lib_importer.windll.DAQmxResetAICurrentShuntResistance
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, cjc_source, cjc_val, cjc_channel)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_current_units(self):
-        """
-        :class:`nidaqmx.constants.CurrentUnits`: Specifies the units to
-            use to return current measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAICurrentUnits
+    def create_tedsai_thrmstr_chan_iex(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmstrChanIex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return CurrentUnits(val.value)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val)
+        self.check_for_error(error_code)
 
-    @ai_current_units.setter
-    def ai_current_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAICurrentUnits
+    def create_tedsai_thrmstr_chan_vex(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, voltage_excit_source,
+            voltage_excit_val, r_1):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIThrmstrChanVex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, voltage_excit_source,
+            voltage_excit_val, r_1)
+        self.check_for_error(error_code)
 
-    @ai_current_units.deleter
-    def ai_current_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAICurrentUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_custom_scale(self):
-        """
-        :class:`nidaqmx.system.scale.Scale`: Specifies the name of a
-            custom scale for the channel.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAICustomScaleName
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_char_p, ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return Scale(val.value.decode('ascii'))
-
-    @ai_custom_scale.setter
-    def ai_custom_scale(self, val):
-        val = val.name
-        cfunc = lib_importer.windll.DAQmxSetAICustomScaleName
+    def create_tedsai_torque_bridge_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAITorqueBridgeChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
                         ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_custom_scale.deleter
-    def ai_custom_scale(self):
-        cfunc = lib_importer.windll.DAQmxResetAICustomScaleName
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_data_xfer_custom_threshold(self):
-        """
-        int: Specifies the number of samples that must be in the FIFO to
-            transfer data from the device if **ai_data_xfer_req_cond**
-            is
-            **InputDataTransferCondition.ONBOARD_MEMORY_CUSTOM_THRESHOLD**.
-        """
-        val = ctypes.c_uint()
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, voltage_excit_source, voltage_excit_val,
+            custom_scale_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIDataXferCustomThreshold
+    def create_tedsai_voltage_chan(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIVoltageChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_custom_threshold.setter
-    def ai_data_xfer_custom_threshold(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDataXferCustomThreshold
+    def create_tedsai_voltage_chan_with_excit(
+            self, task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, voltage_excit_source,
+            voltage_excit_val, custom_scale_name):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIVoltageChanWithExcit
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
+                        ctypes_byte_str, ctypes.c_int, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel,
+            terminal_config, min_val, max_val, units, voltage_excit_source,
+            voltage_excit_val, custom_scale_name)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_custom_threshold.deleter
-    def ai_data_xfer_custom_threshold(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDataXferCustomThreshold
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_data_xfer_max_rate(self):
-        """
-        float: Specifies the rate in B/s to transfer data from the
-            device. If this value is not set, then the device will
-            transfer data at a rate based on the bus detected. Modify
-            this value to affect performance under different
-            combinations of operating system, configuration, and device.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDataXferMaxRate
+    def create_tedsairtd_chan(
+            self, task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val):
+        cfunc = lib_importer.windll.DAQmxCreateTEDSAIRTDChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
+                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
+                        ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, physical_channel, name_to_assign_to_channel, min_val,
+            max_val, units, resistance_config, current_excit_source,
+            current_excit_val)
+        self.check_for_error(error_code)
 
-        return val.value
+    def create_watchdog_timer_task_ex(
+            self, device_name, session_name, timeout):
+        new_session_initialized = True
+        task = lib_importer.task_handle(0)
 
-    @ai_data_xfer_max_rate.setter
-    def ai_data_xfer_max_rate(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDataXferMaxRate
+        cfunc = lib_importer.windll.DAQmxCreateWatchdogTimerTaskEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        ctypes_byte_str, ctypes_byte_str,
+                        ctypes.POINTER(lib_importer.task_handle),
                         ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name, session_name, ctypes.byref(task), timeout)
+        self.check_for_error(error_code)
+        return task, new_session_initialized
 
-    @ai_data_xfer_max_rate.deleter
-    def ai_data_xfer_max_rate(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDataXferMaxRate
+    def delete_network_device(self, device_name):
+        cfunc = lib_importer.windll.DAQmxDeleteNetworkDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_data_xfer_mech(self):
-        """
-        :class:`nidaqmx.constants.DataTransferActiveTransferMode`:
-            Specifies the data transfer mode for the device.
-        """
-        val = ctypes.c_int()
+            device_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIDataXferMech
+    def delete_saved_global_chan(self, channel_name):
+        cfunc = lib_importer.windll.DAQmxDeleteSavedGlobalChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return DataTransferActiveTransferMode(val.value)
+            channel_name)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_mech.setter
-    def ai_data_xfer_mech(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIDataXferMech
+    def delete_saved_scale(self, scale_name):
+        cfunc = lib_importer.windll.DAQmxDeleteSavedScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            scale_name)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_mech.deleter
-    def ai_data_xfer_mech(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDataXferMech
+    def delete_saved_task(self, task_name):
+        cfunc = lib_importer.windll.DAQmxDeleteSavedTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_data_xfer_req_cond(self):
-        """
-        :class:`nidaqmx.constants.InputDataTransferCondition`: Specifies
-            under what condition to transfer data from the onboard
-            memory of the device to the buffer.
-        """
-        val = ctypes.c_int()
+            task_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIDataXferReqCond
+    def disable_ref_trig(self, task):
+        cfunc = lib_importer.windll.DAQmxDisableRefTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return InputDataTransferCondition(val.value)
+            task)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_req_cond.setter
-    def ai_data_xfer_req_cond(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIDataXferReqCond
+    def disable_start_trig(self, task):
+        cfunc = lib_importer.windll.DAQmxDisableStartTrig
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task)
+        self.check_for_error(error_code)
 
-    @ai_data_xfer_req_cond.deleter
-    def ai_data_xfer_req_cond(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDataXferReqCond
+    def disconnect_terms(self, source_terminal, destination_terminal):
+        cfunc = lib_importer.windll.DAQmxDisconnectTerms
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            source_terminal, destination_terminal)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_dc_offset(self):
-        """
-        float: Specifies the DC value to add to the input range of the
-            device. Use **ai_rng_high** and **ai_rng_low** to specify
-            the input range. This offset is in the native units of the
-            device .
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDCOffset
+    def export_signal(self, task, signal_id, output_terminal):
+        cfunc = lib_importer.windll.DAQmxExportSignal
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_dc_offset.setter
-    def ai_dc_offset(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDCOffset
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            task, signal_id, output_terminal)
+        self.check_for_error(error_code)
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_analog_power_up_states_with_output_type(
+            self, channel_names, array_size):
+        state_array = numpy.zeros(array_size, dtype=numpy.float64)
+        channel_type_array = numpy.zeros(array_size, dtype=numpy.int32)
+        array_size = ctypes.c_uint32(array_size)
 
-    @ai_dc_offset.deleter
-    def ai_dc_offset(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDCOffset
+        cfunc = lib_importer.cdll.DAQmxGetAnalogPowerUpStatesWithOutputType
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), wrapped_ndpointer(dtype=numpy.int32,
+                        flags=('C','W')), ctypes.POINTER(ctypes.c_uint)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            channel_names, state_array, channel_type_array,
+            ctypes.byref(array_size))
+        self.check_for_error(error_code)
+        return state_array.tolist(), channel_type_array.tolist()
 
-    @property
-    def ai_dev_scaling_coeff(self):
-        """
-        List[float]: Indicates the coefficients of a polynomial equation
-            that NI-DAQmx uses to scale values from the native format of
-            the device to volts. Each element of the list corresponds to
-            a term of the equation. For example, if index two of the
-            list is 4, the third term of the equation is 4x^2. Scaling
-            coefficients do not account for any custom scales or sensors
-            contained by the channel.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIDevScalingCoeff
+    def get_auto_configured_cdaq_sync_connections(self):
+        cfunc = lib_importer.windll.DAQmxGetAutoConfiguredCDAQSyncConnections
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+                        ctypes.c_char_p, ctypes.c_uint]
 
         temp_size = 0
         while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
+            port_list = ctypes.create_string_buffer(temp_size)
             size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
+                port_list, temp_size)
+            if is_string_buffer_too_small(size_or_code):
                 # Buffer size must have changed between calls; check again.
                 temp_size = 0
             elif size_or_code > 0 and temp_size == 0:
                 # Buffer size obtained, use to retrieve data.
                 temp_size = size_or_code
             else:
                 break
+        self.check_for_error(size_or_code)
+        return port_list.value.decode('ascii')
 
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @property
-    def ai_dig_fltr_bandpass_center_freq(self):
-        """
-        float: Specifies the center frequency of the passband for the
-            digital filter.
-        """
-        val = ctypes.c_double()
+    def get_buffer_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrBandpassCenterFreq
+        cfunc = lib_importer.cdll.DAQmxGetBufferAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def get_chan_attribute_bool(self, task, channel, attribute):
+        value = c_bool32()
 
-    @ai_dig_fltr_bandpass_center_freq.setter
-    def ai_dig_fltr_bandpass_center_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrBandpassCenterFreq
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_dig_fltr_bandpass_center_freq.deleter
-    def ai_dig_fltr_bandpass_center_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrBandpassCenterFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_bandpass_width(self):
-        """
-        float: Specifies the width of the passband centered around the
-            center frequency for the digital filter.
-        """
-        val = ctypes.c_double()
+    def get_chan_attribute_double(self, task, channel, attribute):
+        value = ctypes.c_double()
 
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrBandpassWidth
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_dig_fltr_bandpass_width.setter
-    def ai_dig_fltr_bandpass_width(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrBandpassWidth
+    def get_chan_attribute_double_array(self, task, channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_bandpass_width.deleter
-    def ai_dig_fltr_bandpass_width(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrBandpassWidth
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_coeff(self):
-        """
-        List[float]: Specifies the digital filter coefficients.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
+                        ctypes.c_int32]
 
         temp_size = 0
         while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
+            value = numpy.zeros(temp_size, dtype=numpy.float64)
             size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
+                task, channel, attribute,
+                value.ctypes.data_as(ctypes.c_void_p), temp_size)
             if is_array_buffer_too_small(size_or_code):
                 # Buffer size must have changed between calls; check again.
                 temp_size = 0
             elif size_or_code > 0 and temp_size == 0:
                 # Buffer size obtained, use to retrieve data.
                 temp_size = size_or_code
             else:
                 break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @ai_dig_fltr_coeff.setter
-    def ai_dig_fltr_coeff(self, val):
-        val = numpy.float64(val)
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val, len(val))
-        check_for_error(error_code)
-
-    @ai_dig_fltr_coeff.deleter
-    def ai_dig_fltr_coeff(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_enable(self):
-        """
-        bool: Specifies whether the digital filter is enabled or
-            disabled.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_dig_fltr_enable.setter
-    def ai_dig_fltr_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_enable.deleter
-    def ai_dig_fltr_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_highpass_cutoff_freq(self):
-        """
-        float: Specifies the highpass cutoff frequency of the digital
-            filter.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrHighpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_dig_fltr_highpass_cutoff_freq.setter
-    def ai_dig_fltr_highpass_cutoff_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrHighpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_highpass_cutoff_freq.deleter
-    def ai_dig_fltr_highpass_cutoff_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrHighpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_lowpass_cutoff_freq(self):
-        """
-        float: Specifies the lowpass cutoff frequency of the digital
-            filter.
-        """
-        val = ctypes.c_double()
+    def get_chan_attribute_int32(self, task, channel, attribute):
+        value = ctypes.c_int32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrLowpassCutoffFreq
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_dig_fltr_lowpass_cutoff_freq.setter
-    def ai_dig_fltr_lowpass_cutoff_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrLowpassCutoffFreq
+    def get_chan_attribute_string(self, task, channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+                        ctypes.c_int32]
 
-    @ai_dig_fltr_lowpass_cutoff_freq.deleter
-    def ai_dig_fltr_lowpass_cutoff_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrLowpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_notch_center_freq(self):
-        """
-        float: Specifies the center frequency of the stopband for the
-            digital filter.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrNotchCenterFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_dig_fltr_notch_center_freq.setter
-    def ai_dig_fltr_notch_center_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrNotchCenterFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_notch_center_freq.deleter
-    def ai_dig_fltr_notch_center_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrNotchCenterFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_notch_width(self):
-        """
-        float: Specifies the width of the stopband centered around the
-            center frequency for the digital filter.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrNotchWidth
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_dig_fltr_notch_width.setter
-    def ai_dig_fltr_notch_width(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrNotchWidth
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_notch_width.deleter
-    def ai_dig_fltr_notch_width(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrNotchWidth
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dig_fltr_order(self):
-        """
-        int: Specifies the order of the digital filter.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrOrder
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, channel, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        return val.value
+    def get_chan_attribute_uint32(self, task, channel, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_dig_fltr_order.setter
-    def ai_dig_fltr_order(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrOrder
+        cfunc = lib_importer.cdll.DAQmxGetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_order.deleter
-    def ai_dig_fltr_order(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrOrder
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_dig_fltr_response(self):
-        """
-        :class:`nidaqmx.constants.FilterResponse`: Specifies the digital
-            filter response.
-        """
-        val = ctypes.c_int()
+    def get_device_attribute_bool(self, device_name, attribute):
+        value = c_bool32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrResponse
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            device_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return FilterResponse(val.value)
+    def get_device_attribute_double(self, device_name, attribute):
+        value = ctypes.c_double()
 
-    @ai_dig_fltr_response.setter
-    def ai_dig_fltr_response(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrResponse
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_dig_fltr_response.deleter
-    def ai_dig_fltr_response(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrResponse
+    def get_device_attribute_double_array(self, device_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+                        ctypes_byte_str, ctypes.c_int32]
 
-    @property
-    def ai_dig_fltr_type(self):
-        """
-        :class:`nidaqmx.constants.FilterType`: Specifies the digital
-            filter type.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDigFltrType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return FilterType(val.value)
-
-    @ai_dig_fltr_type.setter
-    def ai_dig_fltr_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIDigFltrType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_dig_fltr_type.deleter
-    def ai_dig_fltr_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDigFltrType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_dither_enable(self):
-        """
-        bool: Specifies whether to enable dithering.  Dithering adds
-            Gaussian noise to the input signal. You can use dithering to
-            achieve higher resolution measurements by over sampling the
-            input signal and averaging the results.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIDitherEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.float64)
+            size_or_code = cfunc(
+                device_name, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        return val.value
+    def get_device_attribute_int32(self, device_name, attribute):
+        value = ctypes.c_int32()
 
-    @ai_dither_enable.setter
-    def ai_dither_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIDitherEnable
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_dither_enable.deleter
-    def ai_dither_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIDitherEnable
+    def get_device_attribute_int32_array(self, device_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+                        ctypes_byte_str, ctypes.c_int32]
 
-    @property
-    def ai_eddy_current_prox_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the eddy current proximity
-            probe . This value is in the units you specify with
-            **ai_eddy_current_prox_sensitivity_units**. Refer to the
-            sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.int32)
+            size_or_code = cfunc(
+                device_name, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIEddyCurrentProxProbeSensitivity)
+    def get_device_attribute_string(self, device_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_eddy_current_prox_sensitivity.setter
-    def ai_eddy_current_prox_sensitivity(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIEddyCurrentProxProbeSensitivity)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                device_name, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_device_attribute_uint32(self, device_name, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_eddy_current_prox_sensitivity.deleter
-    def ai_eddy_current_prox_sensitivity(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIEddyCurrentProxProbeSensitivity)
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            device_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_eddy_current_prox_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.EddyCurrentProxProbeSensitivityUnits`:
-            Specifies the units of **ai_eddy_current_prox_sensitivity**.
-        """
-        val = ctypes.c_int()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIEddyCurrentProxProbeSensitivityUnits)
+    def get_device_attribute_uint32_array(self, device_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetDeviceAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.uint32)
+            size_or_code = cfunc(
+                device_name, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        return EddyCurrentProxProbeSensitivityUnits(val.value)
+    def get_digital_logic_family_power_up_state(self, device_name):
+        logic_family = ctypes.c_int()
 
-    @ai_eddy_current_prox_sensitivity_units.setter
-    def ai_eddy_current_prox_sensitivity_units(self, val):
-        val = val.value
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIEddyCurrentProxProbeSensitivityUnits)
+        cfunc = lib_importer.windll.DAQmxGetDigitalLogicFamilyPowerUpState
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.POINTER(ctypes.c_int)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name, ctypes.byref(logic_family))
+        self.check_for_error(error_code)
+        return logic_family.value
 
-    @ai_eddy_current_prox_sensitivity_units.deleter
-    def ai_eddy_current_prox_sensitivity_units(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIEddyCurrentProxProbeSensitivityUnits)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def get_digital_power_up_states(self, device_name, channel_name):
+        state = []
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        args = [device_name]
+        argtypes: List[type] = [ctypes_byte_str]
 
-    @property
-    def ai_eddy_current_prox_units(self):
-        """
-        :class:`nidaqmx.constants.LengthUnits`: Specifies the units to
-            use to return proximity measurements from the channel.
-        """
-        val = ctypes.c_int()
+        for index in range(len(channel_name)):
+            state_element = ctypes.c_int32()
+            state.append(state_element)
 
-        cfunc = lib_importer.windll.DAQmxGetAIEddyCurrentProxProbeUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            args.append(channel_name[index])
+            argtypes.append(ctypes_byte_str)
+            
+            args.append(ctypes.byref(state_element))
+            argtypes.append(ctypes.POINTER(ctypes.c_int32))
+            
+        args.append(None)
+        argtypes.append(ctypes.c_void_p)
 
-        return LengthUnits(val.value)
+        cfunc = lib_importer.cdll.DAQmxGetDigitalPowerUpStates
+        with cfunc.arglock:
+            cfunc.argtypes = argtypes
+            error_code = cfunc(*args)
+        self.check_for_error(error_code)
+        return [state_element.value for state_element in state]
 
-    @ai_eddy_current_prox_units.setter
-    def ai_eddy_current_prox_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIEddyCurrentProxProbeUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+    def get_digital_pull_up_pull_down_states(self, device_name, channel_name):
+        state = []
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+        args = [device_name]
+        argtypes: List[type] = [ctypes_byte_str]
 
-    @ai_eddy_current_prox_units.deleter
-    def ai_eddy_current_prox_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIEddyCurrentProxProbeUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+        for index in range(len(channel_name)):
+            state_element = ctypes.c_int32()
+            state.append(state_element)
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            args.append(channel_name[index])
+            argtypes.append(ctypes_byte_str)
+            
+            args.append(ctypes.byref(state_element))
+            argtypes.append(ctypes.POINTER(ctypes.c_int32))
+            
+        args.append(None)
+        argtypes.append(ctypes.c_void_p)
 
-    @property
-    def ai_enhanced_alias_rejection_enable(self):
-        """
-        bool: Specifies whether to enable enhanced alias rejection.
-            Leave this property set to the default value for most
-            applications.
-        """
-        val = c_bool32()
+        cfunc = lib_importer.cdll.DAQmxGetDigitalPullUpPullDownStates
+        with cfunc.arglock:
+            cfunc.argtypes = argtypes
+            error_code = cfunc(*args)
+        self.check_for_error(error_code)
+        return [state_element.value for state_element in state]
 
-        cfunc = lib_importer.windll.DAQmxGetAIEnhancedAliasRejectionEnable
+    def get_disconnected_cdaq_sync_ports(self):
+        cfunc = lib_importer.windll.DAQmxGetDisconnectedCDAQSyncPorts
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+                        ctypes.c_char_p, ctypes.c_uint]
 
-    @ai_enhanced_alias_rejection_enable.setter
-    def ai_enhanced_alias_rejection_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIEnhancedAliasRejectionEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+        temp_size = 0
+        while True:
+            port_list = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                port_list, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return port_list.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_exported_signal_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-    @ai_enhanced_alias_rejection_enable.deleter
-    def ai_enhanced_alias_rejection_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIEnhancedAliasRejectionEnable
+        cfunc = lib_importer.cdll.DAQmxGetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_excit_actual_val(self):
-        """
-        float: Specifies the actual amount of excitation supplied by an
-            internal excitation source.  If you read an internal
-            excitation source more precisely with an external device,
-            set this property to the value you read.  NI-DAQmx ignores
-            this value for external excitation. When performing shunt
-            calibration, some devices set this property automatically.
-        """
-        val = ctypes.c_double()
+    def get_exported_signal_attribute_double(self, task, attribute):
+        value = ctypes.c_double()
 
-        cfunc = lib_importer.windll.DAQmxGetAIExcitActualVal
+        cfunc = lib_importer.cdll.DAQmxGetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def get_exported_signal_attribute_int32(self, task, attribute):
+        value = ctypes.c_int32()
 
-    @ai_excit_actual_val.setter
-    def ai_excit_actual_val(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIExcitActualVal
+        cfunc = lib_importer.cdll.DAQmxGetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_actual_val.deleter
-    def ai_excit_actual_val(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitActualVal
+    def get_exported_signal_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-    @property
-    def ai_excit_d_cor_ac(self):
-        """
-        :class:`nidaqmx.constants.ExcitationDCorAC`: Specifies if the
-            excitation supply is DC or AC.
-        """
-        val = ctypes.c_int()
+    def get_exported_signal_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIExcitDCorAC
+        cfunc = lib_importer.cdll.DAQmxGetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return ExcitationDCorAC(val.value)
+    def get_persisted_chan_attribute_bool(self, channel, attribute):
+        value = c_bool32()
 
-    @ai_excit_d_cor_ac.setter
-    def ai_excit_d_cor_ac(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIExcitDCorAC
+        cfunc = lib_importer.cdll.DAQmxGetPersistedChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_d_cor_ac.deleter
-    def ai_excit_d_cor_ac(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitDCorAC
+    def get_persisted_chan_attribute_string(self, channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPersistedChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_excit_idle_output_behavior(self):
-        """
-        :class:`nidaqmx.constants.ExcitationIdleOutputBehavior`:
-            Specifies whether this channel will disable excitation after
-            the task is uncommitted. Setting this to Zero Volts or Amps
-            disables excitation after task uncommit. Setting this
-            attribute to Maintain Existing Value leaves the excitation
-            on after task uncommit.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIExcitIdleOutputBehavior
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ExcitationIdleOutputBehavior(val.value)
-
-    @ai_excit_idle_output_behavior.setter
-    def ai_excit_idle_output_behavior(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIExcitIdleOutputBehavior
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                channel, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_persisted_scale_attribute_bool(self, scale_name, attribute):
+        value = c_bool32()
 
-    @ai_excit_idle_output_behavior.deleter
-    def ai_excit_idle_output_behavior(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitIdleOutputBehavior
+        cfunc = lib_importer.cdll.DAQmxGetPersistedScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            scale_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_excit_sense(self):
-        """
-        :class:`nidaqmx.constants.Sense`: Specifies whether to use local
-            or remote sense to sense excitation.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIExcitSense
+    def get_persisted_scale_attribute_string(self, scale_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPersistedScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return Sense(val.value)
+                        ctypes_byte_str, ctypes.c_int32]
 
-    @ai_excit_sense.setter
-    def ai_excit_sense(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIExcitSense
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                scale_name, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_persisted_task_attribute_bool(self, task_name, attribute):
+        value = c_bool32()
 
-    @ai_excit_sense.deleter
-    def ai_excit_sense(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitSense
+        cfunc = lib_importer.cdll.DAQmxGetPersistedTaskAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_excit_src(self):
-        """
-        :class:`nidaqmx.constants.ExcitationSource`: Specifies the
-            source of excitation.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIExcitSrc
+    def get_persisted_task_attribute_string(self, task_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPersistedTaskAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task_name, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        return ExcitationSource(val.value)
+    def get_physical_chan_attribute_bool(self, physical_channel, attribute):
+        value = c_bool32()
 
-    @ai_excit_src.setter
-    def ai_excit_src(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIExcitSrc
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            physical_channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_src.deleter
-    def ai_excit_src(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitSrc
+    def get_physical_chan_attribute_bytes(self, physical_channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+                        ctypes_byte_str, ctypes.c_int32]
 
-    @property
-    def ai_excit_use_for_scaling(self):
-        """
-        bool: Specifies if NI-DAQmx divides the measurement by the
-            excitation. You should typically set this property to True
-            for ratiometric transducers. If you set this property to
-            True, set **ai_max** and **ai_min** to reflect the scaling.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIExcitUseForScaling
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.uint8)
+            size_or_code = cfunc(
+                physical_channel, attribute,
+                value.ctypes.data_as(ctypes.c_void_p), temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        return val.value
+    def get_physical_chan_attribute_double(self, physical_channel, attribute):
+        value = ctypes.c_double()
 
-    @ai_excit_use_for_scaling.setter
-    def ai_excit_use_for_scaling(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIExcitUseForScaling
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            physical_channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_use_for_scaling.deleter
-    def ai_excit_use_for_scaling(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitUseForScaling
+    def get_physical_chan_attribute_double_array(
+            self, physical_channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_excit_use_multiplexed(self):
-        """
-        bool: Specifies if the SCXI-1122 multiplexes the excitation to
-            the upper half of the channels as it advances through the
-            scan list.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIExcitUseMultiplexed
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.float64)
+            size_or_code = cfunc(
+                physical_channel, attribute,
+                value.ctypes.data_as(ctypes.c_void_p), temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        return val.value
+    def get_physical_chan_attribute_int32(self, physical_channel, attribute):
+        value = ctypes.c_int32()
 
-    @ai_excit_use_multiplexed.setter
-    def ai_excit_use_multiplexed(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIExcitUseMultiplexed
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            physical_channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_use_multiplexed.deleter
-    def ai_excit_use_multiplexed(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitUseMultiplexed
+    def get_physical_chan_attribute_int32_array(
+            self, physical_channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_excit_val(self):
-        """
-        float: Specifies the amount of excitation that the sensor
-            requires. If **ai_excit_voltage_or_current** is
-            **ExcitationVoltageOrCurrent.USE_VOLTAGE**, this value is in
-            volts. If **ai_excit_voltage_or_current** is
-            **ExcitationVoltageOrCurrent.USE_CURRENT**, this value is in
-            amperes.
-        """
-        val = ctypes.c_double()
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.int32)
+            size_or_code = cfunc(
+                physical_channel, attribute,
+                value.ctypes.data_as(ctypes.c_void_p), temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        cfunc = lib_importer.windll.DAQmxGetAIExcitVal
+    def get_physical_chan_attribute_string(self, physical_channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                physical_channel, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        return val.value
+    def get_physical_chan_attribute_uint32(self, physical_channel, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_excit_val.setter
-    def ai_excit_val(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIExcitVal
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            physical_channel, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_val.deleter
-    def ai_excit_val(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitVal
+    def get_physical_chan_attribute_uint32_array(
+            self, physical_channel, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetPhysicalChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.uint32)
+            size_or_code = cfunc(
+                physical_channel, attribute,
+                value.ctypes.data_as(ctypes.c_void_p), temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-    @property
-    def ai_excit_voltage_or_current(self):
-        """
-        :class:`nidaqmx.constants.ExcitationVoltageOrCurrent`: Specifies
-            if the channel uses current or voltage excitation.
-        """
-        val = ctypes.c_int()
+    def get_read_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIExcitVoltageOrCurrent
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return ExcitationVoltageOrCurrent(val.value)
+    def get_read_attribute_double(self, task, attribute):
+        value = ctypes.c_double()
 
-    @ai_excit_voltage_or_current.setter
-    def ai_excit_voltage_or_current(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIExcitVoltageOrCurrent
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_excit_voltage_or_current.deleter
-    def ai_excit_voltage_or_current(self):
-        cfunc = lib_importer.windll.DAQmxResetAIExcitVoltageOrCurrent
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_filter_delay(self):
-        """
-        float: Indicates the amount of time between when the ADC samples
-            data and when the sample is read by the host device. This
-            value is in the units you specify with
-            **ai_filter_delay_units**. You can adjust this amount of
-            time using **ai_filter_delay_adjustment**.
-        """
-        val = ctypes.c_double()
+    def get_read_attribute_int32(self, task, attribute):
+        value = ctypes.c_int32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterDelay
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @property
-    def ai_filter_delay_adjustment(self):
-        """
-        float: Specifies the amount of filter delay that gets removed if
-            **ai_remove_filter_delay** is enabled. This delay adjustment
-            is in addition to the value indicated by
-            **ai_filter_delay**. This delay adjustment is in the units
-            you specify with **ai_filter_delay_units**.
-        """
-        val = ctypes.c_double()
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterDelayAdjustment
+    def get_read_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_filter_delay_adjustment.setter
-    def ai_filter_delay_adjustment(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFilterDelayAdjustment
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_read_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_filter_delay_adjustment.deleter
-    def ai_filter_delay_adjustment(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterDelayAdjustment
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_filter_delay_units(self):
-        """
-        :class:`nidaqmx.constants.DigitalWidthUnits`: Specifies the
-            units of **ai_filter_delay** and
-            **ai_filter_delay_adjustment**.
-        """
-        val = ctypes.c_int()
+    def get_read_attribute_uint64(self, task, attribute):
+        value = ctypes.c_uint64()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterDelayUnits
+        cfunc = lib_importer.cdll.DAQmxGetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return DigitalWidthUnits(val.value)
+    def get_scale_attribute_double(self, scale_name, attribute):
+        value = ctypes.c_double()
 
-    @ai_filter_delay_units.setter
-    def ai_filter_delay_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIFilterDelayUnits
+        cfunc = lib_importer.cdll.DAQmxGetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            scale_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_filter_delay_units.deleter
-    def ai_filter_delay_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterDelayUnits
+    def get_scale_attribute_double_array(self, scale_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.float64)
+            size_or_code = cfunc(
+                scale_name, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-    @property
-    def ai_filter_enable(self):
-        """
-        bool: Specifies the corresponding filter enable/disable state.
-        """
-        val = c_bool32()
+    def get_scale_attribute_int32(self, scale_name, attribute):
+        value = ctypes.c_int32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterEnable
+        cfunc = lib_importer.cdll.DAQmxGetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            scale_name, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_filter_enable.setter
-    def ai_filter_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFilterEnable
+    def get_scale_attribute_string(self, scale_name, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        ctypes_byte_str, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                scale_name, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-    @ai_filter_enable.deleter
-    def ai_filter_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterEnable
+    def get_system_info_attribute_string(self, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetSystemInfoAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-    @property
-    def ai_filter_freq(self):
-        """
-        float: Specifies the corresponding filter frequency (cutoff or
-            center) of the filter response.
-        """
-        val = ctypes.c_double()
+    def get_system_info_attribute_uint32(self, attribute):
+        value = ctypes.c_uint32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterFreq
+        cfunc = lib_importer.cdll.DAQmxGetSystemInfoAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_filter_freq.setter
-    def ai_filter_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFilterFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_task_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-    @ai_filter_freq.deleter
-    def ai_filter_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterFreq
+        cfunc = lib_importer.cdll.DAQmxGetTaskAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_filter_order(self):
-        """
-        int: Specifies the corresponding filter order and defines the
-            slope of the filter response.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAIFilterOrder
+    def get_task_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTaskAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_filter_order.setter
-    def ai_filter_order(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFilterOrder
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_task_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_filter_order.deleter
-    def ai_filter_order(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterOrder
+        cfunc = lib_importer.cdll.DAQmxGetTaskAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_filter_response(self):
-        """
-        :class:`nidaqmx.constants.FilterResponse`: Specifies the
-            corresponding filter response and defines the shape of the
-            filter response.
-        """
-        val = ctypes.c_int()
+    def get_timing_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFilterResponse
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return FilterResponse(val.value)
+    def get_timing_attribute_double(self, task, attribute):
+        value = ctypes.c_double()
 
-    @ai_filter_response.setter
-    def ai_filter_response(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIFilterResponse
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_filter_response.deleter
-    def ai_filter_response(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFilterResponse
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+    def get_timing_attribute_ex_bool(self, task, device_names, attribute):
+        value = c_bool32()
 
-    @property
-    def ai_force_iepe_sensor_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the IEPE force sensor
-            connected to the channel. Specify this value in the unit
-            indicated by **ai_force_iepe_sensor_sensitivity_units**.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIForceIEPESensorSensitivity
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def get_timing_attribute_ex_double(self, task, device_names, attribute):
+        value = ctypes.c_double()
 
-    @ai_force_iepe_sensor_sensitivity.setter
-    def ai_force_iepe_sensor_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIForceIEPESensorSensitivity
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_force_iepe_sensor_sensitivity.deleter
-    def ai_force_iepe_sensor_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIForceIEPESensorSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_force_iepe_sensor_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.ForceIEPESensorSensitivityUnits`:
-            Specifies the units for
-            **ai_force_iepe_sensor_sensitivity**.
-        """
-        val = ctypes.c_int()
+    def get_timing_attribute_ex_int32(self, task, device_names, attribute):
+        value = ctypes.c_int32()
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIForceIEPESensorSensitivityUnits)
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ForceIEPESensorSensitivityUnits(val.value)
+            task, device_names, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_force_iepe_sensor_sensitivity_units.setter
-    def ai_force_iepe_sensor_sensitivity_units(self, val):
-        val = val.value
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIForceIEPESensorSensitivityUnits)
+    def get_timing_attribute_ex_string(self, task, device_names, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+                        ctypes.c_int32]
 
-    @ai_force_iepe_sensor_sensitivity_units.deleter
-    def ai_force_iepe_sensor_sensitivity_units(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIForceIEPESensorSensitivityUnits)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, device_names, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-    @property
-    def ai_force_read_from_chan(self):
-        """
-        bool: Specifies whether to read from the channel if it is a
-            cold-junction compensation channel. By default, DAQmx Read
-            does not return data from cold-junction compensation
-            channels.  Setting this property to True forces read
-            operations to return the cold-junction compensation channel
-            data with the other channels in the task.
-        """
-        val = c_bool32()
+    def get_timing_attribute_ex_uint32(self, task, device_names, attribute):
+        value = ctypes.c_uint32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIForceReadFromChan
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_force_read_from_chan.setter
-    def ai_force_read_from_chan(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIForceReadFromChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+            task, device_names, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_timing_attribute_ex_uint64(self, task, device_names, attribute):
+        value = ctypes.c_uint64()
 
-    @ai_force_read_from_chan.deleter
-    def ai_force_read_from_chan(self):
-        cfunc = lib_importer.windll.DAQmxResetAIForceReadFromChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_force_units(self):
-        """
-        :class:`nidaqmx.constants.ForceUnits`: Specifies in which unit
-            to return force or load measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIForceUnits
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return ForceUnits(val.value)
+    def get_timing_attribute_int32(self, task, attribute):
+        value = ctypes.c_int32()
 
-    @ai_force_units.setter
-    def ai_force_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIForceUnits
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_force_units.deleter
-    def ai_force_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIForceUnits
+    def get_timing_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-    @property
-    def ai_freq_hyst(self):
-        """
-        float: Specifies in volts a window below
-            **ai_freq_thresh_voltage**. The input voltage must pass
-            below **ai_freq_thresh_voltage** minus this value before NI-
-            DAQmx recognizes a waveform repetition at
-            **ai_freq_thresh_voltage**. Hysteresis can improve the
-            measurement accuracy when the signal contains noise or
-            jitter.
-        """
-        val = ctypes.c_double()
+    def get_timing_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFreqHyst
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def get_timing_attribute_uint64(self, task, attribute):
+        value = ctypes.c_uint64()
 
-    @ai_freq_hyst.setter
-    def ai_freq_hyst(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFreqHyst
+        cfunc = lib_importer.cdll.DAQmxGetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_freq_hyst.deleter
-    def ai_freq_hyst(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFreqHyst
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_freq_thresh_voltage(self):
-        """
-        float: Specifies the voltage level at which to recognize
-            waveform repetitions. You should select a voltage level that
-            occurs only once within the entire period of a waveform. You
-            also can select a voltage that occurs only once while the
-            voltage rises or falls.
-        """
-        val = ctypes.c_double()
+    def get_trig_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIFreqThreshVoltage
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def get_trig_attribute_double(self, task, attribute):
+        value = ctypes.c_double()
 
-    @ai_freq_thresh_voltage.setter
-    def ai_freq_thresh_voltage(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIFreqThreshVoltage
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_freq_thresh_voltage.deleter
-    def ai_freq_thresh_voltage(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFreqThreshVoltage
+    def get_trig_attribute_double_array(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_freq_units(self):
-        """
-        :class:`nidaqmx.constants.FrequencyUnits`: Specifies the units
-            to use to return frequency measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIFreqUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.float64)
+            size_or_code = cfunc(
+                task, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        return FrequencyUnits(val.value)
+    def get_trig_attribute_int32(self, task, attribute):
+        value = ctypes.c_int32()
 
-    @ai_freq_units.setter
-    def ai_freq_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIFreqUnits
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_freq_units.deleter
-    def ai_freq_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIFreqUnits
+    def get_trig_attribute_int32_array(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_gain(self):
-        """
-        float: Specifies a gain factor to apply to the channel.
-        """
-        val = ctypes.c_double()
+        temp_size = 0
+        while True:
+            value = numpy.zeros(temp_size, dtype=numpy.int32)
+            size_or_code = cfunc(
+                task, attribute, value.ctypes.data_as(ctypes.c_void_p),
+                temp_size)
+            if is_array_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.tolist()
 
-        cfunc = lib_importer.windll.DAQmxGetAIGain
+    def get_trig_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_gain.setter
-    def ai_gain(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIGain
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_trig_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_gain.deleter
-    def ai_gain(self):
-        cfunc = lib_importer.windll.DAQmxResetAIGain
+        cfunc = lib_importer.cdll.DAQmxGetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_impedance(self):
-        """
-        :class:`nidaqmx.constants.Impedance1`: Specifies the input
-            impedance of the channel.
-        """
-        val = ctypes.c_double()
+    def get_watchdog_attribute_bool(self, task, lines, attribute):
+        value = c_bool32()
 
-        cfunc = lib_importer.windll.DAQmxGetAIImpedance
+        cfunc = lib_importer.cdll.DAQmxGetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, lines, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return Impedance1(val.value)
+    def get_watchdog_attribute_double(self, task, lines, attribute):
+        value = ctypes.c_double()
 
-    @ai_impedance.setter
-    def ai_impedance(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIImpedance
+        cfunc = lib_importer.cdll.DAQmxGetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, lines, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @ai_impedance.deleter
-    def ai_impedance(self):
-        cfunc = lib_importer.windll.DAQmxResetAIImpedance
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+    def get_watchdog_attribute_int32(self, task, lines, attribute):
+        value = ctypes.c_int32()
 
-    @property
-    def ai_input_limits_fault_detect_enable(self):
-        """
-        bool: Specifies whether to enable input limits fault detection.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIInputLimitsFaultDetectEnable
+        cfunc = lib_importer.cdll.DAQmxGetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, lines, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
-
-    @ai_input_limits_fault_detect_enable.setter
-    def ai_input_limits_fault_detect_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIInputLimitsFaultDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_input_limits_fault_detect_enable.deleter
-    def ai_input_limits_fault_detect_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIInputLimitsFaultDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_input_limits_fault_detect_lower_limit(self):
-        """
-        float: Specifies the level of the lower limit for input limits
-            detection. An input sample outside the upper and lower
-            bounds causes a fault. Note: Fault detection applies to both
-            positive and negative inputs. For instance, if you specify a
-            lower limit of 2 mA and an upper limit of 12 mA, NI-DAQmx
-            detects a fault at 15 mA and -15 mA, but not at -6 mA
-            because it is in the range of -12 mA to -2 mA.
-        """
-        val = ctypes.c_double()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIInputLimitsFaultDetectLowerLimit)
+    def get_watchdog_attribute_string(self, task, lines, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+                        ctypes.c_int32]
 
-        return val.value
-
-    @ai_input_limits_fault_detect_lower_limit.setter
-    def ai_input_limits_fault_detect_lower_limit(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIInputLimitsFaultDetectLowerLimit)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+        temp_size = 0
+        while True:
+            value = ctypes.create_string_buffer(temp_size)
+            size_or_code = cfunc(
+                task, lines, attribute, value, temp_size)
+            if is_string_buffer_too_small(size_or_code):
+                # Buffer size must have changed between calls; check again.
+                temp_size = 0
+            elif size_or_code > 0 and temp_size == 0:
+                # Buffer size obtained, use to retrieve data.
+                temp_size = size_or_code
+            else:
+                break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_write_attribute_bool(self, task, attribute):
+        value = c_bool32()
 
-    @ai_input_limits_fault_detect_lower_limit.deleter
-    def ai_input_limits_fault_detect_lower_limit(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIInputLimitsFaultDetectLowerLimit)
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_input_limits_fault_detect_upper_limit(self):
-        """
-        float: Specifies the level of the upper limit for input limits
-            detection. An input sample outside the upper and lower
-            bounds causes a fault. Note: Fault detection applies to both
-            positive and negative inputs. For instance, if you specify a
-            lower limit of 2 mA and an upper limit of 12 mA, NI-DAQmx
-            detects a fault at 15 mA and -15 mA, but not at -6 mA
-            because it is in the range of -12 mA to -2 mA.
-        """
-        val = ctypes.c_double()
+    def get_write_attribute_double(self, task, attribute):
+        value = ctypes.c_double()
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIInputLimitsFaultDetectUpperLimit)
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_input_limits_fault_detect_upper_limit.setter
-    def ai_input_limits_fault_detect_upper_limit(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIInputLimitsFaultDetectUpperLimit)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_write_attribute_int32(self, task, attribute):
+        value = ctypes.c_int32()
 
-    @ai_input_limits_fault_detect_upper_limit.deleter
-    def ai_input_limits_fault_detect_upper_limit(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIInputLimitsFaultDetectUpperLimit)
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_input_src(self):
-        """
-        str: Specifies the source of the channel. You can use the signal
-            from the I/O connector or one of several calibration
-            signals. Certain devices have a single calibration signal
-            bus. For these devices, you must specify the same
-            calibration signal for all channels you connect to a
-            calibration signal.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIInputSrc
+    def get_write_attribute_string(self, task, attribute):
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_char_p, ctypes.c_uint]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         temp_size = 0
         while True:
-            val = ctypes.create_string_buffer(temp_size)
-
+            value = ctypes.create_string_buffer(temp_size)
             size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
+                task, attribute, value, temp_size)
             if is_string_buffer_too_small(size_or_code):
                 # Buffer size must have changed between calls; check again.
                 temp_size = 0
             elif size_or_code > 0 and temp_size == 0:
                 # Buffer size obtained, use to retrieve data.
                 temp_size = size_or_code
             else:
                 break
+        self.check_for_error(size_or_code)
+        return value.value.decode('ascii')
 
-        check_for_error(size_or_code)
-
-        return val.value.decode('ascii')
-
-    @ai_input_src.setter
-    def ai_input_src(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIInputSrc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def get_write_attribute_uint32(self, task, attribute):
+        value = ctypes.c_uint32()
 
-    @ai_input_src.deleter
-    def ai_input_src(self):
-        cfunc = lib_importer.windll.DAQmxResetAIInputSrc
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_lead_wire_resistance(self):
-        """
-        float: Specifies in ohms the resistance of the wires that lead
-            to the sensor.
-        """
-        val = ctypes.c_double()
+    def get_write_attribute_uint64(self, task, attribute):
+        value = ctypes.c_uint64()
 
-        cfunc = lib_importer.windll.DAQmxGetAILeadWireResistance
+        cfunc = lib_importer.cdll.DAQmxGetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.byref(value))
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def is_task_done(self, task):
+        is_task_done = c_bool32()
 
-    @ai_lead_wire_resistance.setter
-    def ai_lead_wire_resistance(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILeadWireResistance
+        cfunc = lib_importer.windll.DAQmxIsTaskDone
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, ctypes.byref(is_task_done))
+        self.check_for_error(error_code)
+        return is_task_done.value
 
-    @ai_lead_wire_resistance.deleter
-    def ai_lead_wire_resistance(self):
-        cfunc = lib_importer.windll.DAQmxResetAILeadWireResistance
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+    def load_task(self, session_name):
+        new_session_initialized = True
+        task = lib_importer.task_handle(0)
 
-    @property
-    def ai_lossy_lsb_removal_compressed_samp_size(self):
-        """
-        int: Specifies the number of bits to return in a raw sample when
-            **ai_raw_data_compression_type** is set to
-            **RawDataCompressionType.LOSSY_LSB_REMOVAL**.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAILossyLSBRemovalCompressedSampSize)
+        cfunc = lib_importer.windll.DAQmxLoadTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        ctypes_byte_str,
+                        ctypes.POINTER(lib_importer.task_handle)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            session_name, ctypes.byref(task))
+        self.check_for_error(error_code)
+        return task, new_session_initialized
 
-        return val.value
+    def read_analog_f64(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_lossy_lsb_removal_compressed_samp_size.setter
-    def ai_lossy_lsb_removal_compressed_samp_size(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAILossyLSBRemovalCompressedSampSize)
+        cfunc = lib_importer.windll.DAQmxReadAnalogF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lossy_lsb_removal_compressed_samp_size.deleter
-    def ai_lossy_lsb_removal_compressed_samp_size(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAILossyLSBRemovalCompressedSampSize)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lowpass_cutoff_freq(self):
-        """
-        float: Specifies the frequency in Hertz that corresponds to the
-            -3dB cutoff of the filter.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAILowpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lowpass_cutoff_freq.setter
-    def ai_lowpass_cutoff_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILowpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_cutoff_freq.deleter
-    def ai_lowpass_cutoff_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassCutoffFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @property
-    def ai_lowpass_enable(self):
-        """
-        bool: Specifies whether to enable the lowpass filter of the
-            channel.
-        """
-        val = c_bool32()
+    def read_analog_scalar_f64(self, task, timeout):
+        value = ctypes.c_double()
 
-        cfunc = lib_importer.windll.DAQmxGetAILowpassEnable
+        cfunc = lib_importer.windll.DAQmxReadAnalogScalarF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_double),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lowpass_enable.setter
-    def ai_lowpass_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILowpassEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_enable.deleter
-    def ai_lowpass_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(value), None)
+        self.check_for_error(error_code)
+        return value.value
 
-    @property
-    def ai_lowpass_switch_cap_clk_src(self):
-        """
-        :class:`nidaqmx.constants.SourceSelection`: Specifies the source
-            of the filter clock. If you need a higher resolution for the
-            filter, you can supply an external clock to increase the
-            resolution. Refer to the SCXI-1141/1142/1143 User Manual for
-            more information.
-        """
-        val = ctypes.c_int()
+    def read_binary_i16(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAILowpassSwitchCapClkSrc
+        cfunc = lib_importer.windll.DAQmxReadBinaryI16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return SourceSelection(val.value)
-
-    @ai_lowpass_switch_cap_clk_src.setter
-    def ai_lowpass_switch_cap_clk_src(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAILowpassSwitchCapClkSrc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_switch_cap_clk_src.deleter
-    def ai_lowpass_switch_cap_clk_src(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassSwitchCapClkSrc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lowpass_switch_cap_ext_clk_div(self):
-        """
-        int: Specifies the divisor for the external clock when you set
-            **ai_lowpass_switch_cap_clk_src** to
-            **SourceSelection.EXTERNAL**. On the SCXI-1141, SCXI-1142,
-            and SCXI-1143, NI-DAQmx determines the filter cutoff by
-            using the equation f/(100*n), where f is the external
-            frequency, and n is the external clock divisor. Refer to the
-            SCXI-1141/1142/1143 User Manual for more information.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAILowpassSwitchCapExtClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lowpass_switch_cap_ext_clk_div.setter
-    def ai_lowpass_switch_cap_ext_clk_div(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILowpassSwitchCapExtClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_switch_cap_ext_clk_div.deleter
-    def ai_lowpass_switch_cap_ext_clk_div(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassSwitchCapExtClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lowpass_switch_cap_ext_clk_freq(self):
-        """
-        float: Specifies the frequency of the external clock when you
-            set **ai_lowpass_switch_cap_clk_src** to
-            **SourceSelection.EXTERNAL**.  NI-DAQmx uses this frequency
-            to set the pre- and post- filters on the SCXI-1141,
-            SCXI-1142, and SCXI-1143. On those devices, NI-DAQmx
-            determines the filter cutoff by using the equation
-            f/(100*n), where f is the external frequency, and n is the
-            external clock divisor. Refer to the SCXI-1141/1142/1143
-            User Manual for more information.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAILowpassSwitchCapExtClkFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lowpass_switch_cap_ext_clk_freq.setter
-    def ai_lowpass_switch_cap_ext_clk_freq(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILowpassSwitchCapExtClkFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_switch_cap_ext_clk_freq.deleter
-    def ai_lowpass_switch_cap_ext_clk_freq(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassSwitchCapExtClkFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lowpass_switch_cap_out_clk_div(self):
-        """
-        int: Specifies the divisor for the output clock.  NI-DAQmx uses
-            the cutoff frequency to determine the output clock
-            frequency. Refer to the SCXI-1141/1142/1143 User Manual for
-            more information.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAILowpassSwitchCapOutClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lowpass_switch_cap_out_clk_div.setter
-    def ai_lowpass_switch_cap_out_clk_div(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILowpassSwitchCapOutClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lowpass_switch_cap_out_clk_div.deleter
-    def ai_lowpass_switch_cap_out_clk_div(self):
-        cfunc = lib_importer.windll.DAQmxResetAILowpassSwitchCapOutClkDiv
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lvdt_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the LVDT. This value is in
-            the units you specify with **ai_lvdt_sensitivity_units**.
-            Refer to the sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAILVDTSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_lvdt_sensitivity.setter
-    def ai_lvdt_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAILVDTSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lvdt_sensitivity.deleter
-    def ai_lvdt_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAILVDTSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_lvdt_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.LVDTSensitivityUnits`: Specifies the
-            units of **ai_lvdt_sensitivity**.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAILVDTSensitivityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return LVDTSensitivityUnits(val.value)
-
-    @ai_lvdt_sensitivity_units.setter
-    def ai_lvdt_sensitivity_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAILVDTSensitivityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_lvdt_sensitivity_units.deleter
-    def ai_lvdt_sensitivity_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAILVDTSensitivityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.int16, flags=('C','W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @property
-    def ai_lvdt_units(self):
-        """
-        :class:`nidaqmx.constants.LengthUnits`: Specifies the units to
-            use to return linear position measurements from the channel.
-        """
-        val = ctypes.c_int()
+    def read_binary_i32(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAILVDTUnits
+        cfunc = lib_importer.windll.DAQmxReadBinaryI32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C','W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        return LengthUnits(val.value)
+    def read_binary_u16(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_lvdt_units.setter
-    def ai_lvdt_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAILVDTUnits
+        cfunc = lib_importer.windll.DAQmxReadBinaryU16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint16,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @ai_lvdt_units.deleter
-    def ai_lvdt_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAILVDTUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_max(self):
-        """
-        float: Specifies the maximum value you expect to measure. This
-            value is in the units you specify with a units property.
-            When you query this property, it returns the coerced maximum
-            value that the device can measure with the current settings.
-        """
-        val = ctypes.c_double()
+    def read_binary_u32(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIMax
+        cfunc = lib_importer.windll.DAQmxReadBinaryU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_max.setter
-    def ai_max(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIMax
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def read_counter_f64(self, task, num_samps_per_chan, timeout, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_max.deleter
-    def ai_max(self):
-        cfunc = lib_importer.windll.DAQmxResetAIMax
+        cfunc = lib_importer.windll.DAQmxReadCounterF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, read_array, read_array.size,
+            ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @property
-    def ai_meas_type(self):
-        """
-        :class:`nidaqmx.constants.UsageTypeAI`: Indicates the
-            measurement to take with the analog input channel and in
-            some cases, such as for temperature measurements, the sensor
-            to use.
-        """
-        val = ctypes.c_int()
+    def read_counter_f64_ex(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIMeasType
+        cfunc = lib_importer.windll.DAQmxReadCounterF64Ex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        return UsageTypeAI(val.value)
+    def read_counter_scalar_f64(self, task, timeout):
+        value = ctypes.c_double()
 
-    @property
-    def ai_mem_map_enable(self):
-        """
-        bool: Specifies for NI-DAQmx to map hardware registers to the
-            memory space of the application, if possible. Normally, NI-
-            DAQmx maps hardware registers to memory accessible only to
-            the kernel. Mapping the registers to the memory space of the
-            application increases performance. However, if the
-            application accesses the memory space mapped to the
-            registers, it can adversely affect the operation of the
-            device and possibly result in a system crash.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIMemMapEnable
+        cfunc = lib_importer.windll.DAQmxReadCounterScalarF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_double),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(value), None)
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def read_counter_scalar_u32(self, task, timeout):
+        value = ctypes.c_uint()
 
-    @ai_mem_map_enable.setter
-    def ai_mem_map_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIMemMapEnable
+        cfunc = lib_importer.windll.DAQmxReadCounterScalarU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_mem_map_enable.deleter
-    def ai_mem_map_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIMemMapEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_microphone_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the microphone. This value
-            is in mV/Pa. Refer to the sensor documentation to determine
-            this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIMicrophoneSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_uint),
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(value), None)
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def read_counter_u32(self, task, num_samps_per_chan, timeout, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_microphone_sensitivity.setter
-    def ai_microphone_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIMicrophoneSensitivity
+        cfunc = lib_importer.windll.DAQmxReadCounterU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, read_array, read_array.size,
+            ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @ai_microphone_sensitivity.deleter
-    def ai_microphone_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIMicrophoneSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def read_counter_u32_ex(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_min(self):
-        """
-        float: Specifies the minimum value you expect to measure. This
-            value is in the units you specify with a units property.
-            When you query this property, it returns the coerced minimum
-            value that the device can measure with the current settings.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIMin
+        cfunc = lib_importer.windll.DAQmxReadCounterU32Ex
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        return val.value
+    def read_ctr_freq(
+            self, task, num_samps_per_chan, timeout, interleaved,
+            read_array_frequency, read_array_duty_cycle):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_min.setter
-    def ai_min(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIMin
+        cfunc = lib_importer.windll.DAQmxReadCtrFreq
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_min.deleter
-    def ai_min(self):
-        cfunc = lib_importer.windll.DAQmxResetAIMin
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')),
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, interleaved,
+            read_array_frequency, read_array_duty_cycle,
+            read_array_duty_cycle.size, ctypes.byref(samps_per_chan_read),
+            None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array_frequency, read_array_duty_cycle, samps_per_chan_read.value
 
-    @property
-    def ai_open_chan_detect_enable(self):
-        """
-        bool: Specifies whether to enable open channel detection.
-        """
-        val = c_bool32()
+    def read_ctr_freq_scalar(self, task, timeout):
+        frequency = ctypes.c_double()
+        duty_cycle = ctypes.c_double()
 
-        cfunc = lib_importer.windll.DAQmxGetAIOpenChanDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadCtrFreqScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_double),
+                        ctypes.POINTER(ctypes.c_double),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_open_chan_detect_enable.setter
-    def ai_open_chan_detect_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIOpenChanDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+            task, timeout, ctypes.byref(frequency), ctypes.byref(duty_cycle),
+            None)
+        self.check_for_error(error_code)
+        return frequency.value, duty_cycle.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def read_ctr_ticks(
+            self, task, num_samps_per_chan, timeout, interleaved,
+            read_array_high_ticks, read_array_low_ticks):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_open_chan_detect_enable.deleter
-    def ai_open_chan_detect_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIOpenChanDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadCtrTicks
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')),
+                        wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, interleaved,
+            read_array_high_ticks, read_array_low_ticks,
+            read_array_low_ticks.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array_high_ticks, read_array_low_ticks, samps_per_chan_read.value
 
-    @property
-    def ai_open_thrmcpl_detect_enable(self):
-        """
-        bool: Specifies whether to apply the open thermocouple detection
-            bias voltage to the channel. Changing the value of this
-            property on a channel may require settling time before the
-            data returned is valid. To compensate for this settling
-            time, discard unsettled data or add a delay between
-            committing and starting the task. Refer to your device
-            specifications for the required settling time. When open
-            thermocouple detection is enabled, use
-            **open_thrmcpl_chans_exist** to determine if any channels
-            were open.
-        """
-        val = c_bool32()
+    def read_ctr_ticks_scalar(self, task, timeout):
+        high_ticks = ctypes.c_uint()
+        low_ticks = ctypes.c_uint()
 
-        cfunc = lib_importer.windll.DAQmxGetAIOpenThrmcplDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadCtrTicksScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_uint),
+                        ctypes.POINTER(ctypes.c_uint),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(high_ticks), ctypes.byref(low_ticks),
+            None)
+        self.check_for_error(error_code)
+        return high_ticks.value, low_ticks.value
 
-        return val.value
+    def read_ctr_time(
+            self, task, num_samps_per_chan, timeout, interleaved,
+            read_array_high_time, read_array_low_time):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_open_thrmcpl_detect_enable.setter
-    def ai_open_thrmcpl_detect_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIOpenThrmcplDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadCtrTime
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_open_thrmcpl_detect_enable.deleter
-    def ai_open_thrmcpl_detect_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIOpenThrmcplDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')),
+                        wrapped_ndpointer(dtype=numpy.float64,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, interleaved,
+            read_array_high_time, read_array_low_time,
+            read_array_low_time.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array_high_time, read_array_low_time, samps_per_chan_read.value
 
-    @property
-    def ai_overcurrent_detect_enable(self):
-        """
-        bool: Specifies whether to enable overcurrent detection.
-        """
-        val = c_bool32()
+    def read_ctr_time_scalar(self, task, timeout):
+        high_time = ctypes.c_double()
+        low_time = ctypes.c_double()
 
-        cfunc = lib_importer.windll.DAQmxGetAIOvercurrentDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadCtrTimeScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_double),
+                        ctypes.POINTER(ctypes.c_double),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(high_time), ctypes.byref(low_time),
+            None)
+        self.check_for_error(error_code)
+        return high_time.value, low_time.value
 
-        return val.value
+    def read_digital_lines(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
+        num_bytes_per_samp = ctypes.c_int()
 
-    @ai_overcurrent_detect_enable.setter
-    def ai_overcurrent_detect_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIOvercurrentDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadDigitalLines
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=bool, flags=('C','W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read),
+            ctypes.byref(num_bytes_per_samp), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value, num_bytes_per_samp.value
 
-    @ai_overcurrent_detect_enable.deleter
-    def ai_overcurrent_detect_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIOvercurrentDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def read_digital_scalar_u32(self, task, timeout):
+        value = ctypes.c_uint()
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_power_supply_fault_detect_enable(self):
-        """
-        bool: Specifies whether to enable power supply fault detection.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIPowerSupplyFaultDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadDigitalScalarU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_uint),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(value), None)
+        self.check_for_error(error_code)
+        return value.value
 
-        return val.value
+    def read_digital_u16(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_power_supply_fault_detect_enable.setter
-    def ai_power_supply_fault_detect_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIPowerSupplyFaultDetectEnable
+        cfunc = lib_importer.windll.DAQmxReadDigitalU16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint16,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-    @ai_power_supply_fault_detect_enable.deleter
-    def ai_power_supply_fault_detect_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAIPowerSupplyFaultDetectEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+    def read_digital_u32(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @property
-    def ai_pressure_units(self):
-        """
-        :class:`nidaqmx.constants.PressureUnits`: Specifies  in which
-            unit to return pressure measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIPressureUnits
+        cfunc = lib_importer.windll.DAQmxReadDigitalU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32,
+                        flags=('C','W')), ctypes.c_uint,
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return PressureUnits(val.value)
-
-    @ai_pressure_units.setter
-    def ai_pressure_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIPressureUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def read_digital_u8(
+            self, task, num_samps_per_chan, timeout, fill_mode, read_array):
+        samps_per_chan_read = ctypes.c_int()
 
-    @ai_pressure_units.deleter
-    def ai_pressure_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIPressureUnits
+        cfunc = lib_importer.windll.DAQmxReadDigitalU8
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_probe_atten(self):
-        """
-        float: Specifies the amount of attenuation provided by the probe
-            connected to the channel. Specify this attenuation as a
-            ratio.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIProbeAtten
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_probe_atten.setter
-    def ai_probe_atten(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIProbeAtten
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_probe_atten.deleter
-    def ai_probe_atten(self):
-        cfunc = lib_importer.windll.DAQmxResetAIProbeAtten
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_raw_data_compression_type(self):
-        """
-        :class:`nidaqmx.constants.RawDataCompressionType`: Specifies the
-            type of compression to apply to raw samples returned from
-            the device.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRawDataCompressionType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return RawDataCompressionType(val.value)
-
-    @ai_raw_data_compression_type.setter
-    def ai_raw_data_compression_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIRawDataCompressionType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_raw_data_compression_type.deleter
-    def ai_raw_data_compression_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRawDataCompressionType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_raw_samp_justification(self):
-        """
-        :class:`nidaqmx.constants.DataJustification`: Indicates the
-            justification of a raw sample from the device.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRawSampJustification
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return DataJustification(val.value)
-
-    @property
-    def ai_raw_samp_size(self):
-        """
-        int: Indicates in bits the size of a raw sample from the device.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRawSampSize
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @property
-    def ai_remove_filter_delay(self):
-        """
-        bool: Specifies if filter delay removal is enabled on the
-            device.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRemoveFilterDelay
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_int,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint8, flags=('C','W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_remove_filter_delay.setter
-    def ai_remove_filter_delay(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRemoveFilterDelay
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+            task, num_samps_per_chan, timeout, fill_mode, read_array,
+            read_array.size, ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
+        return read_array, samps_per_chan_read.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def read_power_scalar_f64(self, task, timeout):
+        voltage = ctypes.c_double()
+        current = ctypes.c_double()
 
-    @ai_remove_filter_delay.deleter
-    def ai_remove_filter_delay(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRemoveFilterDelay
+        cfunc = lib_importer.windll.DAQmxReadPowerScalarF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_double,
+                        ctypes.POINTER(ctypes.c_double),
+                        ctypes.POINTER(ctypes.c_double),
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, timeout, ctypes.byref(voltage), ctypes.byref(current), None)
+        self.check_for_error(error_code)
+        return voltage.value, current.value
 
-    @property
-    def ai_resistance_cfg(self):
-        """
-        :class:`nidaqmx.constants.ResistanceConfiguration`: Specifies
-            the resistance configuration for the channel. NI-DAQmx uses
-            this value for any resistance-based measurements, including
-            temperature measurement using a thermistor or RTD.
-        """
-        val = ctypes.c_int()
+    def register_done_event(
+            self, task, options, callback_function, callback_data):
+        DAQmxDoneEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_void_p)
 
-        cfunc = lib_importer.windll.DAQmxGetAIResistanceCfg
+        cfunc = lib_importer.windll.DAQmxRegisterDoneEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_uint,
+                        DAQmxDoneEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ResistanceConfiguration(val.value)
-
-    @ai_resistance_cfg.setter
-    def ai_resistance_cfg(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIResistanceCfg
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        assert callback_function is not None
+        callback_method_ptr = DAQmxDoneEventCallbackPtr(callback_function)
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_resistance_cfg.deleter
-    def ai_resistance_cfg(self):
-        cfunc = lib_importer.windll.DAQmxResetAIResistanceCfg
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+            task, options, callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        return LibraryEventHandler(callback_method_ptr)
 
-    @property
-    def ai_resistance_units(self):
-        """
-        :class:`nidaqmx.constants.ResistanceUnits`: Specifies the units
-            to use to return resistance measurements.
-        """
-        val = ctypes.c_int()
+    def register_every_n_samples_event(
+            self, task, every_n_samples_event_type, n_samples, options,
+            callback_function, callback_data):
+        DAQmxEveryNSamplesEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_uint, ctypes.c_void_p)
 
-        cfunc = lib_importer.windll.DAQmxGetAIResistanceUnits
+        cfunc = lib_importer.windll.DAQmxRegisterEveryNSamplesEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
+                        ctypes.c_uint, DAQmxEveryNSamplesEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-        return ResistanceUnits(val.value)
-
-    @ai_resistance_units.setter
-    def ai_resistance_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIResistanceUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        assert callback_function is not None
+        callback_method_ptr = DAQmxEveryNSamplesEventCallbackPtr(callback_function)
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, every_n_samples_event_type, n_samples, options,
+            callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-    @ai_resistance_units.deleter
-    def ai_resistance_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIResistanceUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        return LibraryEventHandler(callback_method_ptr)
 
-    @property
-    def ai_resolution(self):
-        """
-        float: Indicates the resolution of the analog-to-digital
-            converter of the channel. This value is in the units you
-            specify with **ai_resolution_units**.
-        """
-        val = ctypes.c_double()
+    def register_signal_event(
+            self, task, signal_id, options, callback_function, callback_data):
+        DAQmxSignalEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_void_p)
 
-        cfunc = lib_importer.windll.DAQmxGetAIResolution
+        cfunc = lib_importer.windll.DAQmxRegisterSignalEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
+                        DAQmxSignalEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-    @property
-    def ai_resolution_units(self):
-        """
-        :class:`nidaqmx.constants.ResolutionType`: Indicates the units
-            of **ai_resolution**.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIResolutionUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+        assert callback_function is not None
+        callback_method_ptr = DAQmxSignalEventCallbackPtr(callback_function)
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, signal_id, options, callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-        return ResolutionType(val.value)
+        return LibraryEventHandler(callback_method_ptr)
 
-    @property
-    def ai_rng_high(self):
-        """
-        float: Specifies the upper limit of the input range of the
-            device. This value is in the native units of the device. On
-            E Series devices, for example, the native units is volts.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRngHigh
+    def remove_cdaq_sync_connection(self, port_list):
+        cfunc = lib_importer.windll.DAQmxRemoveCDAQSyncConnection
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            port_list)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_rng_high.setter
-    def ai_rng_high(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRngHigh
+    def reserve_network_device(self, device_name, override_reservation):
+        cfunc = lib_importer.windll.DAQmxReserveNetworkDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, c_bool32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name, override_reservation)
+        self.check_for_error(error_code)
 
-    @ai_rng_high.deleter
-    def ai_rng_high(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRngHigh
+    def reset_buffer_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetBufferAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rng_low(self):
-        """
-        float: Specifies the lower limit of the input range of the
-            device. This value is in the native units of the device. On
-            E Series devices, for example, the native units is volts.
-        """
-        val = ctypes.c_double()
+            task, attribute)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIRngLow
+    def reset_chan_attribute(self, task, channel, attribute):
+        cfunc = lib_importer.windll.DAQmxResetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, channel, attribute)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_rng_low.setter
-    def ai_rng_low(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRngLow
+    def reset_device(self, device_name):
+        cfunc = lib_importer.windll.DAQmxResetDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rng_low.deleter
-    def ai_rng_low(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRngLow
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rosette_strain_gage_gage_orientation(self):
-        """
-        float: Specifies gage orientation in degrees with respect to the
-            X axis.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRosetteStrainGageOrientation
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            device_name)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_rosette_strain_gage_gage_orientation.setter
-    def ai_rosette_strain_gage_gage_orientation(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRosetteStrainGageOrientation
+    def reset_exported_signal_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute)
+        self.check_for_error(error_code)
 
-    @ai_rosette_strain_gage_gage_orientation.deleter
-    def ai_rosette_strain_gage_gage_orientation(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRosetteStrainGageOrientation
+    def reset_read_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rosette_strain_gage_rosette_meas_type(self):
-        """
-        :class:`nidaqmx.constants.StrainGageRosetteMeasurementType`:
-            Specifies the type of rosette measurement.
-        """
-        val = ctypes.c_int()
+            task, attribute)
+        self.check_for_error(error_code)
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIRosetteStrainGageRosetteMeasType)
+    def reset_timing_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute)
+        self.check_for_error(error_code)
 
-        return StrainGageRosetteMeasurementType(val.value)
-
-    @ai_rosette_strain_gage_rosette_meas_type.setter
-    def ai_rosette_strain_gage_rosette_meas_type(self, val):
-        val = val.value
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIRosetteStrainGageRosetteMeasType)
+    def reset_timing_attribute_ex(self, task, device_names, attribute):
+        cfunc = lib_importer.windll.DAQmxResetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
                         ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rosette_strain_gage_rosette_meas_type.deleter
-    def ai_rosette_strain_gage_rosette_meas_type(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIRosetteStrainGageRosetteMeasType)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rosette_strain_gage_rosette_type(self):
-        """
-        :class:`nidaqmx.constants.StrainGageRosetteType`: Indicates the
-            type of rosette gage.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRosetteStrainGageRosetteType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return StrainGageRosetteType(val.value)
-
-    @property
-    def ai_rosette_strain_gage_strain_chans(self):
-        """
-        List[str]: Indicates the raw strain channels that comprise the
-            strain rosette.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIRosetteStrainGageStrainChans
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_char_p, ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return unflatten_channel_string(val.value.decode('ascii'))
-
-    @property
-    def ai_rtd_a(self):
-        """
-        float: Specifies the 'A' constant of the Callendar-Van Dusen
-            equation. NI-DAQmx requires this value when you use a custom
-            RTD.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRTDA
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_rtd_a.setter
-    def ai_rtd_a(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRTDA
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rtd_a.deleter
-    def ai_rtd_a(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRTDA
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rtd_b(self):
-        """
-        float: Specifies the 'B' constant of the Callendar-Van Dusen
-            equation. NI-DAQmx requires this value when you use a custom
-            RTD.
-        """
-        val = ctypes.c_double()
+            task, device_names, attribute)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIRTDB
+    def reset_trig_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute)
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_rtd_b.setter
-    def ai_rtd_b(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRTDB
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rtd_b.deleter
-    def ai_rtd_b(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRTDB
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rtd_c(self):
-        """
-        float: Specifies the 'C' constant of the Callendar-Van Dusen
-            equation. NI-DAQmx requires this value when you use a custom
-            RTD.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRTDC
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_rtd_c.setter
-    def ai_rtd_c(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRTDC
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rtd_c.deleter
-    def ai_rtd_c(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRTDC
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rtd_r0(self):
-        """
-        float: Specifies in ohms the sensor resistance at 0 deg C. The
-            Callendar-Van Dusen equation requires this value. Refer to
-            the sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRTDR0
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_rtd_r0.setter
-    def ai_rtd_r0(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRTDR0
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rtd_r0.deleter
-    def ai_rtd_r0(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRTDR0
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rtd_type(self):
-        """
-        :class:`nidaqmx.constants.RTDType`: Specifies the type of RTD
-            connected to the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRTDType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return RTDType(val.value)
-
-    @ai_rtd_type.setter
-    def ai_rtd_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIRTDType
+    def reset_watchdog_attribute(self, task, lines, attribute):
+        cfunc = lib_importer.windll.DAQmxResetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
                         ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_rtd_type.deleter
-    def ai_rtd_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRTDType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, lines, attribute)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_rvdt_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the RVDT. This value is in
-            the units you specify with **ai_rvdt_sensitivity_units**.
-            Refer to the sensor documentation to determine this value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIRVDTSensitivity
+    def reset_write_attribute(self, task, attribute):
+        cfunc = lib_importer.windll.DAQmxResetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, attribute)
+        self.check_for_error(error_code)
 
-    @ai_rvdt_sensitivity.setter
-    def ai_rvdt_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIRVDTSensitivity
+    def save_global_chan(self, task, channel_name, save_as, author, options):
+        cfunc = lib_importer.windll.DAQmxSaveGlobalChan
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes_byte_str, ctypes.c_uint32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, channel_name, save_as, author, options)
+        self.check_for_error(error_code)
 
-    @ai_rvdt_sensitivity.deleter
-    def ai_rvdt_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRVDTSensitivity
+    def save_scale(self, scale_name, save_as, author, options):
+        cfunc = lib_importer.windll.DAQmxSaveScale
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes_byte_str, ctypes_byte_str,
+                        ctypes.c_uint32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rvdt_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.RVDTSensitivityUnits`: Specifies the
-            units of **ai_rvdt_sensitivity**.
-        """
-        val = ctypes.c_int()
+            scale_name, save_as, author, options)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIRVDTSensitivityUnits
+    def save_task(self, task, save_as, author, options):
+        cfunc = lib_importer.windll.DAQmxSaveTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes_byte_str, ctypes.c_uint32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, save_as, author, options)
+        self.check_for_error(error_code)
 
-        return RVDTSensitivityUnits(val.value)
-
-    @ai_rvdt_sensitivity_units.setter
-    def ai_rvdt_sensitivity_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIRVDTSensitivityUnits
+    def self_test_device(self, device_name):
+        cfunc = lib_importer.windll.DAQmxSelfTestDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            device_name)
+        self.check_for_error(error_code)
 
-    @ai_rvdt_sensitivity_units.deleter
-    def ai_rvdt_sensitivity_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRVDTSensitivityUnits
+    def set_analog_power_up_states(
+            self, device_name, channel_names, state, channel_type):
+        args = [device_name]
+        argtypes: List[type] = [ctypes_byte_str]
+
+        for index in range(len(channel_names)):
+
+            args.append(channel_names[index])
+            argtypes.append(ctypes_byte_str)
+            
+            args.append(state[index])
+            argtypes.append(ctypes.c_double)
+            
+            args.append(channel_type[index])
+            argtypes.append(ctypes.c_int32)
+            
+        args.append(None)
+        argtypes.append(ctypes.c_void_p)
+
+        cfunc = lib_importer.cdll.DAQmxSetAnalogPowerUpStates
+        with cfunc.arglock:
+            cfunc.argtypes = argtypes
+            error_code = cfunc(*args)
+        self.check_for_error(error_code)
+
+    def set_analog_power_up_states_with_output_type(
+            self, channel_names, state_array, channel_type_array):
+        cfunc = lib_importer.cdll.DAQmxSetAnalogPowerUpStatesWithOutputType
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
+                        ctypes.c_uint]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_rvdt_units(self):
-        """
-        :class:`nidaqmx.constants.AngleUnits`: Specifies the units to
-            use to return angular position measurements from the
-            channel.
-        """
-        val = ctypes.c_int()
+            channel_names, state_array, channel_type_array,
+            len(channel_type_array))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIRVDTUnits
+    def set_buffer_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetBufferAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-        return AngleUnits(val.value)
-
-    @ai_rvdt_units.setter
-    def ai_rvdt_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIRVDTUnits
+    def set_chan_attribute_bool(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, channel, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @ai_rvdt_units.deleter
-    def ai_rvdt_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIRVDTUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_samp_and_hold_enable(self):
-        """
-        bool: Specifies whether to enable the sample and hold circuitry
-            of the device. When you disable sample and hold circuitry, a
-            small voltage offset might be introduced into the signal.
-            You can eliminate this offset by using **ai_auto_zero_mode**
-            to perform an auto zero on the channel.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAISampAndHoldEnable
+    def set_chan_attribute_double(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, channel, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-    @ai_samp_and_hold_enable.setter
-    def ai_samp_and_hold_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAISampAndHoldEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_samp_and_hold_enable.deleter
-    def ai_samp_and_hold_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetAISampAndHoldEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_sensor_power_cfg(self):
-        """
-        :class:`nidaqmx.constants.SensorPowerCfg`: Specifies whether to
-            turn on the sensor's power supply or to leave the
-            configuration unchanged.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAISensorPowerCfg
+    def set_chan_attribute_double_array(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, channel, attribute, value.ctypes.data_as(ctypes.c_void_p),
+            len(value))
+        self.check_for_error(error_code)
 
-        return SensorPowerCfg(val.value)
-
-    @ai_sensor_power_cfg.setter
-    def ai_sensor_power_cfg(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAISensorPowerCfg
+    def set_chan_attribute_int32(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_sensor_power_cfg.deleter
-    def ai_sensor_power_cfg(self):
-        cfunc = lib_importer.windll.DAQmxResetAISensorPowerCfg
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, channel, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_sensor_power_type(self):
-        """
-        :class:`nidaqmx.constants.SensorPowerType`: Specifies the type
-            of power supplied to the sensor.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAISensorPowerType
+    def set_chan_attribute_string(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return SensorPowerType(val.value)
+            task, channel, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @ai_sensor_power_type.setter
-    def ai_sensor_power_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAISensorPowerType
+    def set_chan_attribute_uint32(self, task, channel, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetChanAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, channel, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-    @ai_sensor_power_type.deleter
-    def ai_sensor_power_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAISensorPowerType
+    def set_digital_logic_family_power_up_state(
+            self, device_name, logic_family):
+        cfunc = lib_importer.windll.DAQmxSetDigitalLogicFamilyPowerUpState
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            device_name, logic_family)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_sensor_power_voltage(self):
-        """
-        float: Specifies the voltage level for the sensor's power
-            supply.
-        """
-        val = ctypes.c_double()
+    def set_digital_power_up_states(self, device_name, channel_names, state):
+        args = [device_name]
+        argtypes: List[type] = [ctypes_byte_str]
 
-        cfunc = lib_importer.windll.DAQmxGetAISensorPowerVoltage
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+        for index in range(len(channel_names)):
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            args.append(channel_names[index])
+            argtypes.append(ctypes_byte_str)
+            
+            args.append(state[index])
+            argtypes.append(ctypes.c_int32)
+            
+        args.append(None)
+        argtypes.append(ctypes.c_void_p)
 
-        return val.value
+        cfunc = lib_importer.cdll.DAQmxSetDigitalPowerUpStates
+        with cfunc.arglock:
+            cfunc.argtypes = argtypes
+            error_code = cfunc(*args)
+        self.check_for_error(error_code)
 
-    @ai_sensor_power_voltage.setter
-    def ai_sensor_power_voltage(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAISensorPowerVoltage
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+    def set_digital_pull_up_pull_down_states(
+            self, device_name, channel_names, state):
+        args = [device_name]
+        argtypes: List[type] = [ctypes_byte_str]
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+        for index in range(len(channel_names)):
 
-    @ai_sensor_power_voltage.deleter
-    def ai_sensor_power_voltage(self):
-        cfunc = lib_importer.windll.DAQmxResetAISensorPowerVoltage
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            args.append(channel_names[index])
+            argtypes.append(ctypes_byte_str)
+            
+            args.append(state[index])
+            argtypes.append(ctypes.c_int32)
+            
+        args.append(None)
+        argtypes.append(ctypes.c_void_p)
 
-    @property
-    def ai_sound_pressure_db_ref(self):
-        """
-        float: Specifies the decibel reference level in the units of the
-            channel. When you read samples as a waveform, the decibel
-            reference level is included in the waveform attributes. NI-
-            DAQmx also uses the decibel reference level when converting
-            **ai_sound_pressure_max_sound_pressure_lvl** to a voltage
-            level.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAISoundPressuredBRef
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_sound_pressure_db_ref.setter
-    def ai_sound_pressure_db_ref(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAISoundPressuredBRef
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+        cfunc = lib_importer.cdll.DAQmxSetDigitalPullUpPullDownStates
+        with cfunc.arglock:
+            cfunc.argtypes = argtypes
+            error_code = cfunc(*args)
+        self.check_for_error(error_code)
 
-    @ai_sound_pressure_db_ref.deleter
-    def ai_sound_pressure_db_ref(self):
-        cfunc = lib_importer.windll.DAQmxResetAISoundPressuredBRef
+    def set_exported_signal_attribute_bool(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_sound_pressure_max_sound_pressure_lvl(self):
-        """
-        float: Specifies the maximum instantaneous sound pressure level
-            you expect to measure. This value is in decibels, referenced
-            to 20 micropascals. NI-DAQmx uses the maximum sound pressure
-            level to calculate values in pascals for **ai_max** and
-            **ai_min** for the channel.
-        """
-        val = ctypes.c_double()
+            task, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAISoundPressureMaxSoundPressureLvl)
+    def set_exported_signal_attribute_double(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_sound_pressure_max_sound_pressure_lvl.setter
-    def ai_sound_pressure_max_sound_pressure_lvl(self, val):
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAISoundPressureMaxSoundPressureLvl)
+    def set_exported_signal_attribute_int32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @ai_sound_pressure_max_sound_pressure_lvl.deleter
-    def ai_sound_pressure_max_sound_pressure_lvl(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAISoundPressureMaxSoundPressureLvl)
+    def set_exported_signal_attribute_string(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_sound_pressure_units(self):
-        """
-        :class:`nidaqmx.constants.SoundPressureUnits`: Specifies the
-            units to use to return sound pressure measurements from the
-            channel.
-        """
-        val = ctypes.c_int()
+            task, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAISoundPressureUnits
+    def set_exported_signal_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetExportedSignalAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-        return SoundPressureUnits(val.value)
-
-    @ai_sound_pressure_units.setter
-    def ai_sound_pressure_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAISoundPressureUnits
+    def set_read_attribute_bool(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @ai_sound_pressure_units.deleter
-    def ai_sound_pressure_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAISoundPressureUnits
+    def set_read_attribute_double(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_strain_force_read_from_chan(self):
-        """
-        bool: Specifies whether the data is returned by DAQmx Read when
-            set on a raw strain channel that is part of a rosette
-            configuration.
-        """
-        val = c_bool32()
+            task, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIStrainGageForceReadFromChan
+    def set_read_attribute_int32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_strain_force_read_from_chan.setter
-    def ai_strain_force_read_from_chan(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIStrainGageForceReadFromChan
+    def set_read_attribute_string(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @ai_strain_force_read_from_chan.deleter
-    def ai_strain_force_read_from_chan(self):
-        cfunc = lib_importer.windll.DAQmxResetAIStrainGageForceReadFromChan
+    def set_read_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_strain_gage_cfg(self):
-        """
-        :class:`nidaqmx.constants.StrainGageBridgeType`: Specifies the
-            bridge configuration of the strain gages.
-        """
-        val = ctypes.c_int()
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIStrainGageCfg
+    def set_read_attribute_uint64(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetReadAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return StrainGageBridgeType(val.value)
+            task, attribute, ctypes.c_uint64(value))
+        self.check_for_error(error_code)
 
-    @ai_strain_gage_cfg.setter
-    def ai_strain_gage_cfg(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIStrainGageCfg
+    def set_scale_attribute_double(self, scale_name, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            scale_name, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-    @ai_strain_gage_cfg.deleter
-    def ai_strain_gage_cfg(self):
-        cfunc = lib_importer.windll.DAQmxResetAIStrainGageCfg
+    def set_scale_attribute_double_array(self, scale_name, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            scale_name, attribute, value.ctypes.data_as(ctypes.c_void_p),
+            len(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_strain_gage_gage_factor(self):
-        """
-        float: Specifies the sensitivity of the strain gage.  Gage
-            factor relates the change in electrical resistance to the
-            change in strain. Refer to the sensor documentation for this
-            value.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIStrainGageGageFactor
+    def set_scale_attribute_int32(self, scale_name, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            scale_name, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @ai_strain_gage_gage_factor.setter
-    def ai_strain_gage_gage_factor(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIStrainGageGageFactor
+    def set_scale_attribute_string(self, scale_name, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetScaleAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            scale_name, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @ai_strain_gage_gage_factor.deleter
-    def ai_strain_gage_gage_factor(self):
-        cfunc = lib_importer.windll.DAQmxResetAIStrainGageGageFactor
+    def set_timing_attribute_bool(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_strain_gage_poisson_ratio(self):
-        """
-        float: Specifies the ratio of lateral strain to axial strain in
-            the material you are measuring.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIStrainGagePoissonRatio
+    def set_timing_attribute_double(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_strain_gage_poisson_ratio.setter
-    def ai_strain_gage_poisson_ratio(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIStrainGagePoissonRatio
+    def set_timing_attribute_ex_bool(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_strain_gage_poisson_ratio.deleter
-    def ai_strain_gage_poisson_ratio(self):
-        cfunc = lib_importer.windll.DAQmxResetAIStrainGagePoissonRatio
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, device_names, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_strain_units(self):
-        """
-        :class:`nidaqmx.constants.StrainUnits`: Specifies the units to
-            use to return strain measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIStrainUnits
+    def set_timing_attribute_ex_double(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return StrainUnits(val.value)
+            task, device_names, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-    @ai_strain_units.setter
-    def ai_strain_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIStrainUnits
+    def set_timing_attribute_ex_int32(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @ai_strain_units.deleter
-    def ai_strain_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIStrainUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_teds_is_teds(self):
-        """
-        bool: Indicates if the virtual channel was initialized using a
-            TEDS bitstream from the corresponding physical channel.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetAIIsTEDS
+    def set_timing_attribute_ex_string(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(c_bool32)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @property
-    def ai_teds_units(self):
-        """
-        str: Indicates the units defined by TEDS information associated
-            with the channel.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAITEDSUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_char_p, ctypes.c_uint]
+            task, device_names, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.value.decode('ascii')
-
-    @property
-    def ai_temp_units(self):
-        """
-        :class:`nidaqmx.constants.TemperatureUnits`: Specifies the units
-            to use to return temperature measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAITempUnits
+    def set_timing_attribute_ex_uint32(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-        return TemperatureUnits(val.value)
-
-    @ai_temp_units.setter
-    def ai_temp_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAITempUnits
+    def set_timing_attribute_ex_uint64(
+            self, task, device_names, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttributeEx
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, device_names, attribute, ctypes.c_uint64(value))
+        self.check_for_error(error_code)
 
-    @ai_temp_units.deleter
-    def ai_temp_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAITempUnits
+    def set_timing_attribute_int32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_term_cfg(self):
-        """
-        :class:`nidaqmx.constants.TerminalConfiguration`: Specifies the
-            terminal configuration for the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAITermCfg
+    def set_timing_attribute_string(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-        return TerminalConfiguration(val.value)
-
-    @ai_term_cfg.setter
-    def ai_term_cfg(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAITermCfg
+    def set_timing_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-    @ai_term_cfg.deleter
-    def ai_term_cfg(self):
-        cfunc = lib_importer.windll.DAQmxResetAITermCfg
+    def set_timing_attribute_uint64(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTimingAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint64(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_thrmcpl_cjc_chan(self):
-        """
-        :class:`nidaqmx._task_modules.channels.channel.Channel`:
-            Indicates the channel that acquires the temperature of the
-            cold junction if **ai_thrmcpl_cjc_src** is
-            **CJCSource1.SCANNABLE_CHANNEL**. If the channel is a
-            temperature channel, NI-DAQmx acquires the temperature in
-            the correct units. Other channel types, such as a resistance
-            channel with a custom sensor, must use a custom scale to
-            scale values to degrees Celsius.
-        """
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplCJCChan
+    def set_trig_attribute_bool(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_char_p, ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return Channel._factory(self._handle, val.value.decode('ascii'))
-
-    @property
-    def ai_thrmcpl_cjc_src(self):
-        """
-        :class:`nidaqmx.constants.CJCSource`: Indicates the source of
-            cold-junction compensation.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplCJCSrc
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return CJCSource(val.value)
+            task, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_thrmcpl_cjc_val(self):
-        """
-        float: Specifies the temperature of the cold junction if
-            **ai_thrmcpl_cjc_src** is
-            **CJCSource1.CONSTANT_USER_VALUE**. Specify this value in
-            the units of the measurement.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplCJCVal
+    def set_trig_attribute_double(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-        return val.value
-
-    @ai_thrmcpl_cjc_val.setter
-    def ai_thrmcpl_cjc_val(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmcplCJCVal
+    def set_trig_attribute_double_array(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, value.ctypes.data_as(ctypes.c_void_p), len(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_cjc_val.deleter
-    def ai_thrmcpl_cjc_val(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmcplCJCVal
+    def set_trig_attribute_int32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_thrmcpl_lead_offset_voltage(self):
-        """
-        float: Specifies the lead offset nulling voltage to subtract
-            from measurements on a device. This property is ignored if
-            open thermocouple detection is disabled.
-        """
-        val = ctypes.c_double()
+            task, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplLeadOffsetVoltage
+    def set_trig_attribute_int32_array(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, attribute, value.ctypes.data_as(ctypes.c_void_p), len(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_lead_offset_voltage.setter
-    def ai_thrmcpl_lead_offset_voltage(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmcplLeadOffsetVoltage
+    def set_trig_attribute_string(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_lead_offset_voltage.deleter
-    def ai_thrmcpl_lead_offset_voltage(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmcplLeadOffsetVoltage
+    def set_trig_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetTrigAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_thrmcpl_scale_type(self):
-        """
-        :class:`nidaqmx.constants.ScaleType`: Specifies the method or
-            equation form that the thermocouple scale uses.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplScaleType
+    def set_watchdog_attribute_bool(self, task, lines, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ScaleType(val.value)
+            task, lines, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_scale_type.setter
-    def ai_thrmcpl_scale_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIThrmcplScaleType
+    def set_watchdog_attribute_double(self, task, lines, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, lines, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_scale_type.deleter
-    def ai_thrmcpl_scale_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmcplScaleType
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_thrmcpl_type(self):
-        """
-        :class:`nidaqmx.constants.ThermocoupleType`: Specifies the type
-            of thermocouple connected to the channel. Thermocouple types
-            differ in composition and measurement range.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmcplType
+    def set_watchdog_attribute_int32(self, task, lines, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return ThermocoupleType(val.value)
+            task, lines, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_type.setter
-    def ai_thrmcpl_type(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIThrmcplType
+    def set_watchdog_attribute_string(self, task, lines, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWatchdogAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, lines, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @ai_thrmcpl_type.deleter
-    def ai_thrmcpl_type(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmcplType
+    def set_write_attribute_bool(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_thrmstr_a(self):
-        """
-        float: Specifies the 'A' constant of the Steinhart-Hart
-            thermistor equation.
-        """
-        val = ctypes.c_double()
+            task, attribute, c_bool32(value))
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIThrmstrA
+    def set_write_attribute_double(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, attribute, ctypes.c_double(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_a.setter
-    def ai_thrmstr_a(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmstrA
+    def set_write_attribute_int32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_int32(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_a.deleter
-    def ai_thrmstr_a(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmstrA
+    def set_write_attribute_string(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, attribute, value.encode('ascii'))
+        self.check_for_error(error_code)
 
-    @property
-    def ai_thrmstr_b(self):
-        """
-        float: Specifies the 'B' constant of the Steinhart-Hart
-            thermistor equation.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmstrB
+    def set_write_attribute_uint32(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, attribute, ctypes.c_uint32(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_b.setter
-    def ai_thrmstr_b(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmstrB
+    def set_write_attribute_uint64(self, task, attribute, value):
+        cfunc = lib_importer.cdll.DAQmxSetWriteAttribute
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int32]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, attribute, ctypes.c_uint64(value))
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_b.deleter
-    def ai_thrmstr_b(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmstrB
+    def start_new_file(self, task, file_path):
+        cfunc = lib_importer.windll.DAQmxStartNewFile
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
                         lib_importer.task_handle, ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_thrmstr_c(self):
-        """
-        float: Specifies the 'C' constant of the Steinhart-Hart
-            thermistor equation.
-        """
-        val = ctypes.c_double()
+            task, file_path)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIThrmstrC
+    def start_task(self, task):
+        cfunc = lib_importer.windll.DAQmxStartTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task)
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_c.setter
-    def ai_thrmstr_c(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmstrC
+    def stop_task(self, task):
+        cfunc = lib_importer.windll.DAQmxStopTask
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task)
+        self.check_for_error(error_code)
 
-    @ai_thrmstr_c.deleter
-    def ai_thrmstr_c(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmstrC
+    def task_control(self, task, action):
+        cfunc = lib_importer.windll.DAQmxTaskControl
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, action)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_thrmstr_r1(self):
-        """
-        float: Specifies in ohms the value of the reference resistor for
-            the thermistor if you use voltage excitation. NI-DAQmx
-            ignores this value for current excitation.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetAIThrmstrR1
+    def tristate_output_term(self, output_terminal):
+        cfunc = lib_importer.windll.DAQmxTristateOutputTerm
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            output_terminal)
+        self.check_for_error(error_code)
 
-        return val.value
+    def unregister_done_event(self, task):
+        DAQmxDoneEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_void_p)
 
-    @ai_thrmstr_r1.setter
-    def ai_thrmstr_r1(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIThrmstrR1
+        cfunc = lib_importer.windll.DAQmxRegisterDoneEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_uint,
+                        DAQmxDoneEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_thrmstr_r1.deleter
-    def ai_thrmstr_r1(self):
-        cfunc = lib_importer.windll.DAQmxResetAIThrmstrR1
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+        options = 0
+        callback_method_ptr = DAQmxDoneEventCallbackPtr()  # type: ignore  # typeshed is missing no-argument constructor overload
+        callback_data = None
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, options, callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_torque_units(self):
-        """
-        :class:`nidaqmx.constants.TorqueUnits`: Specifies in which unit
-            to return torque measurements from the channel.
-        """
-        val = ctypes.c_int()
+    def unregister_every_n_samples_event(
+            self, task, every_n_samples_event_type):
+        DAQmxEveryNSamplesEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_uint, ctypes.c_void_p)
 
-        cfunc = lib_importer.windll.DAQmxGetAITorqueUnits
+        cfunc = lib_importer.windll.DAQmxRegisterEveryNSamplesEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
-
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return TorqueUnits(val.value)
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
+                        ctypes.c_uint, DAQmxEveryNSamplesEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-    @ai_torque_units.setter
-    def ai_torque_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAITorqueUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        n_samples = 0
+        options = 0
+        callback_method_ptr = DAQmxEveryNSamplesEventCallbackPtr()  # type: ignore  # typeshed is missing no-argument constructor overload
+        callback_data = None
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, every_n_samples_event_type, n_samples, options,
+            callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-    @ai_torque_units.deleter
-    def ai_torque_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAITorqueUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def unregister_signal_event(self, task, signal_id):
+        DAQmxSignalEventCallbackPtr = ctypes.CFUNCTYPE(
+            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int,
+            ctypes.c_void_p)
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_usb_xfer_req_count(self):
-        """
-        int: Specifies the maximum number of simultaneous USB transfers
-            used to stream data. Modify this value to affect performance
-            under different combinations of operating system and device.
-        """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetAIUsbXferReqCount
+        cfunc = lib_importer.windll.DAQmxRegisterSignalEvent
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
+                        DAQmxSignalEventCallbackPtr,
+                        ctypes.POINTER(ctypes.c_void_p)]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_usb_xfer_req_count.setter
-    def ai_usb_xfer_req_count(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIUsbXferReqCount
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
+        options = 0
+        callback_method_ptr = DAQmxSignalEventCallbackPtr()  # type: ignore  # typeshed is missing no-argument constructor overload
+        callback_data = None
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, signal_id, options, callback_method_ptr, callback_data)
+        self.check_for_error(error_code)
 
-    @ai_usb_xfer_req_count.deleter
-    def ai_usb_xfer_req_count(self):
-        cfunc = lib_importer.windll.DAQmxResetAIUsbXferReqCount
+    def unreserve_network_device(self, device_name):
+        cfunc = lib_importer.windll.DAQmxUnreserveNetworkDevice
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_usb_xfer_req_size(self):
-        """
-        int: Specifies the maximum size of a USB transfer request in
-            bytes. Modify this value to affect performance under
-            different combinations of operating system and device.
-        """
-        val = ctypes.c_uint()
+            device_name)
+        self.check_for_error(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetAIUsbXferReqSize
+    def wait_until_task_done(self, task, time_to_wait):
+        cfunc = lib_importer.windll.DAQmxWaitUntilTaskDone
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_uint)]
+                        lib_importer.task_handle, ctypes.c_double]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, time_to_wait)
+        self.check_for_error(error_code)
 
-        return val.value
+    def write_analog_f64(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-    @ai_usb_xfer_req_size.setter
-    def ai_usb_xfer_req_size(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIUsbXferReqSize
+        cfunc = lib_importer.windll.DAQmxWriteAnalogF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_uint]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-    @ai_usb_xfer_req_size.deleter
-    def ai_usb_xfer_req_size(self):
-        cfunc = lib_importer.windll.DAQmxResetAIUsbXferReqSize
+    def write_analog_scalar_f64(self, task, auto_start, timeout, value):
+        cfunc = lib_importer.windll.DAQmxWriteAnalogScalarF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, c_bool32, ctypes.c_double,
+                        ctypes.c_double, ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, auto_start, timeout, value, None)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_velocity_iepe_sensor_db_ref(self):
-        """
-        float: Specifies the decibel reference level in the units of the
-            channel. When you read samples as a waveform, the decibel
-            reference level is included in the waveform attributes.
-        """
-        val = ctypes.c_double()
+    def write_binary_i16(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIVelocityIEPESensordBRef
+        cfunc = lib_importer.windll.DAQmxWriteBinaryI16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.int16, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @ai_velocity_iepe_sensor_db_ref.setter
-    def ai_velocity_iepe_sensor_db_ref(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIVelocityIEPESensordBRef
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def write_binary_i32(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-    @ai_velocity_iepe_sensor_db_ref.deleter
-    def ai_velocity_iepe_sensor_db_ref(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVelocityIEPESensordBRef
+        cfunc = lib_importer.windll.DAQmxWriteBinaryI32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.int32, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-    @property
-    def ai_velocity_iepe_sensor_sensitivity(self):
-        """
-        float: Specifies the sensitivity of the IEPE velocity sensor
-            connected to the channel. Specify this value in the unit
-            indicated by **ai_velocity_iepe_sensor_sensitivity_units**.
-        """
-        val = ctypes.c_double()
+    def write_binary_u16(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIVelocityIEPESensorSensitivity
+        cfunc = lib_importer.windll.DAQmxWriteBinaryU16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint16, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-        return val.value
+    def write_binary_u32(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-    @ai_velocity_iepe_sensor_sensitivity.setter
-    def ai_velocity_iepe_sensor_sensitivity(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIVelocityIEPESensorSensitivity
+        cfunc = lib_importer.windll.DAQmxWriteBinaryU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-    @ai_velocity_iepe_sensor_sensitivity.deleter
-    def ai_velocity_iepe_sensor_sensitivity(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVelocityIEPESensorSensitivity
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_velocity_iepe_sensor_sensitivity_units(self):
-        """
-        :class:`nidaqmx.constants.VelocityIEPESensorSensitivityUnits`:
-            Specifies the units for
-            **ai_velocity_iepe_sensor_sensitivity**.
-        """
-        val = ctypes.c_int()
+    def write_ctr_freq(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            frequency, duty_cycle):
+        num_samps_per_chan_written = ctypes.c_int()
 
-        cfunc = (lib_importer.windll.
-                 DAQmxGetAIVelocityIEPESensorSensitivityUnits)
+        cfunc = lib_importer.windll.DAQmxWriteCtrFreq
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return VelocityIEPESensorSensitivityUnits(val.value)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            frequency, duty_cycle, ctypes.byref(num_samps_per_chan_written),
+            None)
+        self.check_for_error(error_code, samps_per_chan_written=num_samps_per_chan_written.value)
+        return num_samps_per_chan_written.value
 
-    @ai_velocity_iepe_sensor_sensitivity_units.setter
-    def ai_velocity_iepe_sensor_sensitivity_units(self, val):
-        val = val.value
-        cfunc = (lib_importer.windll.
-                 DAQmxSetAIVelocityIEPESensorSensitivityUnits)
+    def write_ctr_freq_scalar(
+            self, task, auto_start, timeout, frequency, duty_cycle):
+        cfunc = lib_importer.windll.DAQmxWriteCtrFreqScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_velocity_iepe_sensor_sensitivity_units.deleter
-    def ai_velocity_iepe_sensor_sensitivity_units(self):
-        cfunc = (lib_importer.windll.
-                 DAQmxResetAIVelocityIEPESensorSensitivityUnits)
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_velocity_units(self):
-        """
-        :class:`nidaqmx.constants.VelocityUnits`: Specifies in which
-            unit to return velocity measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIVelocityUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, c_bool32, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double,
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, auto_start, timeout, frequency, duty_cycle, None)
+        self.check_for_error(error_code)
 
-        return VelocityUnits(val.value)
+    def write_ctr_ticks(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            high_ticks, low_ticks):
+        num_samps_per_chan_written = ctypes.c_int()
 
-    @ai_velocity_units.setter
-    def ai_velocity_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIVelocityUnits
+        cfunc = lib_importer.windll.DAQmxWriteCtrTicks
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32, flags=('C')),
+                        wrapped_ndpointer(dtype=numpy.uint32, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            high_ticks, low_ticks, ctypes.byref(num_samps_per_chan_written),
+            None)
+        self.check_for_error(error_code, samps_per_chan_written=num_samps_per_chan_written.value)
+        return num_samps_per_chan_written.value
 
-    @ai_velocity_units.deleter
-    def ai_velocity_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVelocityUnits
+    def write_ctr_ticks_scalar(
+            self, task, auto_start, timeout, high_ticks, low_ticks):
+        cfunc = lib_importer.windll.DAQmxWriteCtrTicksScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, c_bool32, ctypes.c_double,
+                        ctypes.c_uint, ctypes.c_uint, ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, auto_start, timeout, high_ticks, low_ticks, None)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_voltage_acrms_units(self):
-        """
-        :class:`nidaqmx.constants.VoltageUnits`: Specifies the units to
-            use to return voltage RMS measurements from the channel.
-        """
-        val = ctypes.c_int()
+    def write_ctr_time(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            high_time, low_time):
+        num_samps_per_chan_written = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIVoltageACRMSUnits
+        cfunc = lib_importer.windll.DAQmxWriteCtrTime
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return VoltageUnits(val.value)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            high_time, low_time, ctypes.byref(num_samps_per_chan_written),
+            None)
+        self.check_for_error(error_code, samps_per_chan_written=num_samps_per_chan_written.value)
+        return num_samps_per_chan_written.value
 
-    @ai_voltage_acrms_units.setter
-    def ai_voltage_acrms_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIVoltageACRMSUnits
+    def write_ctr_time_scalar(
+            self, task, auto_start, timeout, high_time, low_time):
+        cfunc = lib_importer.windll.DAQmxWriteCtrTimeScalar
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_voltage_acrms_units.deleter
-    def ai_voltage_acrms_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVoltageACRMSUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, c_bool32, ctypes.c_double,
+                        ctypes.c_double, ctypes.c_double,
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task, auto_start, timeout, high_time, low_time, None)
+        self.check_for_error(error_code)
 
-    @property
-    def ai_voltage_db_ref(self):
-        """
-        float: Specifies the decibel reference level in the units of the
-            channel. When you read samples as a waveform, the decibel
-            reference level is included in the waveform attributes.
-        """
-        val = ctypes.c_double()
+    def write_digital_lines(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetAIVoltagedBRef
+        cfunc = lib_importer.windll.DAQmxWriteDigitalLines
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=bool, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-    @ai_voltage_db_ref.setter
-    def ai_voltage_db_ref(self, val):
-        cfunc = lib_importer.windll.DAQmxSetAIVoltagedBRef
+    def write_digital_scalar_u32(self, task, auto_start, timeout, value):
+        cfunc = lib_importer.windll.DAQmxWriteDigitalScalarU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        lib_importer.task_handle, c_bool32, ctypes.c_double,
+                        ctypes.c_uint, ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, auto_start, timeout, value, None)
+        self.check_for_error(error_code)
 
-    @ai_voltage_db_ref.deleter
-    def ai_voltage_db_ref(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVoltagedBRef
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def write_digital_u16(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def ai_voltage_units(self):
-        """
-        :class:`nidaqmx.constants.VoltageUnits`: Specifies the units to
-            use to return voltage measurements from the channel.
-        """
-        val = ctypes.c_int()
-
-        cfunc = lib_importer.windll.DAQmxGetAIVoltageUnits
+        cfunc = lib_importer.windll.DAQmxWriteDigitalU16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint16, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-        return VoltageUnits(val.value)
+    def write_digital_u32(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-    @ai_voltage_units.setter
-    def ai_voltage_units(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetAIVoltageUnits
+        cfunc = lib_importer.windll.DAQmxWriteDigitalU32
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint32, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @ai_voltage_units.deleter
-    def ai_voltage_units(self):
-        cfunc = lib_importer.windll.DAQmxResetAIVoltageUnits
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def pwr_current_dev_scaling_coeff(self):
-        """
-        List[float]: Indicates the coefficients of the polynomial
-            equation that NI-DAQmx uses to scale values from the native
-            format of the device to amperes. Can be read at any time
-            during a task.
-        """
-        cfunc = lib_importer.windll.DAQmxGetPwrCurrentDevScalingCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
+    def write_digital_u8(
+            self, task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array):
+        samps_per_chan_written = ctypes.c_int()
 
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.tolist()
-
-    @property
-    def pwr_current_setpoint(self):
-        """
-        float: Specifies the output current, in amperes. If the load
-            draws current greater than the specified value, the device
-            will operate in Constant Current mode.
-        """
-        val = ctypes.c_double()
-
-        cfunc = lib_importer.windll.DAQmxGetPwrCurrentSetpoint
+        cfunc = lib_importer.windll.DAQmxWriteDigitalU8
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double, ctypes.c_int,
+                        wrapped_ndpointer(dtype=numpy.uint8, flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, auto_start, timeout, data_layout,
+            write_array, ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
+        return samps_per_chan_written.value
 
-        return val.value
-
-    @pwr_current_setpoint.setter
-    def pwr_current_setpoint(self, val):
-        cfunc = lib_importer.windll.DAQmxSetPwrCurrentSetpoint
+    def write_to_teds_from_array(
+            self, physical_channel, bit_stream, basic_teds_options):
+        cfunc = lib_importer.windll.DAQmxWriteToTEDSFromArray
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+                        ctypes_byte_str, wrapped_ndpointer(dtype=numpy.uint8,
+                        flags=('C')), ctypes.c_uint, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            physical_channel, bit_stream, len(bit_stream), basic_teds_options)
+        self.check_for_error(error_code)
 
-    @pwr_current_setpoint.deleter
-    def pwr_current_setpoint(self):
-        cfunc = lib_importer.windll.DAQmxResetPwrCurrentSetpoint
+    def write_to_teds_from_file(
+            self, physical_channel, file_path, basic_teds_options):
+        cfunc = lib_importer.windll.DAQmxWriteToTEDSFromFile
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        ctypes_byte_str, ctypes_byte_str, ctypes.c_int]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            physical_channel, file_path, basic_teds_options)
+        self.check_for_error(error_code)
 
-    @property
-    def pwr_idle_output_behavior(self):
-        """
-        :class:`nidaqmx.constants.PowerIdleOutputBehavior`: Specifies
-            whether to disable the output or maintain the existing value
-            after the task is uncommitted.
-        """
-        val = ctypes.c_int()
+    def get_error_string(self, error_code):
+        error_buffer = ctypes.create_string_buffer(2048)
 
-        cfunc = lib_importer.windll.DAQmxGetPwrIdleOutputBehavior
+        cfunc = lib_importer.windll.DAQmxGetErrorString
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                    cfunc.argtypes = [ctypes.c_int, ctypes.c_char_p,
+                                      ctypes.c_uint]
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+        query_error_code = cfunc(error_code, error_buffer, 2048)
+        if query_error_code < 0:
+            _logger.error('Failed to get error string for error code %d. DAQmxGetErrorString returned error code %d.', error_code, query_error_code)
+            return 'Failed to retrieve error description.'
+        return error_buffer.value.decode('utf-8')
 
-        return PowerIdleOutputBehavior(val.value)
+    def get_extended_error_info(self):
+        error_buffer = ctypes.create_string_buffer(2048)
 
-    @pwr_idle_output_behavior.setter
-    def pwr_idle_output_behavior(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetPwrIdleOutputBehavior
+        cfunc = lib_importer.windll.DAQmxGetExtendedErrorInfo
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+                    cfunc.argtypes = [ctypes.c_char_p, ctypes.c_uint]
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+        query_error_code = cfunc(error_buffer, 2048)
+        if query_error_code < 0:
+            _logger.error('Failed to get extended error info. DAQmxGetExtendedErrorInfo returned error code %d.', query_error_code)
+            return 'Failed to retrieve error description.'
+        return error_buffer.value.decode('utf-8')
 
-    @pwr_idle_output_behavior.deleter
-    def pwr_idle_output_behavior(self):
-        cfunc = lib_importer.windll.DAQmxResetPwrIdleOutputBehavior
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+    def read_power_binary_i16(
+            self, task, num_samps_per_chan, timeout, fill_mode,
+            read_voltage_array, read_current_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
-
-    @property
-    def pwr_output_enable(self):
-        """
-        bool: Specifies whether to enable or disable power module
-            output. Can be set while a task is running. Can be read at
-            any time during a task. When a task is running, the output
-            is enabled immediately. Otherwise, the output is not enabled
-            until the task enters the Committed state.
-        """
-        val = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxGetPwrOutputEnable
+        cfunc = lib_importer.windll.DAQmxReadPowerBinaryI16
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_double,
+                        c_bool32,
+                        wrapped_ndpointer(dtype=numpy.int16, flags=('C', 'W')),
+                        wrapped_ndpointer(dtype=numpy.int16, flags=('C', 'W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
                         ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
-
-    @pwr_output_enable.setter
-    def pwr_output_enable(self, val):
-        cfunc = lib_importer.windll.DAQmxSetPwrOutputEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str, c_bool32]
-
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode,
+            read_voltage_array, read_current_array, read_voltage_array.size,
+            ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
 
-    @pwr_output_enable.deleter
-    def pwr_output_enable(self):
-        cfunc = lib_importer.windll.DAQmxResetPwrOutputEnable
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+        return read_voltage_array, read_current_array, samps_per_chan_read.value
 
-    @property
-    def pwr_output_state(self):
-        """
-        :class:`nidaqmx.constants.PowerOutputState`: Indicates power
-            channel operating state. Can be read at any time during a
-            task.
-        """
-        val = ctypes.c_int()
+    def read_power_f64(
+            self, task, num_samps_per_chan, timeout, fill_mode,
+            read_voltage_array, read_current_array):
+        samps_per_chan_read = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetPwrOutputState
+        cfunc = lib_importer.windll.DAQmxReadPowerF64
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_double,
+                        c_bool32,
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C', 'W')),
+                        wrapped_ndpointer(dtype=numpy.float64, flags=('C', 'W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
+                        ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            task, num_samps_per_chan, timeout, fill_mode,
+            read_voltage_array, read_current_array, read_voltage_array.size,
+            ctypes.byref(samps_per_chan_read), None)
+        self.check_for_error(error_code, samps_per_chan_read=samps_per_chan_read.value)
 
-        return PowerOutputState(val.value)
+        return read_voltage_array, read_current_array, samps_per_chan_read.value
 
-    @property
-    def pwr_remote_sense(self):
-        """
-        :class:`nidaqmx.constants.Sense`: Specifies whether to use local
-            or remote sense to sense the output voltage. DAQmx Read
-            (Power) will return remote or local voltage based on the
-            Remote Sense attribute value. Reading this property will
-            return the user-defined value.
-        """
-        val = ctypes.c_int()
+    def read_raw(self, task, num_samps_per_chan, timeout, read_array):
+        samples_read = ctypes.c_int()
+        number_of_bytes_per_sample = ctypes.c_int()
 
-        cfunc = lib_importer.windll.DAQmxGetPwrRemoteSense
+        cfunc = lib_importer.windll.DAQmxReadRaw
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_int)]
+                        lib_importer.task_handle, ctypes.c_int, ctypes.c_double,
+                        wrapped_ndpointer(dtype=read_array.dtype, flags=('C', 'W')),
+                        ctypes.c_uint, ctypes.POINTER(ctypes.c_int),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return Sense(val.value)
+            task, num_samps_per_chan, timeout, read_array,
+            read_array.nbytes, ctypes.byref(samples_read),
+            ctypes.byref(number_of_bytes_per_sample), None)
+        self.check_for_error(error_code, samps_per_chan_read=samples_read.value)
 
-    @pwr_remote_sense.setter
-    def pwr_remote_sense(self, val):
-        val = val.value
-        cfunc = lib_importer.windll.DAQmxSetPwrRemoteSense
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_int]
+        return read_array, samples_read.value, number_of_bytes_per_sample.value
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
+    def write_raw(
+            self, task_handle, num_samps_per_chan, auto_start, timeout, numpy_array):
+        samps_per_chan_written = ctypes.c_int()
 
-    @pwr_remote_sense.deleter
-    def pwr_remote_sense(self):
-        cfunc = lib_importer.windll.DAQmxResetPwrRemoteSense
+        cfunc = lib_importer.windll.DAQmxWriteRaw
         if cfunc.argtypes is None:
             with cfunc.arglock:
                 if cfunc.argtypes is None:
                     cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
+                        lib_importer.task_handle, ctypes.c_int, c_bool32,
+                        ctypes.c_double,
+                        wrapped_ndpointer(dtype=numpy_array.dtype,
+                                        flags=('C')),
+                        ctypes.POINTER(ctypes.c_int), ctypes.POINTER(c_bool32)]
 
         error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+            task_handle, num_samps_per_chan, auto_start, timeout, numpy_array,
+            ctypes.byref(samps_per_chan_written), None)
+        self.check_for_error(error_code, samps_per_chan_written=samps_per_chan_written.value)
 
-    @property
-    def pwr_voltage_dev_scaling_coeff(self):
-        """
-        List[float]: Indicates the coefficients of the polynomial
-            equation that NI-DAQmx uses to scale values from the native
-            format of the device to volts. Can be read at any time
-            during a task.
-        """
-        cfunc = lib_importer.windll.DAQmxGetPwrVoltageDevScalingCoeff
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        wrapped_ndpointer(dtype=numpy.float64,
-                        flags=('C','W')), ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = numpy.zeros(temp_size, dtype=numpy.float64)
-
-            size_or_code = cfunc(
-                self._handle, self._name, val, temp_size)
-
-            if is_array_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
+        return samps_per_chan_written.value
 
-        return val.tolist()
+    def hash_task_handle(self, task_handle):
+        return hash(task_handle.value)
 
-    @property
-    def pwr_voltage_setpoint(self):
-        """
-        float: Specifies the constant output voltage, in volts. Can be
-            set while a task is running. Can be read at any time during
-            a task.
-        """
-        val = ctypes.c_double()
+    def check_for_error(self, error_code, samps_per_chan_written=None, samps_per_chan_read=None):
+        if not error_code:
+            return
 
-        cfunc = lib_importer.windll.DAQmxGetPwrVoltageSetpoint
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.POINTER(ctypes.c_double)]
+        if error_code < 0:
+            extended_error_info = self.get_extended_error_info()
 
-        error_code = cfunc(
-            self._handle, self._name, ctypes.byref(val))
-        check_for_error(error_code)
+            if samps_per_chan_read is not None:
+                raise DaqReadError(extended_error_info, error_code, samps_per_chan_read)
+            elif samps_per_chan_written is not None:
+                raise DaqWriteError(extended_error_info, error_code, samps_per_chan_written)
+            else:
+                raise DaqError(extended_error_info, error_code)
 
-        return val.value
+        elif error_code > 0:
+            error_string = self.get_error_string(error_code)
 
-    @pwr_voltage_setpoint.setter
-    def pwr_voltage_setpoint(self, val):
-        cfunc = lib_importer.windll.DAQmxSetPwrVoltageSetpoint
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes.c_double]
+            warnings.warn(DaqWarning(error_string, error_code))
 
-        error_code = cfunc(
-            self._handle, self._name, val)
-        check_for_error(error_code)
-
-    @pwr_voltage_setpoint.deleter
-    def pwr_voltage_setpoint(self):
-        cfunc = lib_importer.windll.DAQmxResetPwrVoltageSetpoint
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
 
-        error_code = cfunc(
-            self._handle, self._name)
-        check_for_error(error_code)
+def is_string_buffer_too_small(error_code):
+    return (
+        error_code == DAQmxErrors.BUFFER_TOO_SMALL_FOR_STRING or
+        error_code == DAQmxWarnings.CAPI_STRING_TRUNCATED_TO_FIT_BUFFER)
 
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_rtd_r0 instead.")
-    def ai_rtd_r_0(self):
-        return self.ai_rtd_r0
-
-    @ai_rtd_r_0.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_rtd_r0 instead.")
-    def ai_rtd_r_0(self, val):
-        self.ai_rtd_r0 = val
-
-    @ai_rtd_r_0.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_rtd_r0 instead.")
-    def ai_rtd_r_0(self):
-        del self.ai_rtd_r0
-
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_sound_pressure_db_ref instead.")
-    def ai_sound_pressured_b_ref(self):
-        return self.ai_sound_pressure_db_ref
-
-    @ai_sound_pressured_b_ref.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_sound_pressure_db_ref instead.")
-    def ai_sound_pressured_b_ref(self, val):
-        self.ai_sound_pressure_db_ref = val
-
-    @ai_sound_pressured_b_ref.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_sound_pressure_db_ref instead.")
-    def ai_sound_pressured_b_ref(self):
-        del self.ai_sound_pressure_db_ref
-
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_thrmstr_r1 instead.")
-    def ai_thrmstr_r_1(self):
-        return self.ai_thrmstr_r1
-
-    @ai_thrmstr_r_1.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_thrmstr_r1 instead.")
-    def ai_thrmstr_r_1(self, val):
-        self.ai_thrmstr_r1 = val
-
-    @ai_thrmstr_r_1.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_thrmstr_r1 instead.")
-    def ai_thrmstr_r_1(self):
-        del self.ai_thrmstr_r1
-
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_accel_db_ref instead.")
-    def ai_acceld_b_ref(self):
-        return self.ai_accel_db_ref
-
-    @ai_acceld_b_ref.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_accel_db_ref instead.")
-    def ai_acceld_b_ref(self, val):
-        self.ai_accel_db_ref = val
-
-    @ai_acceld_b_ref.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_accel_db_ref instead.")
-    def ai_acceld_b_ref(self):
-        del self.ai_accel_db_ref
-
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_voltage_db_ref instead.")
-    def ai_voltaged_b_ref(self):
-        return self.ai_voltage_db_ref
-
-    @ai_voltaged_b_ref.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_voltage_db_ref instead.")
-    def ai_voltaged_b_ref(self, val):
-        self.ai_voltage_db_ref = val
-
-    @ai_voltaged_b_ref.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_voltage_db_ref instead.")
-    def ai_voltaged_b_ref(self):
-        del self.ai_voltage_db_ref
-
-    @property
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_velocity_iepe_sensor_db_ref instead.")
-    def ai_velocity_iepe_sensord_b_ref(self):
-        return self.ai_velocity_iepe_sensor_db_ref
-
-    @ai_velocity_iepe_sensord_b_ref.setter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_velocity_iepe_sensor_db_ref instead.")
-    def ai_velocity_iepe_sensord_b_ref(self, val):
-        self.ai_velocity_iepe_sensor_db_ref = val
-
-    @ai_velocity_iepe_sensord_b_ref.deleter
-    @deprecation.deprecated(deprecated_in="0.7.0", details="Use ai_velocity_iepe_sensor_db_ref instead.")
-    def ai_velocity_iepe_sensord_b_ref(self):
-        del self.ai_velocity_iepe_sensor_db_ref
 
+def is_array_buffer_too_small(error_code):
+    return error_code == DAQmxErrors.WRITE_BUFFER_TOO_SMALL
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/ci_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/ci_channel_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
-import numpy
-
-from nidaqmx._lib import lib_importer, ctypes_byte_str, c_bool32
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.ci_channel import CIChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     AngleUnits, AngularVelocityUnits, CountDirection, CounterFrequencyMethod,
     Edge, EncoderType, EncoderZIndexPhase, FrequencyUnits, GpsSignalType,
     LengthUnits, TimeUnits, VelocityUnits)
 
 
 class CIChannelCollection(ChannelCollection):
     """
     Contains the collection of counter input channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.ci_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, counter, name_to_assign_to_channel=''):
         """
         Creates and returns a CIChannel object.
 
         Args:
             counter (str): Specifies the names of the counters to use to 
@@ -42,15 +40,15 @@
                 name = '{}0:{}'.format(
                     name_to_assign_to_channel, num_counters-1)
             else:
                 name = name_to_assign_to_channel
         else:
             name = counter
 
-        return CIChannel(self._handle, name)
+        return CIChannel(self._handle, name, self._interpreter)
 
     def add_ci_ang_encoder_chan(
             self, counter, name_to_assign_to_channel="",
             decoding_type=EncoderType.X_4, zidx_enable=False, zidx_val=0,
             zidx_phase=EncoderZIndexPhase.AHIGH_BHIGH,
             units=AngleUnits.DEGREES, pulses_per_rev=24, initial_angle=0.0,
             custom_scale_name=""):
@@ -108,29 +106,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIAngEncoderChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, c_bool32,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_uint, ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_ang_encoder_chan(
             self._handle, counter, name_to_assign_to_channel,
             decoding_type.value, zidx_enable, zidx_val, zidx_phase.value,
             units.value, pulses_per_rev, initial_angle, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_ang_velocity_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.0,
             max_val=1.0, decoding_type=EncoderType.X_4,
             units=AngularVelocityUnits.RPM, pulses_per_rev=24,
@@ -178,29 +166,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIAngVelocityChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_uint,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_ang_velocity_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, decoding_type.value, units.value, pulses_per_rev,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_count_edges_chan(
             self, counter, name_to_assign_to_channel="", edge=Edge.RISING,
             initial_count=0, count_direction=CountDirection.COUNT_UP):
         """
@@ -232,27 +210,18 @@
                 Specifies whether to increment or decrement the counter
                 on each edge.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCICountEdgesChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_uint,
-                        ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_count_edges_chan(
             self._handle, counter, name_to_assign_to_channel, edge.value,
             initial_count, count_direction.value)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_duty_cycle_chan(
             self, counter, name_to_assign_to_channel="", min_freq=2.0,
             max_freq=10000.0, edge=Edge.RISING, custom_scale_name=""):
         """
@@ -288,27 +257,18 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIDutyCycleChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_duty_cycle_chan(
             self._handle, counter, name_to_assign_to_channel, min_freq,
             max_freq, edge.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_freq_chan(
             self, counter, name_to_assign_to_channel="", min_val=2.0,
             max_val=100.0, units=FrequencyUnits.HZ, edge=Edge.RISING,
             meas_method=CounterFrequencyMethod.LOW_FREQUENCY_1_COUNTER,
@@ -362,29 +322,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIFreqChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_uint, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_freq_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value, edge.value, meas_method.value, meas_time,
             divisor, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_gps_timestamp_chan(
             self, counter, name_to_assign_to_channel="",
             units=TimeUnits.SECONDS, sync_method=GpsSignalType.IRIGB,
             custom_scale_name=""):
@@ -420,27 +370,18 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIGPSTimestampChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_cigps_timestamp_chan(
             self._handle, counter, name_to_assign_to_channel, units.value,
             sync_method.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_lin_encoder_chan(
             self, counter, name_to_assign_to_channel="",
             decoding_type=EncoderType.X_4, zidx_enable=False, zidx_val=0,
             zidx_phase=EncoderZIndexPhase.AHIGH_BHIGH,
@@ -500,29 +441,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCILinEncoderChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, c_bool32,
-                        ctypes.c_double, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_lin_encoder_chan(
             self._handle, counter, name_to_assign_to_channel,
             decoding_type.value, zidx_enable, zidx_val, zidx_phase.value,
             units.value, dist_per_pulse, initial_pos, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_lin_velocity_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.0,
             max_val=1.0, decoding_type=EncoderType.X_4,
             units=VelocityUnits.METERS_PER_SECOND, dist_per_pulse=0.001,
@@ -570,29 +501,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCILinVelocityChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_double,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_lin_velocity_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, decoding_type.value, units.value, dist_per_pulse,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_period_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.000001,
             max_val=0.1, units=TimeUnits.SECONDS, edge=Edge.RISING,
             meas_method=CounterFrequencyMethod.LOW_FREQUENCY_1_COUNTER,
@@ -645,29 +566,19 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIPeriodChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_uint, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_period_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value, edge.value, meas_method.value, meas_time,
             divisor, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_pulse_chan_freq(
             self, counter, name_to_assign_to_channel="", min_val=1000,
             max_val=1000000, units=FrequencyUnits.HZ):
         """
@@ -699,27 +610,18 @@
                 Specifies the units to use to return pulse
                 specifications in terms of frequency.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_pulse_chan_freq(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_pulse_chan_ticks(
             self, counter, name_to_assign_to_channel="",
             source_terminal="OnboardClock", min_val=1000, max_val=1000000):
         """
@@ -756,27 +658,18 @@
             max_val (Optional[float]): Specifies in **units** the
                 maximum value you expect to measure.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanTicks
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes_byte_str, ctypes.c_double,
-                        ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_pulse_chan_ticks(
             self._handle, counter, name_to_assign_to_channel, source_terminal,
             min_val, max_val)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_pulse_chan_time(
             self, counter, name_to_assign_to_channel="", min_val=0.000001,
             max_val=0.001, units=TimeUnits.SECONDS):
         """
@@ -808,27 +701,18 @@
                 units to use to return pulse specifications in terms of
                 high time and low time.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIPulseChanTime
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_pulse_chan_time(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_pulse_width_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.000001,
             max_val=0.1, units=TimeUnits.SECONDS, starting_edge=Edge.RISING,
             custom_scale_name=""):
@@ -867,27 +751,18 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCIPulseWidthChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_pulse_width_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value, starting_edge.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_semi_period_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.000001,
             max_val=0.1, units=TimeUnits.SECONDS, custom_scale_name=""):
         """
@@ -922,27 +797,18 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCISemiPeriodChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_semi_period_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value, custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_ci_two_edge_sep_chan(
             self, counter, name_to_assign_to_channel="", min_val=0.000001,
             max_val=1.0, units=TimeUnits.SECONDS, first_edge=Edge.RISING,
             second_edge=Edge.FALLING, custom_scale_name=""):
@@ -986,25 +852,15 @@
                 to this input and set **units** to
                 **FROM_CUSTOM_SCALE**.
         Returns:
             nidaqmx._task_modules.channels.ci_channel.CIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCITwoEdgeSepChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_double, ctypes.c_double,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int,
-                        ctypes_byte_str]
 
-        error_code = cfunc(
+        self._interpreter.create_ci_two_edge_sep_chan(
             self._handle, counter, name_to_assign_to_channel, min_val,
             max_val, units.value, first_edge.value, second_edge.value,
             custom_scale_name)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/co_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/co_channel_collection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
-import numpy
-
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.co_channel import COChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     FrequencyUnits, Level, TimeUnits)
 
 
 class COChannelCollection(ChannelCollection):
     """
     Contains the collection of counter output channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.co_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, counter, name_to_assign_to_channel=''):
         """
         Creates and returns a COChannel object.
 
         Args:
             counter (str): Specifies the names of the counters to use to 
@@ -40,15 +38,15 @@
                 name = '{}0:{}'.format(
                     name_to_assign_to_channel, num_counters-1)
             else:
                 name = name_to_assign_to_channel
         else:
             name = counter
 
-        return COChannel(self._handle, name)
+        return COChannel(self._handle, name, self._interpreter)
 
     def add_co_pulse_chan_freq(
             self, counter, name_to_assign_to_channel="",
             units=FrequencyUnits.HZ, idle_state=Level.LOW, initial_delay=0.0,
             freq=1.0, duty_cycle=0.5):
         """
         Creates channel(s) to generate digital pulses that **freq** and
@@ -79,27 +77,18 @@
                 combined with frequency to determine pulse width and the
                 interval between pulses.
         Returns:
             nidaqmx._task_modules.channels.co_channel.COChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanFreq
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_co_pulse_chan_freq(
             self._handle, counter, name_to_assign_to_channel, units.value,
             idle_state.value, initial_delay, freq, duty_cycle)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_co_pulse_chan_ticks(
             self, counter, source_terminal, name_to_assign_to_channel="",
             idle_state=Level.LOW, initial_delay=0, low_ticks=100,
             high_ticks=100):
@@ -134,27 +123,18 @@
             high_ticks (Optional[int]): Is the number of ticks the pulse
                 is high.
         Returns:
             nidaqmx._task_modules.channels.co_channel.COChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanTicks
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes_byte_str, ctypes.c_int,
-                        ctypes.c_int, ctypes.c_int, ctypes.c_int]
 
-        error_code = cfunc(
-            self._handle, counter, name_to_assign_to_channel, source_terminal,
+        self._interpreter.create_co_pulse_chan_ticks(
+            self._handle, counter, source_terminal, name_to_assign_to_channel,
             idle_state.value, initial_delay, low_ticks, high_ticks)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
 
     def add_co_pulse_chan_time(
             self, counter, name_to_assign_to_channel="",
             units=TimeUnits.SECONDS, idle_state=Level.LOW, initial_delay=0.0,
             low_time=0.01, high_time=0.01):
@@ -186,23 +166,14 @@
             high_time (Optional[float]): Is the amount of time the pulse
                 is high.
         Returns:
             nidaqmx._task_modules.channels.co_channel.COChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateCOPulseChanTime
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int, ctypes.c_int,
-                        ctypes.c_double, ctypes.c_double, ctypes.c_double]
 
-        error_code = cfunc(
+        self._interpreter.create_co_pulse_chan_time(
             self._handle, counter, name_to_assign_to_channel, units.value,
             idle_state.value, initial_delay, low_time, high_time)
-        check_for_error(error_code)
 
         return self._create_chan(counter, name_to_assign_to_channel)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/di_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/di_channel_collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
-import numpy
-
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.di_channel import DIChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     LineGrouping)
 
 
 class DIChannelCollection(ChannelCollection):
     """
     Contains the collection of digital input channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.di_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, lines, line_grouping, name_to_assign_to_lines=''):
         """
         Creates and returns a DIChannel object.
 
         Args:
             lines (str): Specifies the names of the lines to use to 
@@ -50,15 +48,15 @@
                     name = '{}0:{}'.format(
                         name_to_assign_to_lines, num_lines-1)
                 else:
                     name = name_to_assign_to_lines
             else:
                 name = lines
 
-        return DIChannel(self._handle, name)
+        return DIChannel(self._handle, name, self._interpreter)
 
     def add_di_chan(
             self, lines, name_to_assign_to_lines="",
             line_grouping=LineGrouping.CHAN_FOR_ALL_LINES):
         """
         Creates channel(s) to measure digital signals. You can group
         digital lines into one digital channel or separate them into
@@ -83,21 +81,13 @@
                 ports with the **lines** input, you must set this input
                 to **one channel for all lines**.
         Returns:
             nidaqmx._task_modules.channels.di_channel.DIChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateDIChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_di_chan(
             self._handle, lines, name_to_assign_to_lines, line_grouping.value)
-        check_for_error(error_code)
 
         return self._create_chan(lines, line_grouping, name_to_assign_to_lines)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/_task_modules/do_channel_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/_task_modules/do_channel_collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # Do not edit this file; it was automatically generated.
 
-import ctypes
-import numpy
-
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import check_for_error
 from nidaqmx._task_modules.channels.do_channel import DOChannel
 from nidaqmx._task_modules.channel_collection import ChannelCollection
 from nidaqmx.utils import unflatten_channel_string
 from nidaqmx.constants import (
     LineGrouping)
 
 
 class DOChannelCollection(ChannelCollection):
     """
     Contains the collection of digital output channels for a DAQmx Task.
     """
-    def __init__(self, task_handle):
-        super().__init__(task_handle)
+    def __init__(self, task_handle, interpreter):
+        """
+        Do not construct this object directly; instead, construct a nidaqmx.Task and use the task.do_channels property.
+        """
+        super().__init__(task_handle, interpreter)
 
     def _create_chan(self, lines, line_grouping, name_to_assign_to_lines=''):
         """
         Creates and returns a DOChannel object.
 
         Args:
             lines (str): Specifies the names of the lines to use to 
@@ -50,15 +48,15 @@
                     name = '{}0:{}'.format(
                         name_to_assign_to_lines, num_lines-1)
                 else:
                     name = name_to_assign_to_lines
             else:
                 name = lines
 
-        return DOChannel(self._handle, name)
+        return DOChannel(self._handle, name, self._interpreter)
 
     def add_do_chan(
             self, lines, name_to_assign_to_lines="",
             line_grouping=LineGrouping.CHAN_FOR_ALL_LINES):
         """
         Creates channel(s) to generate digital signals. You can group
         digital lines into one digital channel or separate them into
@@ -83,21 +81,13 @@
                 ports with the **lines** input, you must set this input
                 to **one channel for all lines**.
         Returns:
             nidaqmx._task_modules.channels.do_channel.DOChannel:
             
             Indicates the newly created channel object.
         """
-        cfunc = lib_importer.windll.DAQmxCreateDOChan
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_int]
 
-        error_code = cfunc(
+        self._interpreter.create_do_chan(
             self._handle, lines, name_to_assign_to_lines, line_grouping.value)
-        check_for_error(error_code)
 
         return self._create_chan(lines, line_grouping, name_to_assign_to_lines)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/constants.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/constants.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/error_codes.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/error_codes.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/errors.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import ctypes
 import warnings
+import deprecation
 
 from nidaqmx.error_codes import DAQmxErrors, DAQmxWarnings
 
 __all__ = ['DaqError', 'DaqReadError', 'DaqWriteError', 'DaqWarning', 'DaqResourceWarning']
 
 
 class Error(Exception):
@@ -154,54 +154,37 @@
 
 
 DaqResourceWarning = ResourceWarning
 
 warnings.filterwarnings("always", category=DaqWarning)
 warnings.filterwarnings("always", category=DaqResourceWarning)
 
-
+@deprecation.deprecated(deprecated_in="0.8.0", details="This function will be removed in a future update.")
 def check_for_error(error_code, samps_per_chan_written=None, samps_per_chan_read=None):
-    if not error_code:
-        return
+    from nidaqmx._library_interpreter import LibraryInterpreter
+    return LibraryInterpreter().check_for_error(error_code, samps_per_chan_written, samps_per_chan_read)
 
-    from nidaqmx._lib import lib_importer
 
-    if error_code < 0:
-        error_buffer = ctypes.create_string_buffer(2048)
+@deprecation.deprecated(deprecated_in="0.8.0", details="This function will be removed in a future update.")
+def is_string_buffer_too_small(error_code):
+    import nidaqmx._library_interpreter
+    return nidaqmx._library_interpreter.is_string_buffer_too_small(error_code)
 
-        cfunc = lib_importer.windll.DAQmxGetExtendedErrorInfo
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [ctypes.c_char_p, ctypes.c_uint]
-        cfunc(error_buffer, 2048)
-
-        if samps_per_chan_read is not None:
-            raise DaqReadError(error_buffer.value.decode("utf-8"), error_code, samps_per_chan_read)
-        elif samps_per_chan_written is not None:
-            raise DaqWriteError(error_buffer.value.decode("utf-8"), error_code, samps_per_chan_written)
-        else:
-            raise DaqError(error_buffer.value.decode("utf-8"), error_code)
-
-    elif error_code > 0:
-        error_buffer = ctypes.create_string_buffer(2048)
-
-        cfunc = lib_importer.windll.DAQmxGetErrorString
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [ctypes.c_int, ctypes.c_char_p,
-                                      ctypes.c_uint]
-        cfunc(error_code, error_buffer, 2048)
 
-        warnings.warn(DaqWarning(
-            error_buffer.value.decode("utf-8"), error_code))
+@deprecation.deprecated(deprecated_in="0.8.0", details="This function will be removed in a future update.")
+def is_array_buffer_too_small(error_code):
+    import nidaqmx._library_interpreter
+    return nidaqmx._library_interpreter.is_array_buffer_too_small(error_code)
 
 
-def is_string_buffer_too_small(error_code):
-    return (
-        error_code == DAQmxErrors.BUFFER_TOO_SMALL_FOR_STRING or
-        error_code == DAQmxWarnings.CAPI_STRING_TRUNCATED_TO_FIT_BUFFER)
+class RpcError(Error):
+    '''An error specific to sessions to the NI gRPC Device Server'''
 
-
-def is_array_buffer_too_small(error_code):
-    return error_code == DAQmxErrors.WRITE_BUFFER_TOO_SMALL
+    def __init__(self, rpc_code, description):
+        self.rpc_code = rpc_code
+        self.description = description
+        try:
+            import grpc
+            rpc_error = str(grpc.StatusCode(self.rpc_code))
+        except Exception:
+            rpc_error = str(self.rpc_code)
+        super().__init__(rpc_error + ": " + self.description)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/stream_readers.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_readers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,13 @@
 import numpy
 from nidaqmx import DaqError
 
-from nidaqmx.constants import READ_ALL_AVAILABLE
-from nidaqmx._task_modules.read_functions import (
-    _read_analog_f_64, _read_analog_scalar_f_64,
-    _read_power_f_64, _read_power_scalar_f_64, _read_power_i_16,
-    _read_binary_i_16, _read_binary_i_32,
-    _read_binary_u_16, _read_binary_u_32,
-    _read_digital_lines, _read_digital_u_8, _read_digital_u_16,
-    _read_digital_scalar_u_32, _read_digital_u_32, _read_counter_scalar_f_64,
-    _read_counter_scalar_u_32, _read_counter_f_64_ex, _read_counter_u_32_ex,
-    _read_ctr_freq_scalar, _read_ctr_ticks_scalar, _read_ctr_time_scalar,
-    _read_ctr_freq, _read_ctr_ticks, _read_ctr_time)
+from nidaqmx.constants import FillMode, READ_ALL_AVAILABLE
 from nidaqmx.error_codes import DAQmxErrors
-from nidaqmx.types import PowerMeasurement
+from nidaqmx.types import PowerMeasurement, CtrFreq, CtrTick, CtrTime
 
 __all__ = ['AnalogSingleChannelReader', 'AnalogMultiChannelReader',
            'AnalogUnscaledReader', 'CounterReader',
            'DigitalSingleChannelReader', 'DigitalMultiChannelReader',
            'PowerSingleChannelReader', 'PowerMultiChannelReader', 'PowerBinaryReader']
 
 
@@ -31,14 +21,15 @@
         Args:
             task_in_stream: Specifies the input stream associated with
                 an NI-DAQmx task from which to read samples.
         """
         self._in_stream = task_in_stream
         self._task = task_in_stream._task
         self._handle = task_in_stream._task._handle
+        self._interpreter = task_in_stream._task._interpreter
 
         self._verify_array_shape = True
 
     @property
     def verify_array_shape(self):
         """
         bool: Indicates whether the size and shape of the user-defined
@@ -212,17 +203,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_analog_f_64(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_analog_f64(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_one_sample(self, timeout=10):
         """
         Reads a single floating-point sample from a single analog input
         channel in a task.
 
         Args:
@@ -236,15 +229,15 @@
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             float:
 
             Indicates a single floating-point sample from the task.
         """
-        return _read_analog_scalar_f_64(self._handle, timeout)
+        return self._interpreter.read_analog_scalar_f64(self._handle, timeout)
 
 
 class AnalogMultiChannelReader(ChannelReaderBase):
     """
     Reads samples from one or more analog input channels in an NI-DAQmx
     task.
     """
@@ -324,17 +317,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_analog_f_64(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_analog_f64(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_one_sample(self, data, timeout=10):
         """
         Reads a single floating-point sample from one or more analog
         input channels in a task.
 
         This read method accepts a preallocated NumPy array to hold the
@@ -362,15 +357,15 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array(data, 1, True, False)
 
-        _read_analog_f_64(self._handle, data, 1, timeout)
+        self._interpreter.read_analog_f64(self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
 
 class AnalogUnscaledReader(ChannelReaderBase):
     """
     Reads unscaled samples from one or more analog input channels in an
     NI-DAQmx task.
     """
@@ -450,17 +445,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_binary_i_16(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_binary_i16(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_int32(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more unscaled 32-bit integer samples from one or
         more analog input channels in a task.
@@ -533,17 +530,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_binary_i_32(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_binary_i32(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_uint16(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more unscaled 16-bit unsigned integer samples from
         one or more analog input channels in a task.
@@ -616,17 +615,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_binary_u_16(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_binary_u16(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_uint32(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more unscaled unsigned 32-bit integer samples from
         one or more analog input channels in a task.
@@ -699,17 +700,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_binary_u_32(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read =  self._interpreter.read_binary_u32(
+            self._handle, number_of_samples_per_channel,
+            timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
 
 class PowerSingleChannelReader(ChannelReaderBase):
     """
     Reads samples from an analog input power channel in an NI-DAQmx task.
     """
 
@@ -784,17 +787,19 @@
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(voltage_data, number_of_samples_per_channel, False, True)
         self._verify_array(current_data, number_of_samples_per_channel, False, True)
 
-        return _read_power_f_64(
-            self._handle, voltage_data, current_data, number_of_samples_per_channel,
-            timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_power_f64(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, voltage_data, current_data)
+        
+        return samps_per_chan_read
 
     def read_one_sample(self, timeout=10):
         """
         Reads a single floating-point power sample from a single analog input
         power channel in a task.
 
         Args:
@@ -808,15 +813,15 @@
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             float:
 
             Indicates a single floating-point power sample from the task.
         """
-        voltage, current = _read_power_scalar_f_64(self._handle, timeout)
+        voltage, current = self._interpreter.read_power_scalar_f64(self._handle, timeout)
         return PowerMeasurement(voltage=voltage, current=current)
 
 
 class PowerMultiChannelReader(ChannelReaderBase):
     """
     Reads samples from one or more analog input power channels in an NI-DAQmx
     task.
@@ -919,17 +924,19 @@
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(voltage_data, number_of_samples_per_channel, True, True)
         self._verify_array(current_data, number_of_samples_per_channel, True, True)
 
-        return _read_power_f_64(
-            self._handle, voltage_data, current_data, number_of_samples_per_channel,
-            timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_power_f64(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, voltage_data, current_data)
+        
+        return samps_per_chan_read
 
     def read_one_sample(self, voltage_data, current_data, timeout=10):
         """
         Reads a single floating-point power sample from one or more analog
         input channels in a task.
 
         This read method accepts a preallocated NumPy array to hold the
@@ -966,16 +973,17 @@
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array(voltage_data, 1, True, False)
         self._verify_array(current_data, 1, True, False)
 
-        _read_power_f_64(
-            self._handle, voltage_data, current_data, 1, timeout)
+        self._interpreter.read_power_f64(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, 
+            voltage_data, current_data)
 
 
 class PowerBinaryReader(ChannelReaderBase):
     """
     Reads binary samples from one or more analog input power channels in an
     NI-DAQmx task.
     """
@@ -1071,17 +1079,19 @@
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(voltage_data, number_of_samples_per_channel, True, True)
         self._verify_array(current_data, number_of_samples_per_channel, True, True)
 
-        return _read_power_i_16(
-            self._handle, voltage_data, current_data, number_of_samples_per_channel,
-            timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_power_binary_i16(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, voltage_data, current_data)
+        
+        return samps_per_chan_read
 
 
 class CounterReader(ChannelReaderBase):
     """
     Reads samples from a counter input channel in an NI-DAQmx task.
     """
 
@@ -1147,17 +1157,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_counter_f_64_ex(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_counter_f64_ex(
+            self._handle,number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_many_sample_pulse_frequency(
             self, frequencies, duty_cycles,
             number_of_samples_per_channel=READ_ALL_AVAILABLE, timeout=10.0):
         """
         Reads one or more pulse samples in terms of frequency from a
         single counter input channel in a task.
@@ -1228,17 +1240,19 @@
                 number_of_samples_per_channel))
 
         self._verify_array(
             frequencies, number_of_samples_per_channel, False, True)
         self._verify_array(
             duty_cycles, number_of_samples_per_channel, False, True)
 
-        return _read_ctr_freq(
-            self._handle, frequencies, duty_cycles,
-            number_of_samples_per_channel, timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_ctr_freq(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, frequencies, duty_cycles)
+        
+        return samps_per_chan_read
 
     def read_many_sample_pulse_ticks(
             self, high_ticks, low_ticks,
             number_of_samples_per_channel=READ_ALL_AVAILABLE, timeout=10.0):
         """
         Reads one or more pulse samples in terms of ticks from a single
         counter input channel in a task.
@@ -1309,17 +1323,19 @@
                 number_of_samples_per_channel))
 
         self._verify_array(
             high_ticks, number_of_samples_per_channel, False, True)
         self._verify_array(
             low_ticks, number_of_samples_per_channel, False, True)
 
-        return _read_ctr_ticks(
-            self._handle, high_ticks, low_ticks,
-            number_of_samples_per_channel, timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_ctr_ticks(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, high_ticks, low_ticks)
+        
+        return samps_per_chan_read
 
     def read_many_sample_pulse_time(
             self, high_times, low_times,
             number_of_samples_per_channel=READ_ALL_AVAILABLE, timeout=10.0):
         """
         Reads one or more pulse samples in terms of time from a single
         counter input channel in a task.
@@ -1390,17 +1406,19 @@
                 number_of_samples_per_channel))
 
         self._verify_array(
             high_times, number_of_samples_per_channel, False, True)
         self._verify_array(
             low_times, number_of_samples_per_channel, False, True)
 
-        return _read_ctr_time(
-            self._handle, high_times, low_times,
-            number_of_samples_per_channel, timeout)
+        _, _, samps_per_chan_read = self._interpreter.read_ctr_time(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, high_times, low_times)
+        
+        return samps_per_chan_read
 
     def read_many_sample_uint32(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more 32-bit unsigned integer samples from a single
         counter input channel in a task.
@@ -1460,17 +1478,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_counter_u_32_ex(
-            self._handle, data, number_of_samples_per_channel,
-            timeout)
+        _, samps_per_chan_read = self._interpreter.read_counter_u32_ex(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_one_sample_double(self, timeout=10):
         """
         Reads a single floating-point sample from a single counter input
         channel in a task.
 
         Args:
@@ -1483,15 +1503,15 @@
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             float: Indicates a single floating-point sample from the
                 task.
         """
-        return _read_counter_scalar_f_64(self._handle, timeout)
+        return self._interpreter.read_counter_scalar_f64(self._handle, timeout)
 
     def read_one_sample_pulse_frequency(self, timeout=10):
         """
         Reads a pulse sample in terms of frequency from a single counter
         input channel in a task.
 
         Args:
@@ -1505,15 +1525,17 @@
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             nidaqmx.types.CtrFreq:
 
             Indicates a pulse sample in terms of frequency from the task.
         """
-        return _read_ctr_freq_scalar(self._handle, timeout)
+        freq, duty_cycle = self._interpreter.read_ctr_freq_scalar(self._handle, timeout)
+
+        return CtrFreq(freq, duty_cycle)
 
     def read_one_sample_pulse_ticks(self, timeout=10):
         """
         Reads a pulse sample in terms of ticks from a single counter
         input channel in a task.
 
         Args:
@@ -1527,15 +1549,17 @@
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             nidaqmx.types.CtrTick:
 
             Indicates a pulse sample in terms of ticks from the task.
         """
-        return _read_ctr_ticks_scalar(self._handle, timeout)
+        high_ticks, low_ticks = self._interpreter.read_ctr_ticks_scalar(self._handle, timeout)
+
+        return CtrTick(high_ticks, low_ticks)
 
     def read_one_sample_pulse_time(self, timeout=10):
         """
         Reads a pulse sample in terms of time from a single counter
         input channel in a task.
 
         Args:
@@ -1549,15 +1573,17 @@
                 once to read the requested samples and returns an error
                 if it is unable to.
         Returns:
             nidaqmx.types.CtrTime:
 
             Indicates a pulse sample in terms of time from the task.
         """
-        return _read_ctr_time_scalar(self._handle, timeout)
+        high_time, low_time = self._interpreter.read_ctr_time_scalar(self._handle, timeout)
+
+        return CtrTime(high_time, low_time)
 
     def read_one_sample_uint32(self, timeout=10):
         """
         Reads a single 32-bit unsigned integer sample from a single
         counter input channel in a task.
 
         Args:
@@ -1572,15 +1598,15 @@
                 if it is unable to.
         Returns:
             int:
 
             Indicates a single 32-bit unsigned integer sample from the
             task.
         """
-        return _read_counter_scalar_u_32(self._handle, timeout)
+        return self._interpreter.read_counter_scalar_u32(self._handle, timeout)
 
 
 class DigitalSingleChannelReader(ChannelReaderBase):
     """
     Reads samples from a digital input channel in an NI-DAQmx task.
     """
 
@@ -1648,16 +1674,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_digital_u_8(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u8(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_many_sample_port_uint16(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more 16-bit unsigned integer samples from a single
         digital input channel in a task.
@@ -1719,16 +1748,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_digital_u_16(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u16(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_many_sample_port_uint32(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more 32-bit unsigned integer samples from a single
         digital input channel in a task.
@@ -1790,16 +1822,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, False, True)
 
-        return _read_digital_u_32(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u32(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_one_sample_multi_line(self, data, timeout=10):
         """
         Reads a single boolean sample from a single digital input
         channel in a task. The channel can contain multiple digital
         lines.
 
@@ -1827,15 +1862,16 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array_digital_lines(data, False, True)
 
-        _read_digital_lines(self._handle, data, 1, timeout)
+        _, samps_per_chan_read, num_bytes_per_samp = self._interpreter.read_digital_lines(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)    
 
     def read_one_sample_one_line(self, timeout=10):
         """
         Reads a single boolean sample from a single digital input
         channel in a task. The channel can contain only one digital
         line.
 
@@ -1851,15 +1887,16 @@
                 if it is unable to.
         Returns:
             bool:
 
             Indicates a single boolean sample from the task.
         """
         data = numpy.zeros(1, dtype=bool)
-        _read_digital_lines(self._handle, data, 1, timeout)
+        _, samps_per_chan_read, num_bytes_per_samp= self._interpreter.read_digital_lines(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
         return bool(data[0])
 
     def read_one_sample_port_byte(self, timeout=10):
         """
         Reads a single 8-bit unsigned integer sample from a single
         digital input channel in a task.
@@ -1879,15 +1916,16 @@
         Returns:
             int:
 
             Indicates a single 8-bit unsigned integer sample from the
             task.
         """
         data = numpy.zeros(1, dtype=numpy.uint8)
-        _read_digital_u_8(self._handle, data, 1, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u8(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
         return int(data[0])
 
     def read_one_sample_port_uint16(self, timeout=10):
         """
         Reads a single 16-bit unsigned integer sample from a single
         digital input channel in a task.
@@ -1907,15 +1945,16 @@
         Returns:
             int:
 
             Indicates a single 16-bit unsigned integer sample from the
             task.
         """
         data = numpy.zeros(1, dtype=numpy.uint16)
-        _read_digital_u_16(self._handle, data, 1, timeout)
+        _, samps_per_read_chan = self._interpreter.read_digital_u16(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
         return int(data[0])
 
     def read_one_sample_port_uint32(self, timeout=10):
         """
         Reads a single 32-bit unsigned integer sample from a single
         digital input channel in a task.
@@ -1934,15 +1973,15 @@
                 if it is unable to.
         Returns:
             int:
 
             Indicates a single 32-bit unsigned integer sample from the
             task.
         """
-        return _read_digital_scalar_u_32(self._handle, timeout)
+        return self._interpreter.read_digital_scalar_u32(self._handle, timeout)
 
 
 class DigitalMultiChannelReader(ChannelReaderBase):
     """
     Reads samples from one or more digital input channels in an NI-DAQmx
     task.
     """
@@ -2024,16 +2063,19 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_digital_u_8(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u8(
+            self._handle, number_of_samples_per_channel, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_many_sample_port_uint16(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more 16-bit unsigned integer samples from one or
         more digital input channels in a task.
@@ -2108,16 +2150,18 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_digital_u_16(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u16(
+            self._handle, number_of_samples_per_channel, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_many_sample_port_uint32(
             self, data, number_of_samples_per_channel=READ_ALL_AVAILABLE,
             timeout=10.0):
         """
         Reads one or more 32-bit unsigned integer samples from one or
         more digital input channels in a task.
@@ -2192,16 +2236,18 @@
         """
         number_of_samples_per_channel = (
             self._task._calculate_num_samps_per_chan(
                 number_of_samples_per_channel))
 
         self._verify_array(data, number_of_samples_per_channel, True, True)
 
-        return _read_digital_u_32(
-            self._handle, data, number_of_samples_per_channel, timeout)
+        _, samps_per_chan_read = self._interpreter.read_digital_u32(
+            self._handle, number_of_samples_per_channel, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
+        
+        return samps_per_chan_read
 
     def read_one_sample_multi_line(self, data, timeout=10):
         """
         Reads a single boolean sample from one or more digital input
         channels in a task. The channels can contain multiple digital
         lines.
 
@@ -2243,15 +2289,16 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array_digital_lines(data, True, True)
 
-        _read_digital_lines(self._handle, data, 1, timeout)
+        _, samps_per_chan_read, num_bytes_per_samp= self._interpreter.read_digital_lines(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def read_one_sample_one_line(self, data, timeout=10):
         """
         Reads a single boolean sample from one or more digital input
         channels in a task. The channel can contain only one digital
         line.
 
@@ -2279,15 +2326,16 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array_digital_lines(data, True, False)
 
-        _read_digital_lines(self._handle, data, 1, timeout)
+        _, samps_per_chan_read, num_bytes_per_samp= self._interpreter.read_digital_lines(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def read_one_sample_port_byte(self, data, timeout=10):
         """
         Reads a single 8-bit unsigned integer sample from one or more
         digital input channels in a task.
 
         Use this method for devices with up to 8 lines per port.
@@ -2317,15 +2365,16 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array(data, 1, True, False)
 
-        _read_digital_u_8(self._handle, data, 1, timeout)
+        self._interpreter.read_digital_u8(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def read_one_sample_port_uint16(self, data, timeout=10):
         """
         Reads a single 16-bit unsigned integer sample from one or more
         digital input channels in a task.
 
         Use this method for devices with up to 16 lines per port.
@@ -2355,15 +2404,16 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array(data, 1, True, False)
 
-        _read_digital_u_16(self._handle, data, 1, timeout)
+        self._interpreter.read_digital_u16(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def read_one_sample_port_uint32(self, data, timeout=10):
         """
         Reads a single 32-bit unsigned integer sample from one or more
         digital input channels in a task.
 
         Use this method for devices with up to 32 lines per port.
@@ -2393,8 +2443,9 @@
                 nidaqmx.constants.WAIT_INFINITELY, the method waits
                 indefinitely. If you set timeout to 0, the method tries
                 once to read the requested samples and returns an error
                 if it is unable to.
         """
         self._verify_array(data, 1, True, False)
 
-        _read_digital_u_32(self._handle, data, 1, timeout)
+        self._interpreter.read_digital_u32(
+            self._handle, 1, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/stream_writers.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/stream_writers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import numpy
+
+from nidaqmx.constants import FillMode
 from nidaqmx import DaqError
-from nidaqmx._task_modules.write_functions import (
-    _write_analog_f_64, _write_analog_scalar_f_64, _write_binary_i_16,
-    _write_binary_i_32, _write_binary_u_16, _write_binary_u_32,
-    _write_ctr_freq, _write_ctr_ticks, _write_ctr_time, _write_ctr_freq_scalar,
-    _write_ctr_ticks_scalar, _write_ctr_time_scalar, _write_digital_u_8,
-    _write_digital_u_16, _write_digital_u_32, _write_digital_lines,
-    _write_digital_scalar_u_32)
 from nidaqmx.error_codes import DAQmxErrors
 
 __all__ = ['AnalogSingleChannelWriter', 'AnalogMultiChannelWriter',
            'AnalogUnscaledWriter', 'CounterWriter',
            'DigitalSingleChannelWriter', 'DigitalMultiChannelWriter']
 
 
@@ -42,14 +37,15 @@
                 method used. If you use a one sample write method, the
                 value is True; conversely, if you use a many sample 
                 write method, the value is False.
         """
         self._out_stream = task_out_stream
         self._task = task_out_stream._task
         self._handle = task_out_stream._task._handle
+        self._interpreter = task_out_stream._task._interpreter
 
         self._verify_array_shape = True
         self._auto_start = auto_start
 
     @property
     def auto_start(self):
         """
@@ -227,16 +223,16 @@
             successfully wrote.
         """
         self._verify_array(data, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_analog_f_64(
-            self._handle, data, data.shape[0], auto_start, timeout)
+        return self._interpreter.write_analog_f64(
+            self._handle, data.shape[0], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample(self, data, timeout=10):
         """
         Writes a single floating-point sample to a single analog output
         channel in a task.
 
         Args:
@@ -256,16 +252,16 @@
                 once to write the submitted samples. If the method could
                 not write all the submitted samples, it returns an error
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
-        return _write_analog_scalar_f_64(
-            self._handle, data, auto_start, timeout)
+        return self._interpreter.write_analog_scalar_f64(
+            self._handle, auto_start, timeout, data)
 
 
 class AnalogMultiChannelWriter(ChannelWriterBase):
     """
     Writes samples to one or more analog output channels in an NI-DAQmx
     task.
     """
@@ -310,16 +306,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_analog_f_64(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_analog_f64(
+            self._handle, data.shape[1], auto_start, timeout,FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample(self, data, timeout=10):
         """
         Writes a single floating-point sample to one or more analog
         output channels in a task.
 
         Args:
@@ -343,16 +339,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array(data, True, False)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_analog_f_64(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_analog_f64(
+            self._handle, 1, auto_start, timeout,FillMode.GROUP_BY_CHANNEL.value, data)
 
 
 class AnalogUnscaledWriter(ChannelWriterBase):
     """
     Writes unscaled samples to one or more analog output channels in
     an NI-DAQmx task.
     """
@@ -395,16 +391,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_binary_i_16(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_binary_i16(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_int32(self, data, timeout=10.0):
         """
         Writes one or more unscaled 32-bit integer samples to one or
         more analog output channels in a task.
 
         If the task uses on-demand timing, this method returns only
@@ -440,16 +436,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_binary_i_32(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_binary_i32(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_uint16(self, data, timeout=10.0):
         """
         Writes one or more unscaled 16-bit unsigned integer samples to
         one or more analog output channels in a task.
 
         If the task uses on-demand timing, this method returns only
@@ -485,16 +481,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_binary_u_16(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_binary_u16(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_uint32(self, data, timeout=10.0):
         """
         Writes one or more unscaled 32-bit unsigned integer samples to
         one or more analog output channels in a task.
 
         If the task uses on-demand timing, this method returns only
@@ -530,16 +526,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_binary_u_32(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_binary_u32(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
 
 class CounterWriter(ChannelWriterBase):
     """
     Writes samples to a counter output channel in an NI-DAQmx task.
     """
 
@@ -586,17 +582,17 @@
         """
         self._verify_array(frequencies, False, True)
         self._verify_array(duty_cycles, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_ctr_freq(
-            self._handle, frequencies, duty_cycles, frequencies.shape[0],
-            auto_start, timeout)
+        return self._interpreter.write_ctr_freq(
+            self._handle, frequencies.shape[0], auto_start, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, frequencies, duty_cycles)
 
     def write_many_sample_pulse_ticks(
             self, high_ticks, low_ticks, timeout=10.0):
         """
         Writes one or more pulse samples in terms of ticks to a single
         counter output channel in a task.
 
@@ -637,17 +633,17 @@
         """
         self._verify_array(high_ticks, False, True)
         self._verify_array(low_ticks, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_ctr_ticks(
-            self._handle, high_ticks, low_ticks, high_ticks.shape[0],
-            auto_start, timeout)
+        return self._interpreter.write_ctr_ticks(
+            self._handle, high_ticks.shape[0], auto_start, timeout,
+            FillMode.GROUP_BY_CHANNEL.value, high_ticks, low_ticks)
 
     def write_many_sample_pulse_time(
             self, high_times, low_times, timeout=10.0):
         """
         Writes one or more pulse samples in terms of time to a single
         counter output channel in a task.
 
@@ -688,17 +684,17 @@
         """
         self._verify_array(high_times, False, True)
         self._verify_array(low_times, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_ctr_time(
-            self._handle, high_times, low_times, high_times.shape[0],
-            auto_start, timeout)
+        return self._interpreter.write_ctr_time(
+            self._handle, high_times.shape[0], auto_start, timeout, 
+            FillMode.GROUP_BY_CHANNEL.value, high_times, low_times)
 
     def write_one_sample_pulse_frequency(
             self, frequency, duty_cycle, timeout=10):
         """
         Writes a new pulse frequency and duty cycle to a single counter
         output channel in a task.
 
@@ -723,16 +719,16 @@
                 once to write the submitted samples. If the method could
                 not write all the submitted samples, it returns an error
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
-        return _write_ctr_freq_scalar(
-            self._handle, frequency, duty_cycle, auto_start, timeout)
+        return self._interpreter.write_ctr_freq_scalar(
+            self._handle, auto_start, timeout, frequency, duty_cycle)
 
     def write_one_sample_pulse_ticks(
             self, high_ticks, low_ticks, timeout=10):
         """
         Writes a new pulse high tick count and low tick count to a
         single counter output channel in a task.
 
@@ -752,16 +748,16 @@
                 once to write the submitted samples. If the method could
                 not write all the submitted samples, it returns an error
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
-        return _write_ctr_ticks_scalar(
-            self._handle, high_ticks, low_ticks, auto_start, timeout)
+        return self._interpreter.write_ctr_ticks_scalar(
+            self._handle, auto_start, timeout, high_ticks, low_ticks)
 
     def write_one_sample_pulse_time(
             self, high_time, low_time, timeout=10):
         """
         Writes a new pulse high time and low time to a single counter
         output channel in a task.
 
@@ -781,16 +777,16 @@
                 once to write the submitted samples. If the method could
                 not write all the submitted samples, it returns an error
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
-        return _write_ctr_time_scalar(
-            self._handle, high_time, low_time, auto_start, timeout)
+        return self._interpreter.write_ctr_time_scalar(
+            self._handle, auto_start, timeout, high_time, low_time)
 
 
 class DigitalSingleChannelWriter(ChannelWriterBase):
     """
     Writes samples to a single digital output channel in an NI-DAQmx
     task.
     """
@@ -833,16 +829,16 @@
             successfully wrote.
         """
         self._verify_array(data, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_8(
-            self._handle, data, data.shape[0], auto_start, timeout)
+        return self._interpreter.write_digital_u8(
+            self._handle, data.shape[0], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_many_sample_port_uint16(self, data, timeout=10.0):
         """
         Writes one or more 16-bit unsigned integer samples to a single
         digital output channel in a task.
 
         Use this method for devices with up to 16 lines per port.
@@ -878,16 +874,16 @@
             successfully wrote.
         """
         self._verify_array(data, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_16(
-            self._handle, data, data.shape[0], auto_start, timeout)
+        return self._interpreter.write_digital_u16(
+            self._handle, data.shape[0], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_many_sample_port_uint32(self, data, timeout=10.0):
         """
         Writes one or more 32-bit unsigned integer samples to a single
         digital output channel in a task.
 
         Use this method for devices with up to 32 lines per port.
@@ -923,16 +919,16 @@
             successfully wrote.
         """
         self._verify_array(data, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_32(
-            self._handle, data, data.shape[0], auto_start, timeout)
+        return self._interpreter.write_digital_u32(
+            self._handle, data.shape[0], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_multi_line(self, data, timeout=10):
         """
         Writes a single boolean sample to a single digital output
         channel in a task. The channel can contain multiple digital
         lines.
 
@@ -953,16 +949,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array_digital_lines(data, False, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_lines(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_lines(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_one_line(self, data, timeout=10):
         """
         Writes a single boolean sample to a single digital output
         channel in a task. The channel can contain only one digital
         line.
 
@@ -982,16 +978,16 @@
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
         numpy_array = numpy.asarray([data], dtype=bool)
 
-        return _write_digital_lines(
-            self._handle, numpy_array, 1, auto_start, timeout)
+        return self._interpreter.write_digital_lines(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, numpy_array)
 
     def write_one_sample_port_byte(self, data, timeout=10):
         """
         Writes a single 8-bit unsigned integer sample to a single
         digital output channel in a task.
 
         Use this method for devices with up to 8 lines per port.
@@ -1012,16 +1008,16 @@
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
         numpy_array = numpy.asarray([data], dtype=numpy.uint8)
 
-        return _write_digital_u_8(
-            self._handle, numpy_array, 1, auto_start, timeout)
+        return self._interpreter.write_digital_u8(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, numpy_array)
 
     def write_one_sample_port_uint16(self, data, timeout=10):
         """
         Writes a single 16-bit unsigned integer sample to a single
         digital output channel in a task.
 
         Use this method for devices with up to 16 lines per port.
@@ -1042,16 +1038,16 @@
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
         numpy_array = numpy.asarray([data], dtype=numpy.uint16)
 
-        return _write_digital_u_16(
-            self._handle, numpy_array, 1, auto_start, timeout)
+        return self._interpreter.write_digital_u16(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, numpy_array)
 
     def write_one_sample_port_uint32(self, data, timeout=10):
         """
         Writes a single 32-bit unsigned integer sample to a single
         digital output channel in a task.
 
         Use this method for devices with up to 32 lines per port.
@@ -1070,16 +1066,16 @@
                 once to write the submitted samples. If the method could
                 not write all the submitted samples, it returns an error
                 and the number of samples successfully written.
         """
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
         
-        return _write_digital_scalar_u_32(
-            self._handle, data, auto_start, timeout)
+        return self._interpreter.write_digital_scalar_u32(
+            self._handle, auto_start, timeout, data)
 
 
 class DigitalMultiChannelWriter(ChannelWriterBase):
     """
     Writes samples to one or more digital output channels in an NI-DAQmx
     task.
     """
@@ -1126,16 +1122,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_8(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_digital_u8(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_many_sample_port_uint16(self, data, timeout=10.0):
         """
         Writes one or more 16-bit unsigned integer samples to one or
         more digital output channels in a task.
 
         Use this method for devices with up to 16 lines per port.
@@ -1175,16 +1171,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_16(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_digital_u16(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_many_sample_port_uint32(self, data, timeout=10.0):
         """
         Writes one or more 32-bit unsigned integer samples to one or
         more digital output channels in a task.
 
         Use this method for devices with up to 32 lines per port.
@@ -1224,16 +1220,16 @@
             successfully wrote to each channel in the task.
         """
         self._verify_array(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else False)
 
-        return _write_digital_u_32(
-            self._handle, data, data.shape[1], auto_start, timeout)
+        return self._interpreter.write_digital_u32(
+            self._handle, data.shape[1], auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_multi_line(self, data, timeout=10):
         """
         Writes a single boolean sample to one or more digital output
         channels in a task. The channel can contain multiple digital
         lines.
 
@@ -1258,16 +1254,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array_digital_lines(data, True, True)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_lines(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_lines(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_one_line(self, data, timeout=10):
         """
         Writes a single boolean sample to one or more digital output
         channels in a task. The channel can contain only one digital
         line.
 
@@ -1292,16 +1288,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array_digital_lines(data, True, False)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_lines(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_lines(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_port_byte(self, data, timeout=10):
         """
         Writes a single 8-bit unsigned integer sample to one or more
         digital output channels in a task.
 
         Use this method for devices with up to 8 lines per port.
@@ -1327,16 +1323,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array(data, True, False)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_u_8(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_u8(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_port_uint16(self, data, timeout=10):
         """
         Writes a single 16-bit unsigned integer sample to one or more
         digital output channels in a task.
 
         Use this method for devices with up to 16 lines per port.
@@ -1362,16 +1358,16 @@
                 and the number of samples successfully written.
         """
         self._verify_array(data, True, False)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_u_16(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_u16(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
     def write_one_sample_port_uint32(self, data, timeout=10):
         """
         Writes a single 32-bit unsigned integer sample to one or more
         digital output channels in a task.
 
         Use this method for devices with up to 32 lines per port.
@@ -1397,9 +1393,9 @@
                 and the number of samples successfully written.
         """
         self._verify_array(data, True, False)
         
         auto_start = (self._auto_start if self._auto_start is not 
                       AUTO_START_UNSET else True)
 
-        return _write_digital_u_32(
-            self._handle, data, 1, auto_start, timeout)
+        return self._interpreter.write_digital_u32(
+            self._handle, 1, auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/system/_collections/device_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_scale_collection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,94 @@
-import ctypes
 from collections.abc import Sequence
 
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import (
-    check_for_error, is_string_buffer_too_small, DaqError)
+from nidaqmx.errors import DaqError
 from nidaqmx.error_codes import DAQmxErrors
-from nidaqmx.system.device import Device
+from nidaqmx.system.storage.persisted_scale import PersistedScale, _PersistedScaleAlternateConstructor
 from nidaqmx.utils import unflatten_channel_string
 
-
-class DeviceCollection(Sequence):
+class PersistedScaleCollection(Sequence):
     """
-    Contains the collection of devices for a DAQmx system.
+    Contains the collection of custom scales on a DAQmx system.
     
     This class defines methods that implements a container object.
     """
+    def __init__(self, interpreter):
+        """
+        Do not construct this object directly; instead, call nidaqmx.system.System.local().scales.
+        """
+        self._interpreter = interpreter
+    
     def __contains__(self, item):
-        device_names = self.device_names
+        scale_names = self.scale_names
 
         if isinstance(item, str):
             items = unflatten_channel_string(item)
-            return all([i in device_names for i in items])
-        elif isinstance(item, Device):
-            return item.name in device_names
-        return False
+            return all([i in scale_names for i in items])
+        elif isinstance(item, PersistedScale):
+            return item._name in scale_names
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return True
         return False
 
     def __getitem__(self, index):
         """
-        Indexes a subset of devices on this device collection.
+        Indexes a subset of custom scales on this collection.
 
         Args:
-            index: The value of the index. The following index types are
-                supported:
-                - str: Name of the device. You also can specify a string
-                    that contains a list or range of names to this input.
-                    If you have a list of names, use the DAQmx Flatten
-                    Channel String function to convert the list to a
-                    string.
-                - int: Index/position of the device in the collection.
-                - slice: Range of the indexes/positions of devices in the
+            index: The value of the index. The following index types
+                are supported:
+                - str: Name of the custom scale. You also can specify
+                    a string that contains a list or range of names to
+                    this input. If you have a list of names, use the
+                    DAQmx Flatten Channel String function to convert
+                    the list to a string.
+                - int: Index/position of the custom scale in the
                     collection.
+                - slice: Range of the indexes/positions of custom scales
+                    in the collection.
         Returns:
-            List[nidaqmx.system.device.Device]: 
+            List[nidaqmx.system.storage.persisted_scale.PersistedScale]:
             
-            Indicates the subset of devices indexed.
+            Indicates the subset of custom scales indexed.
         """
         if isinstance(index, int):
-            return Device(self.device_names[index])
+            return _PersistedScaleAlternateConstructor(self.scale_names[index], self._interpreter)
         elif isinstance(index, slice):
-            return [Device(name) for name in self.device_names[index]]
+            return [_PersistedScaleAlternateConstructor(name, self._interpreter) for name in
+                    self.scale_names[index]]
         elif isinstance(index, str):
-            device_names = unflatten_channel_string(index)
-            if len(device_names) == 1:
-                return Device(device_names[0])
-            return [Device(name) for name in device_names]
+            names = unflatten_channel_string(index)
+            if len(names) == 1:
+                return _PersistedScaleAlternateConstructor(names[0], self._interpreter)
+            return [_PersistedScaleAlternateConstructor(name, self._interpreter) for name in names]
         else:
             raise DaqError(
                 'Invalid index type "{}" used to access collection.'
                 .format(type(index)), DAQmxErrors.UNKNOWN)
 
     def __iter__(self):
-        for device_name in self.device_names:
-            yield Device(device_name)
+        for scale_name in self.scale_names:
+            yield _PersistedScaleAlternateConstructor(scale_name, self._interpreter)
 
     def __len__(self):
-        return len(self.device_names)
+        return len(self.scale_names)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __reversed__(self):
-        device_names = self.device_names
-        device_names.reverse()
+        scale_names = self.scale_names
+        scale_names.reverse()
 
-        for device_name in device_names:
-            yield Device(device_name)
+        for scale_name in scale_names:
+            yield _PersistedScaleAlternateConstructor(scale_name, self._interpreter)
 
     @property
-    def device_names(self):
+    def scale_names(self):
         """
-        List[str]: Indicates the names of all devices on this device
+        List[str]: Indicates the names of all the custom scales on this
             collection.
         """
-        cfunc = lib_importer.windll.DAQmxGetSysDevNames
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        ctypes.c_char_p, ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return unflatten_channel_string(val.value.decode('ascii'))
+        val = self._interpreter.get_system_info_attribute_string(0x1266)
+        return unflatten_channel_string(val)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/system/_collections/persisted_task_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_collections/persisted_task_collection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-import ctypes
 from collections.abc import Sequence
 
-from nidaqmx._lib import lib_importer, ctypes_byte_str
-from nidaqmx.errors import (
-    check_for_error, is_string_buffer_too_small, DaqError)
+from nidaqmx.errors import DaqError
 from nidaqmx.error_codes import DAQmxErrors
-from nidaqmx.system.storage.persisted_task import PersistedTask
+from nidaqmx.system.storage.persisted_task import PersistedTask, _PersistedTaskAlternateConstructor
 from nidaqmx.utils import unflatten_channel_string
 
-
 class PersistedTaskCollection(Sequence):
     """
     Contains the collection of task saved on a DAQmx system.
     
     This class defines methods that implements a container object.
     """
+    def __init__(self, interpreter):
+        """
+        Do not construct this object directly; instead, call nidaqmx.system.System.local().tasks.
+        """
+        self._interpreter = interpreter
+    
     def __contains__(self, item):
         task_names = self.task_names
 
         if isinstance(item, str):
             items = unflatten_channel_string(item)
             return all([i in task_names for i in items])
         elif isinstance(item, PersistedTask):
@@ -47,69 +49,45 @@
                     in the collection.
         Returns:
             List[nidaqmx.system.storage.persisted_task.PersistedTask]:
             
             Indicates the subset of saved tasks indexed.
         """
         if isinstance(index, int):
-            return PersistedTask(self.task_names[index])
+            return _PersistedTaskAlternateConstructor(self.task_names[index], self._interpreter)
         elif isinstance(index, slice):
-            return [PersistedTask(name) for name in
+            return [_PersistedTaskAlternateConstructor(name, self._interpreter) for name in
                     self.task_names[index]]
         elif isinstance(index, str):
             names = unflatten_channel_string(index)
             if len(names) == 1:
-                return PersistedTask(names[0])
-            return [PersistedTask(name) for name in names]
+                return _PersistedTaskAlternateConstructor(names[0], self._interpreter)
+            return [_PersistedTaskAlternateConstructor(name, self._interpreter) for name in names]
         else:
             raise DaqError(
                 'Invalid index type "{}" used to access collection.'
                 .format(type(index)), DAQmxErrors.UNKNOWN)
 
     def __iter__(self):
         for task_name in self.task_names:
-            yield PersistedTask(task_name)
+            yield _PersistedTaskAlternateConstructor(task_name, self._interpreter)
 
     def __len__(self):
         return len(self.task_names)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __reversed__(self):
         task_names = self.task_names
         task_names.reverse()
 
         for task_name in task_names:
-            yield PersistedTask(task_name)
+            yield _PersistedTaskAlternateConstructor(task_name, self._interpreter)
 
     @property
     def task_names(self):
         """
         List[str]: Indicates the names of all the tasks on this collection.
         """
-        cfunc = lib_importer.windll.DAQmxGetSysTasks
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        ctypes.c_char_p, ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return unflatten_channel_string(val.value.decode('ascii'))
+        val = self._interpreter.get_system_info_attribute_string(0x1267)
+        return unflatten_channel_string(val)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/system/_watchdog_modules/expiration_states_collection.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 class ExpirationStatesCollection:
     """
     Contains the collection of expiration states for a DAQmx Watchdog Task.
     
     This class defines methods that implements a container object.
     """
-    def __init__(self, task_handle):
+    def __init__(self, task_handle, interpreter):
         self._handle = task_handle
+        self._interpreter = interpreter
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self._handle == other._handle
         return False
 
     def __hash__(self):
-        return hash(self._handle.value)
+        return self._interpreter.hash_task_handle(self._handle)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __getitem__(self, index):
         """
         Indexes an expiration state on this collection.
@@ -31,12 +32,12 @@
                 expiration state to retrieve.
         Returns:
             nidaqmx.system._watchdog_modules.expiration_state.ExpirationState:
             
             The object representing the indexed expiration state.
         """
         if isinstance(index, str):
-            return ExpirationState(self._handle, index)
+            return ExpirationState(self._handle, index, self._interpreter)
         else:
             raise DaqError(
                 'Invalid index type "{}" used to access expiration states.'
                 .format(type(index)), -1)
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/task.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-import ctypes
-import numpy
+import threading
 import warnings
+from enum import Enum
+
+import numpy
 
-from nidaqmx._lib import lib_importer, ctypes_byte_str, c_bool32
+from nidaqmx import utils
 from nidaqmx._task_modules.channels.channel import Channel
 from nidaqmx._task_modules.export_signals import ExportSignals
 from nidaqmx._task_modules.in_stream import InStream
-from nidaqmx._task_modules.read_functions import (
-    _read_analog_f_64, _read_power_f_64,
-    _read_digital_lines, _read_digital_u_32,
-    _read_ctr_freq,_read_ctr_time, _read_ctr_ticks,
-    _read_counter_u_32_ex, _read_counter_f_64_ex)
 from nidaqmx._task_modules.timing import Timing
 from nidaqmx._task_modules.triggers import Triggers
 from nidaqmx._task_modules.out_stream import OutStream
 from nidaqmx._task_modules.ai_channel_collection import (
     AIChannelCollection)
 from nidaqmx._task_modules.ao_channel_collection import (
     AOChannelCollection)
@@ -22,24 +19,21 @@
     CIChannelCollection)
 from nidaqmx._task_modules.co_channel_collection import (
     COChannelCollection)
 from nidaqmx._task_modules.di_channel_collection import (
     DIChannelCollection)
 from nidaqmx._task_modules.do_channel_collection import (
     DOChannelCollection)
-from nidaqmx._task_modules.write_functions import (
-    _write_analog_f_64, _write_digital_lines, _write_digital_u_32,
-    _write_ctr_freq, _write_ctr_time, _write_ctr_ticks)
 from nidaqmx.constants import (
-    AcquisitionType, ChannelType, UsageTypeAI, UsageTypeCI, EveryNSamplesEventType,
+    AcquisitionType, ChannelType, FillMode, UsageTypeAI, UsageTypeCI, EveryNSamplesEventType,
     READ_ALL_AVAILABLE, UsageTypeCO, _Save)
 from nidaqmx.error_codes import DAQmxErrors
 from nidaqmx.errors import (
-    check_for_error, is_string_buffer_too_small, DaqError, DaqResourceWarning)
-from nidaqmx.system.device import Device
+    DaqError, DaqResourceWarning)
+from nidaqmx.system.device import _DeviceAlternateConstructor
 from nidaqmx.types import CtrFreq, CtrTick, CtrTime, PowerMeasurement
 from nidaqmx.utils import unflatten_channel_string, flatten_channel_string
 
 __all__ = ['Task']
 
 
 class UnsetNumSamplesSentinel:
@@ -58,282 +52,202 @@
 
 
 class Task:
     """
     Represents a DAQmx Task.
     """
 
-    def __init__(self, new_task_name=''):
+    def __init__(self, new_task_name='', *, grpc_options=None):
         """
         Creates a DAQmx task.
 
         Args:
             new_task_name (Optional[str]): Specifies the name to assign to
                 the task.
 
                 If you use this method in a loop and specify a name for the
                 task, you must use the DAQmx Clear Task method within the loop
                 after you are finished with the task. Otherwise, NI-DAQmx
                 attempts to create multiple tasks with the same name, which
                 results in an error.
+
+            grpc_options (Optional[:class:`~nidaqmx.GrpcSessionOptions`]): Specifies
+                the gRPC session options.
         """
-        self._handle = lib_importer.task_handle(0)
+        # Initialize the fields that __del__ accesses so it doesn't crash when __init__ raises an exception.
+        self._handle = None
+        self._close_on_exit = False
+        self._saved_name = new_task_name  # _initialize sets this to the name assigned by DAQmx.
+        self._grpc_options = grpc_options
+        self._event_handlers = {}
+
+        if grpc_options and not (
+            grpc_options.session_name == "" or grpc_options.session_name == new_task_name
+        ):
+            raise DaqError(
+                f'Unsupported session name: "{grpc_options.session_name}". If a session name is specified, it must match the task name.',
+                DAQmxErrors.UNKNOWN,
+                task_name=new_task_name)
 
-        cfunc = lib_importer.windll.DAQmxCreateTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        ctypes_byte_str,
-                        ctypes.POINTER(lib_importer.task_handle)]
-
-        error_code = cfunc(
-            new_task_name, ctypes.byref(self._handle))
-        check_for_error(error_code)
+        self._interpreter = utils._select_interpreter(grpc_options)
+        self._handle, self._close_on_exit = self._interpreter.create_task(new_task_name)
 
-        self._initialize(self._handle)
+        self._initialize(self._handle, self._interpreter)
 
     def __del__(self):
-        if self._handle:
+        if self._handle is not None and self._close_on_exit and self._grpc_options is None:
             warnings.warn(
                 'Task of name "{}" was not explicitly closed before it was '
                 'destructed. Resources on the task device may still be '
-                'reserved.'.format(self._saved_name), DaqResourceWarning)
+                'reserved.'.format(self._saved_name),
+                DaqResourceWarning
+            )
+        elif (
+            self._grpc_options is not None
+            and self._event_handlers
+        ):
+            warnings.warn(
+                'Task of name "{}" was not explicitly closed before it was '
+                'destructed. Event handlers may still be active.'.format(self._saved_name),
+                DaqResourceWarning
+            )
 
     def __enter__(self):
         return self
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
             return self._handle == other._handle
         return False
 
     def __exit__(self, type, value, traceback):
-        self.close()
+        if self._close_on_exit:
+            self.close()
 
     def __hash__(self):
-        return hash(self._handle)
+        return self._interpreter.hash_task_handle(self._handle)
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __repr__(self):
-        return f'Task(name={self.name})'
+        return f'Task(name={self._saved_name})'
 
     @property
     def name(self):
         """
         str: Indicates the name of the task.
         """
-        cfunc = lib_importer.windll.DAQmxGetTaskName
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.c_char_p,
-                        ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return val.value.decode('ascii')
+        val = self._interpreter.get_task_attribute_string(self._handle, 0x1276)
+        return val
 
     @property
     def channels(self):
         """
-        :class:`nidaqmx._task_modules.channels.channel.Channel`: Specifies 
-            a channel object that represents the entire list of virtual 
+        :class:`nidaqmx._task_modules.channels.channel.Channel`: Specifies
+            a channel object that represents the entire list of virtual
             channels in this task.
         """
         return Channel._factory(
-            self._handle, flatten_channel_string(self.channel_names))
+            self._handle, flatten_channel_string(self.channel_names), self._interpreter)
 
     @property
     def channel_names(self):
         """
         List[str]: Indicates the names of all virtual channels in the task.
         """
-        cfunc = lib_importer.windll.DAQmxGetTaskChannels
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.c_char_p,
-                        ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return unflatten_channel_string(val.value.decode('ascii'))
+        val = self._interpreter.get_task_attribute_string(self._handle, 0x1273)
+        return unflatten_channel_string(val)
 
     @property
     def number_of_channels(self):
         """
         int: Indicates the number of virtual channels in the task.
         """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetTaskNumChans
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+        val = self._interpreter.get_task_attribute_uint32(self._handle, 0x2181)
+        return val
 
     @property
     def devices(self):
         """
-        List[:class:`nidaqmx.system.device.Device`]: Indicates a list 
+        List[:class:`nidaqmx.system.device.Device`]: Indicates a list
             of Device objects representing all the devices in the task.
         """
-        cfunc = lib_importer.windll.DAQmxGetTaskDevices
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.c_char_p,
-                        ctypes.c_uint]
-
-        temp_size = 0
-        while True:
-            val = ctypes.create_string_buffer(temp_size)
-
-            size_or_code = cfunc(
-                self._handle, val, temp_size)
-
-            if is_string_buffer_too_small(size_or_code):
-                # Buffer size must have changed between calls; check again.
-                temp_size = 0
-            elif size_or_code > 0 and temp_size == 0:
-                # Buffer size obtained, use to retrieve data.
-                temp_size = size_or_code
-            else:
-                break
-
-        check_for_error(size_or_code)
-
-        return [Device(v) for v in
-                unflatten_channel_string(val.value.decode('ascii'))]
+        val = self._interpreter.get_task_attribute_string(self._handle, 0x230e)
+        return [_DeviceAlternateConstructor(v, self._interpreter) for v in
+                unflatten_channel_string(val)]
 
     @property
     def number_of_devices(self):
         """
         int: Indicates the number of devices in the task.
         """
-        val = ctypes.c_uint()
-
-        cfunc = lib_importer.windll.DAQmxGetTaskNumDevices
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.POINTER(ctypes.c_uint)]
-
-        error_code = cfunc(
-            self._handle, ctypes.byref(val))
-        check_for_error(error_code)
-
-        return val.value
+        val = self._interpreter.get_task_attribute_uint32(self._handle, 0x29ba)
+        return val
 
     @property
     def ai_channels(self):
         """
         :class:`nidaqmx._task_modules.ai_channel_collection.AIChannelCollection`:
             Gets the collection of analog input channels for this task.
         """
         return self._ai_channels
 
     @property
     def ao_channels(self):
         """
-        :class:`nidaqmx._task_modules.ao_channel_collection.AOChannelCollection`: 
+        :class:`nidaqmx._task_modules.ao_channel_collection.AOChannelCollection`:
             Gets the collection of analog output channels for this task.
         """
         return self._ao_channels
 
     @property
     def ci_channels(self):
         """
-        :class:`nidaqmx._task_modules.ci_channel_collection.CIChannelCollection`: 
+        :class:`nidaqmx._task_modules.ci_channel_collection.CIChannelCollection`:
             Gets the collection of counter input channels for this task.
         """
         return self._ci_channels
 
     @property
     def co_channels(self):
         """
-        :class:`nidaqmx._task_modules.co_channel_collection.COChannelCollection`: 
+        :class:`nidaqmx._task_modules.co_channel_collection.COChannelCollection`:
             Gets the collection of counter output channels for this task.
         """
         return self._co_channels
 
     @property
     def di_channels(self):
         """
-        :class:`nidaqmx._task_modules.di_channel_collection.DIChannelCollection`: 
+        :class:`nidaqmx._task_modules.di_channel_collection.DIChannelCollection`:
             Gets the collection of digital input channels for this task.
         """
         return self._di_channels
 
     @property
     def do_channels(self):
         """
-        :class:`nidaqmx._task_modules.do_channel_collection.DOChannelCollection`: 
+        :class:`nidaqmx._task_modules.do_channel_collection.DOChannelCollection`:
             Gets the collection of digital output channels for this task.
         """
         return self._do_channels
 
     @property
     def export_signals(self):
         """
-        :class:`nidaqmx._task_modules.export_signals.ExportSignals`: Gets the 
+        :class:`nidaqmx._task_modules.export_signals.ExportSignals`: Gets the
             exported signal configurations for the task.
         """
         return self._export_signals
 
     @property
     def in_stream(self):
         """
-        :class:`nidaqmx._task_modules.in_stream.InStream`: Gets the read 
+        :class:`nidaqmx._task_modules.in_stream.InStream`: Gets the read
             configurations for the task.
         """
         return self._in_stream
 
     @property
     def out_stream(self):
         """
@@ -341,57 +255,51 @@
             write configurations for the task.
         """
         return self._out_stream
 
     @property
     def timing(self):
         """
-        :class:`nidaqmx._task_modules.timing.Timing`: Gets the timing 
+        :class:`nidaqmx._task_modules.timing.Timing`: Gets the timing
             configurations for the task.
         """
         return self._timing
 
     @property
     def triggers(self):
         """
         :class:`nidaqmx._task_modules.triggers.Triggers`: Gets the trigger
             configurations for the task.
         """
         return self._triggers
 
-    def _initialize(self, task_handle):
+    def _initialize(self, task_handle, interpreter):
         """
         Instantiates and populates various attributes used by this task.
 
         Args:
             task_handle (TaskHandle): Specifies the handle for this task.
         """
         # Saved name is used in self.close() to throw graceful error on
         # double closes.
         self._saved_name = self.name
 
-        self._ai_channels = AIChannelCollection(task_handle)
-        self._ao_channels = AOChannelCollection(task_handle)
-        self._ci_channels = CIChannelCollection(task_handle)
-        self._co_channels = COChannelCollection(task_handle)
-        self._di_channels = DIChannelCollection(task_handle)
-        self._do_channels = DOChannelCollection(task_handle)
-        self._export_signals = ExportSignals(task_handle)
-        self._in_stream = InStream(self)
-        self._timing = Timing(task_handle)
-        self._triggers = Triggers(task_handle)
-        self._out_stream = OutStream(self)
-
-        # These lists keep C callback objects in memory as ctypes doesn't.
-        # Program will crash if callback is made after object is garbage
-        # collected.
-        self._done_event_callbacks = []
-        self._every_n_transferred_event_callbacks = []
-        self._every_n_acquired_event_callbacks = []
-        self._signal_event_callbacks = []
+        self._ai_channels = AIChannelCollection(task_handle, interpreter)
+        self._ao_channels = AOChannelCollection(task_handle, interpreter)
+        self._ci_channels = CIChannelCollection(task_handle, interpreter)
+        self._co_channels = COChannelCollection(task_handle, interpreter)
+        self._di_channels = DIChannelCollection(task_handle, interpreter)
+        self._do_channels = DOChannelCollection(task_handle, interpreter)
+        self._export_signals = ExportSignals(task_handle, interpreter)
+        self._in_stream = InStream(self, interpreter)
+        self._timing = Timing(task_handle, interpreter)
+        self._triggers = Triggers(task_handle, interpreter)
+        self._out_stream = OutStream(self, interpreter)
+
+        self._event_handler_lock = threading.Lock()
 
     def _calculate_num_samps_per_chan(self, num_samps_per_chan):
         """
         Calculates the actual number of samples per channel to read.
 
         This method is necessary because the number of samples per channel
         can be set to NUM_SAMPLES_UNSET or -1, where each value entails a
@@ -423,26 +331,17 @@
             global_channels (List[nidaqmx.system.storage.persisted_channel.PersistedChannel]):
                 Specifies the channels to add to the task.
 
                 These channels must be valid channels available from MAX.
                 If you pass an invalid channel, NI-DAQmx returns an error.
                 This value is ignored if it is empty.
         """
-        cfunc = lib_importer.windll.DAQmxAddGlobalChansToTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str]
-
         channels = flatten_channel_string([g._name for g in global_channels])
 
-        error_code = cfunc(
-            self._handle, channels)
-        check_for_error(error_code)
+        self._interpreter.add_global_chans_to_task(self._handle, channels)
 
     def close(self):
         """
         Clears the task.
 
         Before clearing, this method aborts the task, if necessary,
         and releases any resources the task reserved. You cannot use a task
@@ -454,71 +353,58 @@
         """
         if self._handle is None:
             warnings.warn(
                 'Attempted to close NI-DAQmx task of name "{}" but task was '
                 'already closed.'.format(self._saved_name), DaqResourceWarning)
             return
 
-        cfunc = lib_importer.windll.DAQmxClearTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle]
-
-        error_code = cfunc(
-            self._handle)
-        check_for_error(error_code)
-
+        first_exception = None
+        try:
+            self._interpreter.clear_task(self._handle)
+        except Exception as ex:
+            first_exception = first_exception or ex
         self._handle = None
 
+        with self._event_handler_lock:
+            event_handlers = self._event_handlers
+            self._event_handlers = {}
+
+        for event_handler in event_handlers.values():
+            try:
+                event_handler.close()
+            except Exception as ex:
+                first_exception = first_exception or ex
+
+        if first_exception:
+            raise first_exception
+
     def control(self, action):
         """
         Alters the state of a task according to the action you specify.
 
         Args:
             action (nidaqmx.constants.TaskMode): Specifies how to alter
                 the task state.
         """
-        cfunc = lib_importer.windll.DAQmxTaskControl
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.c_int]
-
-        error_code = cfunc(
-            self._handle, action.value)
-        check_for_error(error_code)
+        self._interpreter.task_control(self._handle, action.value)
 
     def is_task_done(self):
         """
         Queries the status of the task and indicates if it completed
         execution. Use this function to ensure that the specified
         operation is complete before you stop the task.
 
         Returns:
             bool:
 
             Indicates if the measurement or generation completed.
         """
-        is_task_done = c_bool32()
-
-        cfunc = lib_importer.windll.DAQmxIsTaskDone
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes.POINTER(c_bool32)]
-
-        error_code = cfunc(
-            self._handle, ctypes.byref(is_task_done))
-        check_for_error(error_code)
+        is_task_done = self._interpreter.is_task_done(self._handle)
 
-        return is_task_done.value
+        return is_task_done
 
     def read(self, number_of_samples_per_channel=NUM_SAMPLES_UNSET,
              timeout=10.0):
         """
         Reads samples from the task or virtual channels you specify.
 
         This read method is dynamic, and is capable of inferring an appropriate
@@ -613,30 +499,29 @@
                 array_shape = (number_of_channels,
                                number_of_samples_per_channel)
             else:
                 array_shape = number_of_channels
         else:
             array_shape = number_of_samples_per_channel
 
-        # Analog Input
         if read_chan_type == ChannelType.ANALOG_INPUT:
             has_power_chan = False
             for chan in channels_to_read:
                 meas_type = chan.ai_meas_type
                 has_power_chan = meas_type == UsageTypeAI.POWER
                 if has_power_chan:
                     break
 
             if has_power_chan:
                 voltages = numpy.zeros(array_shape, dtype=numpy.float64)
                 currents = numpy.zeros(array_shape, dtype=numpy.float64)
 
-                samples_read = _read_power_f_64(
-                    self._handle, voltages, currents,
-                    number_of_samples_per_channel, timeout)
+                _, _, samples_read = self._interpreter.read_power_f64(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, voltages, currents)
 
                 if number_of_channels > 1:
                     if number_of_samples_per_channel == 1:
                         # n channel, 1 sample
                         data = []
                         for v, i in zip(voltages, currents):
                             data.append(PowerMeasurement(voltage=v, current=i))
@@ -660,79 +545,81 @@
                         # 1 channel, n samples
                         data = []
                         for v, i in zip(voltages, currents):
                             data.append(PowerMeasurement(voltage=v, current=i))
                         return data[:samples_read]
             else:
                 data = numpy.zeros(array_shape, dtype=numpy.float64)
-                samples_read = _read_analog_f_64(
-                    self._handle, data, number_of_samples_per_channel, timeout)
+                _, samples_read = self._interpreter.read_analog_f64(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, data)
 
-        # Digital Input or Digital Output
         elif (read_chan_type == ChannelType.DIGITAL_INPUT or
                 read_chan_type == ChannelType.DIGITAL_OUTPUT):
             if self.in_stream.di_num_booleans_per_chan == 1:
                 data = numpy.zeros(array_shape, dtype=bool)
-                samples_read = _read_digital_lines(
-                    self._handle, data, number_of_samples_per_channel, timeout
-                    ).samps_per_chan_read
+                _, samples_read, _ = self._interpreter.read_digital_lines(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, data)
             else:
                 data = numpy.zeros(array_shape, dtype=numpy.uint32)
-                samples_read = _read_digital_u_32(
-                    self._handle, data, number_of_samples_per_channel, timeout)
+                _, samples_read = self._interpreter.read_digital_u32(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, data)
 
-        # Counter Input
         elif read_chan_type == ChannelType.COUNTER_INPUT:
             meas_type = channels_to_read.ci_meas_type
 
             if meas_type == UsageTypeCI.PULSE_FREQ:
                 frequencies = numpy.zeros(array_shape, dtype=numpy.float64)
                 duty_cycles = numpy.zeros(array_shape, dtype=numpy.float64)
 
-                samples_read = _read_ctr_freq(
-                    self._handle, frequencies, duty_cycles,
-                    number_of_samples_per_channel, timeout)
+                _, _, samples_read = self._interpreter.read_ctr_freq(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, frequencies, duty_cycles)
 
                 data = []
                 for f, d in zip(frequencies, duty_cycles):
                     data.append(CtrFreq(freq=f, duty_cycle=d))
 
             elif meas_type == UsageTypeCI.PULSE_TIME:
                 high_times = numpy.zeros(array_shape, dtype=numpy.float64)
                 low_times = numpy.zeros(array_shape, dtype=numpy.float64)
 
-                samples_read = _read_ctr_time(
-                    self._handle, high_times, low_times,
-                    number_of_samples_per_channel, timeout)
+                _, _, samples_read = self._interpreter.read_ctr_time(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, high_times, low_times)
                 data = []
                 for h, l in zip(high_times, low_times):
                     data.append(CtrTime(high_time=h, low_time=l))
 
             elif meas_type == UsageTypeCI.PULSE_TICKS:
                 high_ticks = numpy.zeros(array_shape, dtype=numpy.uint32)
                 low_ticks = numpy.zeros(array_shape, dtype=numpy.uint32)
 
-                samples_read = _read_ctr_ticks(
-                    self._handle, high_ticks, low_ticks,
-                    number_of_samples_per_channel, timeout)
+                _, _ , samples_read = self._interpreter.read_ctr_ticks(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, high_ticks, low_ticks)
                 data = []
                 for h, l in zip(high_ticks, low_ticks):
                     data.append(CtrTick(high_tick=h, low_tick=l))
 
             elif meas_type == UsageTypeCI.COUNT_EDGES:
                 data = numpy.zeros(array_shape, dtype=numpy.uint32)
 
-                samples_read = _read_counter_u_32_ex(
-                    self._handle, data, number_of_samples_per_channel, timeout)
+                _, samples_read = self._interpreter.read_counter_u32_ex(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, data)
 
             else:
                 data = numpy.zeros(array_shape, dtype=numpy.float64)
 
-                samples_read = _read_counter_f_64_ex(
-                    self._handle, data, number_of_samples_per_channel, timeout)
+                _, samples_read = self._interpreter.read_counter_f64_ex(
+                    self._handle, number_of_samples_per_channel, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, data)
         else:
             raise DaqError(
                 'Read failed, because there are no channels in this task from '
                 'which data can be read.',
                 DAQmxErrors.READ_NO_INPUT_CHANS_IN_TASK,
                 task_name=self.name)
 
@@ -784,37 +671,27 @@
                 If the status value is positive, it indicates a warning. The
                 callbackData parameter contains the value you passed in the
                 callbackData parameter of this function.
 
                 Passing None for this parameter unregisters the event callback
                 function.
         """
-        DAQmxDoneEventCallbackPtr = ctypes.CFUNCTYPE(
-            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int32,
-            ctypes.c_void_p)
-
-        cfunc = lib_importer.windll.DAQmxRegisterDoneEvent
-
-        with cfunc.arglock:
-            if callback_method is not None:
-                callback_method_ptr = DAQmxDoneEventCallbackPtr(callback_method)
-                self._done_event_callbacks.append(callback_method_ptr)
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_uint,
-                    DAQmxDoneEventCallbackPtr, ctypes.c_void_p]
-            else:
-                del self._done_event_callbacks[:]
-                callback_method_ptr = None
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_uint, ctypes.c_void_p,
-                    ctypes.c_void_p]
-
-            error_code = cfunc(
-                self._handle, 0, callback_method_ptr, None)
-        check_for_error(error_code)
+        if callback_method is not None:
+            # If the event is already registered, the interpreter should raise DaqError with code
+            # DAQmxErrors.DONE_EVENT_ALREADY_REGISTERED.
+            event_handler = self._interpreter.register_done_event(self._handle, 0, callback_method, None)
+            with self._event_handler_lock:
+                assert _TaskEventType.DONE not in self._event_handlers, "Event already registered."
+                self._event_handlers[_TaskEventType.DONE] = event_handler
+        else:
+            self._interpreter.unregister_done_event(self._handle)
+            with self._event_handler_lock:
+                event_handler = self._event_handlers.pop(_TaskEventType.DONE, None)
+            if event_handler is not None:
+                event_handler.close()  # may raise an exception
 
     def register_every_n_samples_acquired_into_buffer_event(
             self, sample_interval, callback_method):
         """
         Registers a callback function to receive an event when the specified
         number of samples is written from the device to the buffer. This
         function only works with devices that support buffered tasks.
@@ -842,41 +719,30 @@
                 the sample_interval parameter of this function. The
                 callback_data parameter contains the value you passed in the
                 callback_data parameter of this function.
 
                 Passing None for this parameter unregisters the event callback
                 function.
         """
-        DAQmxEveryNSamplesEventCallbackPtr = ctypes.CFUNCTYPE(
-            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int32,
-            ctypes.c_uint32, ctypes.c_void_p)
-
-        cfunc = lib_importer.windll.DAQmxRegisterEveryNSamplesEvent
-
-        with cfunc.arglock:
-            if callback_method is not None:
-                callback_method_ptr = DAQmxEveryNSamplesEventCallbackPtr(
-                    callback_method)
-                self._every_n_acquired_event_callbacks.append(
-                    callback_method_ptr)
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    ctypes.c_uint, DAQmxEveryNSamplesEventCallbackPtr,
-                    ctypes.c_void_p]
-            else:
-                del self._every_n_acquired_event_callbacks[:]
-                callback_method_ptr = None
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    ctypes.c_uint, ctypes.c_void_p, ctypes.c_void_p]
-
-            error_code = cfunc(
+        if callback_method is not None:
+            # If the event is already registered, the interpreter should raise DaqError with code
+            # DAQmxErrors.EVERY_N_SAMPS_ACQ_INTO_BUFFER_EVENT_ALREADY_REGISTERED.
+            event_handler = self._interpreter.register_every_n_samples_event(
                 self._handle, EveryNSamplesEventType.ACQUIRED_INTO_BUFFER.value,
-                sample_interval, 0, callback_method_ptr, None)
-        check_for_error(error_code)
+                sample_interval, 0, callback_method, None)
+            with self._event_handler_lock:
+                assert _TaskEventType.EVERY_N_SAMPLES_ACQUIRED_INTO_BUFFER not in self._event_handlers, "Event already registered."
+                self._event_handlers[_TaskEventType.EVERY_N_SAMPLES_ACQUIRED_INTO_BUFFER] = event_handler
+        else:
+            self._interpreter.unregister_every_n_samples_event(
+                self._handle, EveryNSamplesEventType.ACQUIRED_INTO_BUFFER.value)
+            with self._event_handler_lock:
+                event_handler = self._event_handlers.pop(_TaskEventType.EVERY_N_SAMPLES_ACQUIRED_INTO_BUFFER, None)
+            if event_handler is not None:
+                event_handler.close()  # may raise an exception
 
     def register_every_n_samples_transferred_from_buffer_event(
             self, sample_interval, callback_method):
         """
         Registers a callback function to receive an event when the specified
         number of samples is written from the buffer to the device. This
         function only works with devices that support buffered tasks.
@@ -904,42 +770,30 @@
                 the sample_interval parameter of this function. The
                 callback_data parameter contains the value you passed in the
                 callback_data parameter of this function.
 
                 Passing None for this parameter unregisters the event callback
                 function.
         """
-        DAQmxEveryNSamplesEventCallbackPtr = ctypes.CFUNCTYPE(
-            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int32,
-            ctypes.c_uint32, ctypes.c_void_p)
-
-        cfunc = lib_importer.windll.DAQmxRegisterEveryNSamplesEvent
-
-        with cfunc.arglock:
-            if callback_method is not None:
-                callback_method_ptr = DAQmxEveryNSamplesEventCallbackPtr(
-                    callback_method)
-                self._every_n_transferred_event_callbacks.append(
-                    callback_method_ptr)
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    ctypes.c_uint, DAQmxEveryNSamplesEventCallbackPtr,
-                    ctypes.c_void_p]
-            else:
-                del self._every_n_transferred_event_callbacks[:]
-                callback_method_ptr = None
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    ctypes.c_uint, ctypes.c_void_p, ctypes.c_void_p]
-
-            error_code = cfunc(
-                self._handle,
-                EveryNSamplesEventType.TRANSFERRED_FROM_BUFFER.value,
-                sample_interval, 0, callback_method_ptr, None)
-        check_for_error(error_code)
+        if callback_method is not None:
+            # If the event is already registered, the interpreter should raise DaqError with code
+            # DAQmxErrors.EVERY_N_SAMPS_TRANSFERRED_FROM_BUFFER_EVENT_ALREADY_REGISTERED.
+            event_handler = self._interpreter.register_every_n_samples_event(
+                self._handle, EveryNSamplesEventType.TRANSFERRED_FROM_BUFFER.value,
+                sample_interval, 0, callback_method, None)
+            with self._event_handler_lock:
+                assert _TaskEventType.EVERY_N_SAMPLES_TRANSFERRED_FROM_BUFFER not in self._event_handlers, "Event already registered."
+                self._event_handlers[_TaskEventType.EVERY_N_SAMPLES_TRANSFERRED_FROM_BUFFER] = event_handler
+        else:
+            self._interpreter.unregister_every_n_samples_event(
+                self._handle, EveryNSamplesEventType.TRANSFERRED_FROM_BUFFER.value)
+            with self._event_handler_lock:
+                event_handler = self._event_handlers.pop(_TaskEventType.EVERY_N_SAMPLES_TRANSFERRED_FROM_BUFFER, None)
+            if event_handler is not None:
+                event_handler.close()  # may raise an exception
 
     def register_signal_event(self, signal_type, callback_method):
         """
         Registers a callback function to receive an event when the specified
         hardware event occurs.
 
         When you stop a task explicitly any pending events are discarded. For
@@ -962,38 +816,28 @@
                 the signal_type parameter of this function. The callback_data
                 parameter contains the value you passed in the callback_data
                 parameter of this function.
 
                 Passing None for this parameter unregisters the event callback
                 function.
         """
-        DAQmxSignalEventCallbackPtr = ctypes.CFUNCTYPE(
-            ctypes.c_int32, lib_importer.task_handle, ctypes.c_int32,
-            ctypes.c_void_p)
-
-        cfunc = lib_importer.windll.DAQmxRegisterSignalEvent
-
-        with cfunc.arglock:
-            if callback_method is not None:
-                callback_method_ptr = DAQmxSignalEventCallbackPtr(
-                    callback_method)
-                self._signal_event_callbacks.append(callback_method_ptr)
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    DAQmxSignalEventCallbackPtr, ctypes.c_void_p]
-            else:
-                del self._signal_event_callbacks[:]
-                callback_method_ptr = None
-                cfunc.argtypes = [
-                    lib_importer.task_handle, ctypes.c_int, ctypes.c_uint,
-                    ctypes.c_void_p, ctypes.c_void_p]
-
-            error_code = cfunc(
-                self._handle, signal_type.value, 0, callback_method_ptr, None)
-        check_for_error(error_code)
+        if callback_method is not None:
+            # If the event is already registered, the interpreter should raise DaqError with code
+            # DAQmxErrors.SIGNAL_EVENT_ALREADY_REGISTERED.
+            event_handler = self._interpreter.register_signal_event(
+                self._handle, signal_type.value, 0, callback_method, None)
+            with self._event_handler_lock:
+                assert _TaskEventType.SIGNAL not in self._event_handlers, "Event already registered."
+                self._event_handlers[_TaskEventType.SIGNAL] = event_handler
+        else:
+            self._interpreter.unregister_signal_event(self._handle, signal_type.value)
+            with self._event_handler_lock:
+                event_handler = self._event_handlers.pop(_TaskEventType.SIGNAL, None)
+            if event_handler is not None:
+                event_handler.close()  # may raise an exception
 
     def save(self, save_as="", author="", overwrite_existing_task=False,
              allow_interactive_editing=True, allow_interactive_deletion=True):
         """
         Saves this task and any local channels it contains to MAX.
 
         This function does not save global channels. Use the DAQmx Save
@@ -1024,25 +868,15 @@
         if overwrite_existing_task:
             options |= _Save.OVERWRITE.value
         if allow_interactive_editing:
             options |= _Save.ALLOW_INTERACTIVE_EDITING.value
         if allow_interactive_deletion:
             options |= _Save.ALLOW_INTERACTIVE_DELETION.value
 
-        cfunc = lib_importer.windll.DAQmxSaveTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [
-                        lib_importer.task_handle, ctypes_byte_str,
-                        ctypes_byte_str, ctypes.c_uint]
-
-        error_code = cfunc(
-            self._handle, save_as, author, options)
-        check_for_error(error_code)
+        self._interpreter.save_task(self._handle, save_as, author, options)
 
     def start(self):
         """
         Transitions the task to the running state to begin the measurement
         or generation. Using this method is required for some applications and
         is optional for others.
 
@@ -1053,43 +887,29 @@
 
         If you do not use the DAQmx Start Task method and the DAQmx Stop Task
         method when you use the DAQmx Read method or the DAQmx Write method
         multiple times, such as in a loop, the task starts and stops
         repeatedly. Starting and stopping a task repeatedly reduces the
         performance of the application.
         """
-        cfunc = lib_importer.windll.DAQmxStartTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [lib_importer.task_handle]
-
-        error_code = cfunc(self._handle)
-        check_for_error(error_code)
+        self._interpreter.start_task(self._handle)
 
     def stop(self):
         """
         Stops the task and returns it to the state the task was in before the
         DAQmx Start Task method ran or the DAQmx Write method ran with the
         autostart input set to TRUE.
 
         If you do not use the DAQmx Start Task method and the DAQmx Stop Task
         method when you use the DAQmx Read method or the DAQmx Write method
         multiple times, such as in a loop, the task starts and stops
         repeatedly. Starting and stopping a task repeatedly reduces the
         performance of the application.
         """
-        cfunc = lib_importer.windll.DAQmxStopTask
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [lib_importer.task_handle]
-
-        error_code = cfunc(self._handle)
-        check_for_error(error_code)
+        self._interpreter.stop_task(self._handle)
 
     def wait_until_done(self, timeout=10.0):
         """
         Waits for the measurement or generation to complete.
 
         Use this method to ensure that the specified operation is complete
         before you stop the task.
@@ -1099,22 +919,15 @@
                 seconds to wait for the measurement or generation to complete.
                 This method returns an error if the time elapses. The
                 default is 10. If you set timeout (sec) to
                 nidaqmx.WAIT_INFINITELY, the method waits indefinitely. If you
                 set timeout (sec) to 0, the method checks once and returns
                 an error if the measurement or generation is not done.
         """
-        cfunc = lib_importer.windll.DAQmxWaitUntilTaskDone
-        if cfunc.argtypes is None:
-            with cfunc.arglock:
-                if cfunc.argtypes is None:
-                    cfunc.argtypes = [lib_importer.task_handle, ctypes.c_double]
-
-        error_code = cfunc(self._handle, timeout)
-        check_for_error(error_code)
+        self._interpreter.wait_until_task_done(self._handle, timeout)
 
     def _raise_invalid_num_lines_error(
             self, num_lines_expected, num_lines_in_data):
         raise DaqError(
             'Specified read or write operation failed, because the number '
             'of lines in the data for a channel does not match the number '
             'of lines in the channel.\n\n'
@@ -1143,31 +956,31 @@
 
     def write(self, data, auto_start=AUTO_START_UNSET, timeout=10.0):
         """
         Writes samples to the task or virtual channels you specify.
 
         This write method is dynamic, and is capable of accepting the
         samples to write in the various forms for most operations:
-        
+
         - Scalar: Single sample for 1 channel.
         - List/1D numpy.ndarray: Multiple samples for 1 channel or 1
           sample for multiple channels.
         - List of lists/2D numpy.ndarray: Multiple samples for multiple
           channels.
 
         The data type of the samples passed in must be appropriate for
         the channel type of the task.
 
         For counter output pulse operations, this write method only
         accepts samples in these forms:
-        
-        - Scalar CtrFreq, CtrTime, CtrTick (from nidaqmx.types): 
+
+        - Scalar CtrFreq, CtrTime, CtrTick (from nidaqmx.types):
           Single sample for 1 channel.
         - List of CtrFreq, CtrTime, CtrTick (from nidaqmx.types):
-          Multiple samples for 1 channel or 1 sample for multiple 
+          Multiple samples for 1 channel or 1 sample for multiple
           channels.
 
         If the task uses on-demand timing, this method returns only
         after the device generates all samples. On-demand is the default
         timing type if you do not use the timing property on the task to
         configure a sample timing type. If the task uses any timing type
         other than on-demand, this method returns immediately and does
@@ -1264,53 +1077,50 @@
 
         if auto_start is AUTO_START_UNSET:
             if number_of_samples_per_channel > 1:
                 auto_start = False
             else:
                 auto_start = True
 
-        # Analog Input
         if write_chan_type == ChannelType.ANALOG_OUTPUT:
             data = numpy.asarray(data, dtype=numpy.float64)
-            return _write_analog_f_64(
-                self._handle, data, number_of_samples_per_channel, auto_start,
-                timeout)
+            return self._interpreter.write_analog_f64(
+                self._handle, number_of_samples_per_channel, auto_start,
+                timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
-        # Digital Input
         elif write_chan_type == ChannelType.DIGITAL_OUTPUT:
             if self.out_stream.do_num_booleans_per_chan == 1:
                 if (not isinstance(element, bool) and
                         not isinstance(element, numpy.bool_)):
                     raise DaqError(
                         'Write failed, because this write method only accepts '
                         'boolean samples when there is one digital line per '
                         'channel in a task.\n\n'
                         'Requested sample type: {}'.format(type(element)),
                         DAQmxErrors.UNKNOWN, task_name=self.name)
 
                 data = numpy.asarray(data, dtype=bool)
-                return _write_digital_lines(
-                    self._handle, data, number_of_samples_per_channel,
-                    auto_start, timeout)
+                return self._interpreter.write_digital_lines(
+                    self._handle, number_of_samples_per_channel,
+                    auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
             else:
                 if (not isinstance(element, int) and
                         not isinstance(element, numpy.uint32)):
                     raise DaqError(
                         'Write failed, because this write method only accepts '
                         'unsigned 32-bit integer samples when there are '
                         'multiple digital lines per channel in a task.\n\n'
                         'Requested sample type: {}'.format(type(element)),
                         DAQmxErrors.UNKNOWN, task_name=self.name)
 
                 data = numpy.asarray(data, dtype=numpy.uint32)
-                return _write_digital_u_32(
-                    self._handle, data, number_of_samples_per_channel,
-                    auto_start, timeout)
+                return self._interpreter.write_digital_u32(
+                    self._handle, number_of_samples_per_channel,
+                    auto_start, timeout, FillMode.GROUP_BY_CHANNEL.value, data)
 
-        # Counter Input
         elif write_chan_type == ChannelType.COUNTER_OUTPUT:
             output_type = channels_to_write.co_output_type
 
             if number_of_samples_per_channel == 1:
                 data = [data]
 
             if output_type == UsageTypeCO.PULSE_FREQUENCY:
@@ -1319,44 +1129,85 @@
                 for sample in data:
                     frequencies.append(sample.freq)
                     duty_cycles.append(sample.duty_cycle)
 
                 frequencies = numpy.asarray(frequencies, dtype=numpy.float64)
                 duty_cycles = numpy.asarray(duty_cycles, dtype=numpy.float64)
 
-                return _write_ctr_freq(
-                    self._handle, frequencies, duty_cycles,
-                    number_of_samples_per_channel, auto_start, timeout)
+                return self._interpreter.write_ctr_freq(
+                    self._handle, number_of_samples_per_channel, auto_start, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, frequencies, duty_cycles)
 
             elif output_type == UsageTypeCO.PULSE_TIME:
                 high_times = []
                 low_times = []
                 for sample in data:
                     high_times.append(sample.high_time)
                     low_times.append(sample.low_time)
 
                 high_times = numpy.asarray(high_times, dtype=numpy.float64)
                 low_times = numpy.asarray(low_times, dtype=numpy.float64)
 
-                return _write_ctr_time(
-                    self._handle, high_times, low_times,
-                    number_of_samples_per_channel, auto_start, timeout)
+                return self._interpreter.write_ctr_time(
+                    self._handle, number_of_samples_per_channel, auto_start, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, high_times, low_times)
 
             elif output_type == UsageTypeCO.PULSE_TICKS:
                 high_ticks = []
                 low_ticks = []
                 for sample in data:
                     high_ticks.append(sample.high_tick)
                     low_ticks.append(sample.low_tick)
 
                 high_ticks = numpy.asarray(high_ticks, dtype=numpy.uint32)
                 low_ticks = numpy.asarray(low_ticks, dtype=numpy.uint32)
 
-                return _write_ctr_ticks(
-                    self._handle, high_ticks, low_ticks,
-                    number_of_samples_per_channel, auto_start, timeout)
+                return self._interpreter.write_ctr_ticks(
+                    self._handle, number_of_samples_per_channel, auto_start, timeout,
+                    FillMode.GROUP_BY_CHANNEL.value, high_ticks, low_ticks)
         else:
             raise DaqError(
                 'Write failed, because there are no output channels in this '
                 'task to which data can be written.',
                 DAQmxErrors.WRITE_NO_OUTPUT_CHANS_IN_TASK,
                 task_name=self.name)
+
+
+class _TaskAlternateConstructor(Task):
+    """
+    Provide an alternate constructor for the Task object.
+
+    This is a private API used to instantiate a Task with an existing task handle and interpreter.
+    """
+    # Setting __slots__ avoids TypeError: __class__ assignment: 'Base' object layout differs from 'Derived'.
+    __slots__ = ()
+
+    def __init__(self, task_handle, interpreter, close_on_exit):
+        """
+        Args:
+            task_handle: Specifies the task handle from which to create a
+                Task object.
+            interpreter: Specifies the interpreter instance.
+            close_on_exit: Specifies whether the task's context manager closes the task.
+
+        """
+        # Initialize the fields that __del__ accesses so it doesn't crash when _initialize raises an exception.
+        self._handle = task_handle
+        self._close_on_exit = close_on_exit
+        self._saved_name = ""  # _initialize sets this to the name assigned by DAQmx.
+        self._grpc_options = getattr(interpreter, "_grpc_options", None)
+        self._event_handlers = {}
+
+        self._interpreter = interpreter
+        self._initialize(self._handle, self._interpreter)
+
+        # Use meta-programming to change the type of this object to Task,
+        # so the user isn't confused when doing introspection.
+        self.__class__ = Task
+
+
+class _TaskEventType(Enum):
+    """Internal enum for task event bookkeeping."""
+    DONE = 1
+    EVERY_N_SAMPLES_ACQUIRED_INTO_BUFFER = 2
+    EVERY_N_SAMPLES_TRANSFERRED_FROM_BUFFER = 3
+    SIGNAL = 4
```

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/types.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/types.py`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/generated/nidaqmx/utils.py` & `nidaqmx-0.8.0.dev0/generated/nidaqmx/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import re
+from typing import Optional
 
 from nidaqmx.errors import DaqError
+from nidaqmx.grpc_session_options import GrpcSessionOptions
+from nidaqmx._base_interpreter import BaseInterpreter
+
 
 # Method logic adapted from
 # //Measurements/Infrastructure/dmxf/trunk/2.5/source/nimuck/parseUtilities.cpp
 
 _invalid_range_syntax_message = (
     "Syntax for a range of objects in the input string is invalid.\n\n"
     "For ranges of objects, specify a number immediately before and after "
@@ -200,7 +204,22 @@
 
             if num_after < num_before:
                 colon_expanded_channel.reverse()
 
             channel_list_to_return.extend(colon_expanded_channel)
 
     return channel_list_to_return
+
+
+def _select_interpreter(
+    grpc_options: Optional[GrpcSessionOptions] = None,
+    interpreter: Optional[BaseInterpreter] = None
+) -> BaseInterpreter:
+    if interpreter:
+        return interpreter
+    else:
+        if grpc_options:
+            from nidaqmx._grpc_interpreter import GrpcStubInterpreter
+            return GrpcStubInterpreter(grpc_options)
+        else:
+            from nidaqmx._library_interpreter import LibraryInterpreter
+            return LibraryInterpreter()
```

### Comparing `nidaqmx-0.7.0/LICENSE` & `nidaqmx-0.8.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/README.rst` & `nidaqmx-0.8.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `nidaqmx-0.7.0/PKG-INFO` & `nidaqmx-0.8.0.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nidaqmx
-Version: 0.7.0
+Version: 0.8.0.dev0
 Summary: NI-DAQmx Python API
 Home-page: https://github.com/ni/nidaqmx-python
 License: MIT
 Keywords: nidaqmx,nidaq,daqmx,daq
 Author: NI
 Author-email: opensource@ni.com
 Maintainer: Zach Hindes
@@ -19,29 +19,27 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: System :: Hardware :: Hardware Drivers
 Provides-Extra: docs
+Provides-Extra: grpc
 Requires-Dist: Sphinx (>=4.3,<5.0) ; extra == "docs"
 Requires-Dist: deprecation (>=2.1)
+Requires-Dist: grpcio (>=1.49.0,<1.53) ; (python_version < "3.8") and (extra == "grpc")
+Requires-Dist: grpcio (>=1.49.0,<2.0) ; (python_version >= "3.8" and python_version < "4.0") and (extra == "grpc")
 Requires-Dist: importlib_metadata (>=4.2,<5.0) ; python_version >= "3.7" and python_version < "3.8"
 Requires-Dist: numpy (>=1.20,<1.22) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.22) ; python_version >= "3.8" and python_version < "4.0"
+Requires-Dist: protobuf (>=4.21,<5.0) ; extra == "grpc"
 Requires-Dist: sphinx_rtd_theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Documentation, https://nidaqmx-python.readthedocs.io
 Project-URL: Repository, https://github.com/ni/nidaqmx-python
 Description-Content-Type: text/x-rst
 
 ===========  =================================================================================================================================
 Info         Contains a Python API for interacting with NI-DAQmx. See `GitHub <https://github.com/ni/nidaqmx-python/>`_ for the latest source.
```

