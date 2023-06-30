# Comparing `tmp/zaber_motion-4.2.0.tar.gz` & `tmp/zaber_motion-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-4.2.0.tar", last modified: Sat Jun 17 02:49:41 2023, max compression
+gzip compressed data, was "zaber_motion-4.2.1.tar", last modified: Fri Jun 30 01:40:15 2023, max compression
```

## Comparing `zaber_motion-4.2.0.tar` & `zaber_motion-4.2.1.tar`

### file list

```diff
@@ -1,189 +1,194 @@
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481835 zaber_motion-4.2.0/
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/DESCRIPTION.md
--rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/LICENSE.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/MANIFEST.in
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-17 02:49:41.481904 zaber_motion-4.2.0/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/README.md
--rw-r--r--   0 zaber      (501) staff       (20)      134 2023-06-17 02:49:41.482156 zaber_motion-4.2.0/setup.cfg
--rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/setup.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.458952 zaber_motion-4.2.0/test/
--rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/test/test_integration.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.460904 zaber_motion-4.2.0/zaber_motion/
--rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/__init__.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.467797 zaber_motion-4.2.0/zaber_motion/ascii/
--rw-r--r--   0 zaber      (501) staff       (20)     2742 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/alert_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/all_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)    41645 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis.py
--rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      272 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_axis_response.py
--rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_device_response.py
--rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/conversion_factor.py
--rw-r--r--   0 zaber      (501) staff       (20)    24838 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_io.py
--rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_io_info.py
--rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/io_port_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/lockstep.py
--rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/lockstep_axes.py
--rw-r--r--   0 zaber      (501) staff       (20)      386 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/message_type.py
--rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope.py
--rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py
--rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      268 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data_source.py
--rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/paramset_info.py
--rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pid_tuning.py
--rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      256 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      247 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/pvt_sequence.py
--rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/response.py
--rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuner.py
--rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_param.py
--rw-r--r--   0 zaber      (501) staff       (20)      384 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_paramset.py
--rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/setting_constants.py
--rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/simple_tuning_param_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/storage.py
--rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream.py
--rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)      253 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_buffer.py
--rw-r--r--   0 zaber      (501) staff       (20)      273 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/stream_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/transport.py
--rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/warning_flags.py
--rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/ascii/warnings.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.469576 zaber_motion-4.2.0/zaber_motion/binary/
--rw-r--r--   0 zaber      (501) staff       (20)      653 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/binary_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/command_code.py
--rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/connection.py
--rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device.py
--rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_identity.py
--rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_settings.py
--rw-r--r--   0 zaber      (501) staff       (20)      276 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/device_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/error_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/message.py
--rw-r--r--   0 zaber      (501) staff       (20)      415 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/reply_code.py
--rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/reply_only_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/binary/unknown_response_event.py
--rw-r--r--   0 zaber      (501) staff       (20)     1153 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/bindings.py
--rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/call.py
--rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/convert_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      257 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/device_db_source_type.py
--rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/events.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.479734 zaber_motion-4.2.0/zaber_motion/exceptions/
--rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      991 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_preempted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      304 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/connection_closed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/connection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/conversion_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      314 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      911 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      283 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_detection_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/device_not_identified_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      309 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/internal_error_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      295 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_argument_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_data_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      310 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_operation_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_park_state_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_pvt_point.py
--rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      928 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      342 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/io_channel_out_of_range_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/io_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      322 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/lockstep_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      329 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/lockstep_not_enabled_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      396 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/motion_lib_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/no_device_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/no_value_for_key_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/not_supported_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/os_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/out_of_request_ids_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      326 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      285 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/pvt_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/request_timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      349 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/serial_port_busy_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/setting_not_found_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_discontinuity_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_mode_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
--rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/stream_setup_failed_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      341 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/timeout_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/transport_already_used_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/exceptions/unknown_request_exception.py
--rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/firmware_version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.480984 zaber_motion-4.2.0/zaber_motion/gcode/
--rw-r--r--   0 zaber      (501) staff       (20)      578 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_mapping.py
--rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/axis_transformation.py
--rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/device_definition.py
--rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/offline_translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translate_message.py
--rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translate_result.py
--rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translator.py
--rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/gcode/translator_config.py
--rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/library.py
--rw-r--r--   0 zaber      (501) staff       (20)      279 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/log_output_mode.py
--rw-r--r--   0 zaber      (501) staff       (20)     1631 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/measurement.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481223 zaber_motion-4.2.0/zaber_motion/microscopy/
--rw-r--r--   0 zaber      (501) staff       (20)       68 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/microscopy/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/microscopy/objective_changer.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.481603 zaber_motion-4.2.0/zaber_motion/protobufs/
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/__init__.py
--rw-r--r--   0 zaber      (501) staff       (20)    66434 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.py
--rw-r--r--   0 zaber      (501) staff       (20)   202637 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.pyi
--rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/py.typed
--rw-r--r--   0 zaber      (501) staff       (20)      278 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/rotation_direction.py
--rw-r--r--   0 zaber      (501) staff       (20)      987 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/serialization.py
--rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/tools.py
--rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/units.py
--rw-r--r--   0 zaber      (501) staff       (20)       22 2023-06-17 02:48:51.000000 zaber_motion-4.2.0/zaber_motion/version.py
-drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-17 02:49:41.461476 zaber_motion-4.2.0/zaber_motion.egg-info/
--rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/PKG-INFO
--rw-r--r--   0 zaber      (501) staff       (20)     7670 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/SOURCES.txt
--rw-r--r--   0 zaber      (501) staff       (20)        1 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/dependency_links.txt
--rw-r--r--   0 zaber      (501) staff       (20)      239 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/requires.txt
--rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-17 02:49:41.000000 zaber_motion-4.2.0/zaber_motion.egg-info/top_level.txt
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.030592 zaber_motion-4.2.1/
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/DESCRIPTION.md
+-rw-r--r--   0 zaber      (501) staff       (20)   109244 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/LICENSE.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/MANIFEST.in
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-30 01:40:15.030657 zaber_motion-4.2.1/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)      218 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/README.md
+-rw-r--r--   0 zaber      (501) staff       (20)      134 2023-06-30 01:40:15.030914 zaber_motion-4.2.1/setup.cfg
+-rw-r--r--   0 zaber      (501) staff       (20)     1371 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/setup.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:14.998294 zaber_motion-4.2.1/test/
+-rw-r--r--   0 zaber      (501) staff       (20)     3544 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/test/test_integration.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.001630 zaber_motion-4.2.1/zaber_motion/
+-rw-r--r--   0 zaber      (501) staff       (20)     6583 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/__init__.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.012700 zaber_motion-4.2.1/zaber_motion/ascii/
+-rw-r--r--   0 zaber      (501) staff       (20)     3136 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2185 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/alert_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     8708 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/all_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)    41649 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/axis.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2259 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/axis_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12952 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/axis_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      272 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1265 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/can_set_state_axis_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1530 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/can_set_state_device_response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    36081 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1959 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/conversion_factor.py
+-rw-r--r--   0 zaber      (501) staff       (20)    24816 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2801 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17751 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/device_io.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2077 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/device_io_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12120 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/io_port_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    37243 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/lockstep.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1671 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/lockstep_axes.py
+-rw-r--r--   0 zaber      (501) staff       (20)      386 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/message_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)    17493 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2423 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5695 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      268 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope_data_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1601 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/paramset_info.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2078 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pid_tuning.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22773 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/process.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3830 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/process_controller.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/process_controller_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2074 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/process_controller_source.py
+-rw-r--r--   0 zaber      (501) staff       (20)      281 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/process_controller_source_sensor.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2071 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pvt_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      256 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pvt_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3190 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pvt_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      247 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pvt_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)    33707 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/pvt_sequence.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2896 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/response.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19220 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/servo_tuner.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1782 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/servo_tuning_param.py
+-rw-r--r--   0 zaber      (501) staff       (20)      384 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/servo_tuning_paramset.py
+-rw-r--r--   0 zaber      (501) staff       (20)    22658 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/setting_constants.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1893 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/simple_tuning_param_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    26082 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/storage.py
+-rw-r--r--   0 zaber      (501) staff       (20)    85042 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/stream.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2110 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/stream_axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)      253 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/stream_axis_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3084 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/stream_buffer.py
+-rw-r--r--   0 zaber      (501) staff       (20)      273 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/stream_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5345 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/transport.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2966 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2855 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/warning_flags.py
+-rw-r--r--   0 zaber      (501) staff       (20)     5066 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/ascii/warnings.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.014966 zaber_motion-4.2.1/zaber_motion/binary/
+-rw-r--r--   0 zaber      (501) staff       (20)      653 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1941 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/binary_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3132 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/command_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)    19348 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/connection.py
+-rw-r--r--   0 zaber      (501) staff       (20)    29083 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/device.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3361 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/device_identity.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3513 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/device_settings.py
+-rw-r--r--   0 zaber      (501) staff       (20)      276 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/device_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3116 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/error_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1498 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/message.py
+-rw-r--r--   0 zaber      (501) staff       (20)      415 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/reply_code.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1552 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/reply_only_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1588 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/binary/unknown_response_event.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1535 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/bindings.py
+-rw-r--r--   0 zaber      (501) staff       (20)     4196 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/call.py
+-rw-r--r--   0 zaber      (501) staff       (20)     7349 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/convert_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      257 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/device_db_source_type.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2200 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/events.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.027986 zaber_motion-4.2.1/zaber_motion/exceptions/
+-rw-r--r--   0 zaber      (501) staff       (20)     7384 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1121 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/binary_command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      991 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1045 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/command_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3097 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/command_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/command_preempted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1129 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/command_too_long_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1971 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/command_too_long_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      304 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/connection_closed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/connection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/conversion_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1158 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_address_conflict_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1126 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      314 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1092 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_db_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      911 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      283 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_detection_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/device_not_identified_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1065 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/g_code_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1321 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1036 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/g_code_syntax_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1300 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      309 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/internal_error_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      295 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_argument_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_data_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      310 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_operation_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1058 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_packet_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1198 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_park_state_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1140 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_pvt_point.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1091 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_response_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      928 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/invalid_response_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      342 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/io_channel_out_of_range_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/io_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      322 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/lockstep_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      329 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/lockstep_not_enabled_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      396 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/motion_lib_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1070 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1852 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1137 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1875 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      292 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/no_device_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      297 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/no_value_for_key_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      308 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/not_supported_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/os_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      317 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/out_of_request_ids_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1037 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1749 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      326 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1102 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1292 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1169 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1327 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      285 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/pvt_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      300 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/request_timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      349 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/serial_port_busy_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     3563 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/set_device_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1085 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2372 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1120 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      307 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/setting_not_found_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_discontinuity_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1060 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_execution_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1232 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_execution_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      323 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_mode_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1134 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1313 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1199 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1348 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py
+-rw-r--r--   0 zaber      (501) staff       (20)      282 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/stream_setup_failed_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      341 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/timeout_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      320 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/transport_already_used_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)      335 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/exceptions/unknown_request_exception.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2088 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/firmware_version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.029607 zaber_motion-4.2.1/zaber_motion/gcode/
+-rw-r--r--   0 zaber      (501) staff       (20)      578 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2242 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/axis_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1547 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/axis_mapping.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2139 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/axis_transformation.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2290 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/device_definition.py
+-rw-r--r--   0 zaber      (501) staff       (20)    12481 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/offline_translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1555 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/translate_message.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1401 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/translate_result.py
+-rw-r--r--   0 zaber      (501) staff       (20)    13105 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/translator.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2206 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/gcode/translator_config.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2838 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/library.py
+-rw-r--r--   0 zaber      (501) staff       (20)      279 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/log_output_mode.py
+-rw-r--r--   0 zaber      (501) staff       (20)     1937 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/measurement.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.029923 zaber_motion-4.2.1/zaber_motion/microscopy/
+-rw-r--r--   0 zaber      (501) staff       (20)       68 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/microscopy/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)     6181 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/microscopy/objective_changer.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.030360 zaber_motion-4.2.1/zaber_motion/protobufs/
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/protobufs/__init__.py
+-rw-r--r--   0 zaber      (501) staff       (20)    67598 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/protobufs/main_pb2.py
+-rw-r--r--   0 zaber      (501) staff       (20)   206262 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/protobufs/main_pb2.pyi
+-rw-r--r--   0 zaber      (501) staff       (20)        0 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/py.typed
+-rw-r--r--   0 zaber      (501) staff       (20)      278 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/rotation_direction.py
+-rw-r--r--   0 zaber      (501) staff       (20)      987 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/serialization.py
+-rw-r--r--   0 zaber      (501) staff       (20)     2108 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/tools.py
+-rw-r--r--   0 zaber      (501) staff       (20)     9021 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/units.py
+-rw-r--r--   0 zaber      (501) staff       (20)       22 2023-06-30 01:39:25.000000 zaber_motion-4.2.1/zaber_motion/version.py
+drwxr-xr-x   0 zaber      (501) staff       (20)        0 2023-06-30 01:40:15.002422 zaber_motion-4.2.1/zaber_motion.egg-info/
+-rw-r--r--   0 zaber      (501) staff       (20)      808 2023-06-30 01:40:14.000000 zaber_motion-4.2.1/zaber_motion.egg-info/PKG-INFO
+-rw-r--r--   0 zaber      (501) staff       (20)     7890 2023-06-30 01:40:14.000000 zaber_motion-4.2.1/zaber_motion.egg-info/SOURCES.txt
+-rw-r--r--   0 zaber      (501) staff       (20)        1 2023-06-30 01:40:14.000000 zaber_motion-4.2.1/zaber_motion.egg-info/dependency_links.txt
+-rw-r--r--   0 zaber      (501) staff       (20)      239 2023-06-30 01:40:14.000000 zaber_motion-4.2.1/zaber_motion.egg-info/requires.txt
+-rw-r--r--   0 zaber      (501) staff       (20)       13 2023-06-30 01:40:14.000000 zaber_motion-4.2.1/zaber_motion.egg-info/top_level.txt
```

### Comparing `zaber_motion-4.2.0/LICENSE.txt` & `zaber_motion-4.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/PKG-INFO` & `zaber_motion-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber_motion
-Version: 4.2.0
+Version: 4.2.1
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.0/setup.py` & `zaber_motion-4.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read_from_file(*filename):
     with open(path.join(*filename), 'r') as f:
         return f.read()
 
 
 setup(
     name='zaber_motion',
-    version='4.2.0',
+    version='4.2.1',
     packages=find_packages(exclude=["test*", "test_*", "*_test*"]),
     package_data={
         '': ['*.pyi', 'py.typed']
     },
     description='A library for communicating with Zaber devices',
     long_description=read_from_file('DESCRIPTION.md'),
     long_description_content_type="text/markdown",
@@ -32,12 +32,12 @@
         'License :: OSI Approved :: MIT License',
     ],
     keywords='',
     python_requires='>=3.8',
     install_requires=[
         'protobuf>=3.20.0,<4.22.0',
         'rx>=3.0.0',
-        'zaber_motion_bindings_windows==4.2.0;platform_system=="Windows"',
-        'zaber_motion_bindings_linux==4.2.0;platform_system=="Linux"',
-        'zaber_motion_bindings_darwin==4.2.0;platform_system=="Darwin"',
+        'zaber_motion_bindings_windows==4.2.1;platform_system=="Windows"',
+        'zaber_motion_bindings_linux==4.2.1;platform_system=="Linux"',
+        'zaber_motion_bindings_darwin==4.2.1;platform_system=="Darwin"',
     ],
 )
```

### Comparing `zaber_motion-4.2.0/test/test_integration.py` & `zaber_motion-4.2.1/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/__init__.py` & `zaber_motion-4.2.1/zaber_motion/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/__init__.py` & `zaber_motion-4.2.1/zaber_motion/ascii/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,12 +35,17 @@
 from .pid_tuning import PidTuning as PidTuning
 from .servo_tuning_param import ServoTuningParam as ServoTuningParam
 from .simple_tuning_param_definition import SimpleTuningParamDefinition as SimpleTuningParamDefinition
 from .storage import AxisStorage as AxisStorage, DeviceStorage as DeviceStorage
 from .conversion_factor import ConversionFactor as ConversionFactor
 from .can_set_state_axis_response import CanSetStateAxisResponse as CanSetStateAxisResponse
 from .can_set_state_device_response import CanSetStateDeviceResponse as CanSetStateDeviceResponse
+from .process_controller import ProcessController as ProcessController
+from .process import Process as Process
+from .process_controller_source import ProcessControllerSource as ProcessControllerSource
+from .process_controller_source_sensor import ProcessControllerSourceSensor as ProcessControllerSourceSensor
+from .process_controller_mode import ProcessControllerMode as ProcessControllerMode
 from .pvt_sequence import PvtSequence as PvtSequence
 from .pvt_buffer import PvtBuffer as PvtBuffer
 from .pvt_mode import PvtMode as PvtMode
 from .pvt_axis_type import PvtAxisType as PvtAxisType
 from .pvt_axis_definition import PvtAxisDefinition as PvtAxisDefinition
```

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/alert_event.py` & `zaber_motion-4.2.1/zaber_motion/ascii/alert_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/all_axes.py` & `zaber_motion-4.2.1/zaber_motion/ascii/all_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/axis.py` & `zaber_motion-4.2.1/zaber_motion/ascii/axis.py`

 * *Files 0% similar despite different names*

```diff
@@ -994,15 +994,15 @@
         return response.value
 
     def set_state(
             self,
             state: str
     ) -> None:
         """
-        Applies a saved state to an axis.
+        Applies a saved state to this axis.
 
         Args:
             state: The state object to apply to this axis.
         """
         request = main_pb2.SetStateRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
@@ -1011,15 +1011,15 @@
         call("device/set_state", request)
 
     async def set_state_async(
             self,
             state: str
     ) -> None:
         """
-        Applies a saved state to an axis.
+        Applies a saved state to this axis.
 
         Args:
             state: The state object to apply to this axis.
         """
         request = main_pb2.SetStateRequest()
         request.interface_id = self.device.connection.interface_id
         request.device = self.device.device_address
```

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/axis_identity.py` & `zaber_motion-4.2.1/zaber_motion/ascii/axis_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/axis_settings.py` & `zaber_motion-4.2.1/zaber_motion/ascii/axis_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_axis_response.py` & `zaber_motion-4.2.1/zaber_motion/ascii/can_set_state_axis_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/can_set_state_device_response.py` & `zaber_motion-4.2.1/zaber_motion/ascii/can_set_state_device_response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/connection.py` & `zaber_motion-4.2.1/zaber_motion/ascii/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/conversion_factor.py` & `zaber_motion-4.2.1/zaber_motion/ascii/conversion_factor.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/device.py` & `zaber_motion-4.2.1/zaber_motion/ascii/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,18 +565,18 @@
 
     def set_state(
             self,
             state: str,
             device_only: bool = False
     ) -> None:
         """
-        Applies a saved state to an axis.
+        Applies a saved state to this device.
 
         Args:
-            state: The state object to apply to this axis.
+            state: The state object to apply to this device.
             device_only: If true, only device scope settings and features will be set.
         """
         request = main_pb2.SetStateRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.state = state
         request.device_only = device_only
@@ -584,33 +584,33 @@
 
     async def set_state_async(
             self,
             state: str,
             device_only: bool = False
     ) -> None:
         """
-        Applies a saved state to an axis.
+        Applies a saved state to this device.
 
         Args:
-            state: The state object to apply to this axis.
+            state: The state object to apply to this device.
             device_only: If true, only device scope settings and features will be set.
         """
         request = main_pb2.SetStateRequest()
         request.interface_id = self.connection.interface_id
         request.device = self.device_address
         request.state = state
         request.device_only = device_only
         await call_async("device/set_state", request)
 
     def can_set_state(
             self,
             state: str
     ) -> CanSetStateDeviceResponse:
         """
-        Checks if a state can be applied to a device and its peripherals.
+        Checks if a state can be applied to this device.
         This only covers exceptions that can be determined statically such as mismatches of ID or version,
         the process of applying the state can still fail when running.
 
         Args:
             state: The state object to check against.
 
         Returns:
@@ -625,15 +625,15 @@
         return CanSetStateDeviceResponse.from_protobuf(response)
 
     async def can_set_state_async(
             self,
             state: str
     ) -> CanSetStateDeviceResponse:
         """
-        Checks if a state can be applied to a device and its peripherals.
+        Checks if a state can be applied to this device.
         This only covers exceptions that can be determined statically such as mismatches of ID or version,
         the process of applying the state can still fail when running.
 
         Args:
             state: The state object to check against.
 
         Returns:
```

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/device_identity.py` & `zaber_motion-4.2.1/zaber_motion/ascii/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/device_io.py` & `zaber_motion-4.2.1/zaber_motion/ascii/device_io.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/device_io_info.py` & `zaber_motion-4.2.1/zaber_motion/ascii/device_io_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/device_settings.py` & `zaber_motion-4.2.1/zaber_motion/ascii/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/lockstep.py` & `zaber_motion-4.2.1/zaber_motion/ascii/lockstep.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/lockstep_axes.py` & `zaber_motion-4.2.1/zaber_motion/ascii/lockstep_axes.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope.py` & `zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_capture_properties.py` & `zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope_capture_properties.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/oscilloscope_data.py` & `zaber_motion-4.2.1/zaber_motion/ascii/oscilloscope_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/paramset_info.py` & `zaber_motion-4.2.1/zaber_motion/ascii/paramset_info.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/pid_tuning.py` & `zaber_motion-4.2.1/zaber_motion/ascii/pid_tuning.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/pvt_axis_definition.py` & `zaber_motion-4.2.1/zaber_motion/ascii/pvt_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/pvt_buffer.py` & `zaber_motion-4.2.1/zaber_motion/ascii/pvt_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/pvt_sequence.py` & `zaber_motion-4.2.1/zaber_motion/ascii/pvt_sequence.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/response.py` & `zaber_motion-4.2.1/zaber_motion/ascii/response.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/servo_tuner.py` & `zaber_motion-4.2.1/zaber_motion/ascii/servo_tuner.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/servo_tuning_param.py` & `zaber_motion-4.2.1/zaber_motion/ascii/servo_tuning_param.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/setting_constants.py` & `zaber_motion-4.2.1/zaber_motion/ascii/setting_constants.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/simple_tuning_param_definition.py` & `zaber_motion-4.2.1/zaber_motion/ascii/simple_tuning_param_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/storage.py` & `zaber_motion-4.2.1/zaber_motion/ascii/storage.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/stream.py` & `zaber_motion-4.2.1/zaber_motion/ascii/stream.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/stream_axis_definition.py` & `zaber_motion-4.2.1/zaber_motion/ascii/stream_axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/stream_buffer.py` & `zaber_motion-4.2.1/zaber_motion/ascii/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/transport.py` & `zaber_motion-4.2.1/zaber_motion/ascii/transport.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/unknown_response_event.py` & `zaber_motion-4.2.1/zaber_motion/ascii/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/warning_flags.py` & `zaber_motion-4.2.1/zaber_motion/ascii/warning_flags.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/ascii/warnings.py` & `zaber_motion-4.2.1/zaber_motion/ascii/warnings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/__init__.py` & `zaber_motion-4.2.1/zaber_motion/binary/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/binary_settings.py` & `zaber_motion-4.2.1/zaber_motion/binary/binary_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/command_code.py` & `zaber_motion-4.2.1/zaber_motion/binary/command_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/connection.py` & `zaber_motion-4.2.1/zaber_motion/binary/connection.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/device.py` & `zaber_motion-4.2.1/zaber_motion/binary/device.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/device_identity.py` & `zaber_motion-4.2.1/zaber_motion/binary/device_identity.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/device_settings.py` & `zaber_motion-4.2.1/zaber_motion/binary/device_settings.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/error_code.py` & `zaber_motion-4.2.1/zaber_motion/binary/error_code.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/message.py` & `zaber_motion-4.2.1/zaber_motion/binary/message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/reply_only_event.py` & `zaber_motion-4.2.1/zaber_motion/binary/reply_only_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/binary/unknown_response_event.py` & `zaber_motion-4.2.1/zaber_motion/binary/unknown_response_event.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/bindings.py` & `zaber_motion-4.2.1/zaber_motion/bindings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ctypes import c_void_p, c_int, c_int64, c_uint8, CFUNCTYPE
 from typing import Any
 import platform
 import sys
 import importlib
+from .version import __version__
 
 
 def _load_library() -> Any:
     is64bit = sys.maxsize > 2**32
     os_system = platform.system().lower()
     os_machine = platform.machine().lower()
 
@@ -22,15 +23,21 @@
     if os_system == "linux":
         ext = ".so"
     if os_system == "darwin":
         ext = ".dylib"
 
     lib_name = "zaber-motion-lib-{}-{}{}".format(os_system, arch, ext)
     module_name = "zaber_motion_bindings_{}".format(os_system)
-    return importlib.import_module(module_name).load_library(lib_name)
+    binding_module = importlib.import_module(module_name)
+    if __version__ != binding_module.__version__:
+        raise RuntimeError((
+            f"The dependent module {module_name} is not compatible with "
+            f"zaber_motion ({__version__} != {binding_module.__version__}). "
+            f"Please install the correct version {module_name}=={__version__}."))
+    return binding_module.load_library(lib_name)
 
 
 lib = _load_library()
 
 CALLBACK = CFUNCTYPE(None, c_void_p, c_int64)
 
 c_call = lib.call
```

### Comparing `zaber_motion-4.2.0/zaber_motion/call.py` & `zaber_motion-4.2.1/zaber_motion/call.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/convert_exception.py` & `zaber_motion-4.2.1/zaber_motion/convert_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/events.py` & `zaber_motion-4.2.1/zaber_motion/events.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/__init__.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/binary_command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/binary_command_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/binary_command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/command_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/command_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/command_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/command_too_long_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/command_too_long_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/command_too_long_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/device_address_conflict_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/device_address_conflict_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/device_address_conflict_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/device_db_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/device_db_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/device_db_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/g_code_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_execution_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/g_code_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/g_code_syntax_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/g_code_syntax_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/g_code_syntax_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/invalid_packet_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_packet_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/invalid_packet_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_pvt_point.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/invalid_pvt_point.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/invalid_response_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/invalid_response_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/invalid_response_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/movement_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/movement_interrupted_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_execution_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/pvt_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/set_device_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/set_device_state_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/set_device_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/set_peripheral_state_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/set_peripheral_state_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/set_peripheral_state_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_execution_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_execution_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_execution_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_failed_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_failed_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_failed_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py` & `zaber_motion-4.2.1/zaber_motion/exceptions/stream_movement_interrupted_exception_data.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/firmware_version.py` & `zaber_motion-4.2.1/zaber_motion/firmware_version.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/__init__.py` & `zaber_motion-4.2.1/zaber_motion/gcode/__init__.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/axis_definition.py` & `zaber_motion-4.2.1/zaber_motion/gcode/axis_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/axis_mapping.py` & `zaber_motion-4.2.1/zaber_motion/gcode/axis_mapping.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/axis_transformation.py` & `zaber_motion-4.2.1/zaber_motion/gcode/axis_transformation.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/device_definition.py` & `zaber_motion-4.2.1/zaber_motion/gcode/device_definition.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/offline_translator.py` & `zaber_motion-4.2.1/zaber_motion/gcode/offline_translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/translate_message.py` & `zaber_motion-4.2.1/zaber_motion/gcode/translate_message.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/translate_result.py` & `zaber_motion-4.2.1/zaber_motion/gcode/translate_result.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/translator.py` & `zaber_motion-4.2.1/zaber_motion/gcode/translator.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/gcode/translator_config.py` & `zaber_motion-4.2.1/zaber_motion/gcode/translator_config.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/library.py` & `zaber_motion-4.2.1/zaber_motion/library.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/measurement.py` & `zaber_motion-4.2.1/zaber_motion/measurement.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,14 +44,25 @@
     def unit(self, value: Optional[UnitsAndLiterals]) -> None:
         self._unit = value
 
     def __repr__(self) -> str:
         return str(self.__dict__)
 
     @staticmethod
+    def from_protobuf(
+        pb_data: main_pb2.Measurement
+    ) -> 'Measurement':
+        instance = Measurement.__new__(
+            Measurement
+        )  # type: Measurement
+        instance.value = pb_data.value
+        instance.unit = Units(pb_data.unit)
+        return instance
+
+    @staticmethod
     def to_protobuf(source: 'Optional[Measurement]') -> main_pb2.Measurement:
         pb_data = main_pb2.Measurement()
 
         if source is None:
             pb_data.is_null = True
             return pb_data
```

### Comparing `zaber_motion-4.2.0/zaber_motion/microscopy/objective_changer.py` & `zaber_motion-4.2.1/zaber_motion/microscopy/objective_changer.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.py` & `zaber_motion-4.2.1/zaber_motion/protobufs/main_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"E\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14protobufs/main.proto\x12\x16zaber.motion.protobufs\"\x1a\n\x07Request\x12\x0f\n\x07request\x18\x01 \x01(\t\"\xb9\x01\n\x08Response\x12?\n\x08response\x18\x01 \x01(\x0e\x32-.zaber.motion.protobufs.Response.ResponseType\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"!\n\x0cResponseType\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x16\n\x05\x45vent\x12\r\n\x05\x65vent\x18\x01 \x01(\t\"\x0e\n\x0c\x45mptyRequest\"\x1d\n\x0c\x42oolResponse\x12\r\n\x05value\x18\x01 \x01(\x08\"\x1f\n\x0e\x44oubleResponse\x12\r\n\x05value\x18\x01 \x01(\x01\"%\n\x13\x44oubleArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"\x1c\n\x0bIntResponse\x12\r\n\x05value\x18\x01 \x01(\x05\"\x1f\n\x0eStringResponse\x12\r\n\x05value\x18\x01 \x01(\t\"%\n\x13StringArrayResponse\x12\x0e\n\x06values\x18\x01 \x03(\t\"\xdd\x01\n\x0c\x41xisIdentity\x12\x15\n\ris_peripheral\x18\x01 \x01(\x08\x12\x15\n\rperipheral_id\x18\x02 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x03 \x01(\t\x12@\n\taxis_type\x18\x04 \x01(\x0e\x32-.zaber.motion.protobufs.AxisIdentity.AxisType\x12\x13\n\x0bis_modified\x18\x05 \x01(\x08\"/\n\x08\x41xisType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\xcb\x01\n\x0e\x44\x65viceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\naxis_count\x18\x04 \x01(\x05\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x13\n\x0bis_modified\x18\x06 \x01(\x08\x12\x15\n\ris_integrated\x18\x07 \x01(\x08\">\n\x0f\x46irmwareVersion\x12\r\n\x05major\x18\x01 \x01(\x05\x12\r\n\x05minor\x18\x02 \x01(\x05\x12\r\n\x05\x62uild\x18\x03 \x01(\x05\"\x8a\x01\n\x0c\x44\x65viceIOInfo\x12\x1d\n\x15number_analog_outputs\x18\x02 \x01(\x05\x12\x1c\n\x14number_analog_inputs\x18\x03 \x01(\x05\x12\x1e\n\x16number_digital_outputs\x18\x04 \x01(\x05\x12\x1d\n\x15number_digital_inputs\x18\x05 \x01(\x05\";\n\x0bMeasurement\x12\r\n\x05value\x18\x01 \x01(\x01\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\x0f\n\x07is_null\x18\x03 \x01(\x08\">\n\x14StreamAxisDefinition\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x11\n\taxis_type\x18\x02 \x01(\x05\"<\n\x1aInvalidPacketExceptionData\x12\x0e\n\x06packet\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\">\n\"DeviceAddressConflictExceptionData\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"b\n MovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"J\n&StreamMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n#PvtMovementInterruptedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"]\n\x1bMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0e\n\x06\x64\x65vice\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x04 \x01(\x05\"E\n!StreamMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1ePvtMovementFailedExceptionData\x12\x10\n\x08warnings\x18\x01 \x03(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"B\n\x1cStreamExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x80\x01\n\x19PvtExecutionExceptionData\x12\x12\n\nerror_flag\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12?\n\x0einvalid_points\x18\x03 \x03(\x0b\x32\'.zaber.motion.protobufs.InvalidPvtPoint\"/\n\x0fInvalidPvtPoint\x12\r\n\x05index\x18\x01 \x01(\x05\x12\r\n\x05point\x18\x02 \x01(\t\"0\n\x1cInvalidResponseExceptionData\x12\x10\n\x08response\x18\x01 \x01(\t\"\xb7\x01\n\x1a\x43ommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\t\x12\x12\n\nreply_flag\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x04 \x01(\t\x12\x16\n\x0e\x64\x65vice_address\x18\x05 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x06 \x01(\x05\x12\n\n\x02id\x18\x07 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x08 \x01(\t\"9\n BinaryCommandFailedExceptionData\x12\x15\n\rresponse_data\x18\x01 \x01(\x05\"\x89\x01\n\x1fSetPeripheralStateExceptionData\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\x10\n\x08settings\x18\x02 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x03 \x01(\t\x12\x0f\n\x07storage\x18\x04 \x03(\t\x12\x18\n\x10stored_positions\x18\x05 \x03(\t\"\xfd\x01\n\x1bSetDeviceStateExceptionData\x12L\n\x0bperipherals\x18\x02 \x03(\x0b\x32\x37.zaber.motion.protobufs.SetPeripheralStateExceptionData\x12\x10\n\x08settings\x18\x03 \x03(\t\x12\x16\n\x0estream_buffers\x18\x04 \x03(\t\x12\x10\n\x08triggers\x18\x05 \x03(\t\x12\x14\n\x0cservo_tuning\x18\x06 \x01(\t\x12\x0f\n\x07storage\x18\x07 \x03(\t\x12\x18\n\x10stored_positions\x18\x08 \x03(\t\x12\x13\n\x0bpvt_buffers\x18\t \x03(\t\"g\n\x1b\x43ommandTooLongExceptionData\x12\x0b\n\x03\x66it\x18\x01 \x01(\t\x12\x11\n\tremainder\x18\x02 \x01(\t\x12\x13\n\x0bpacket_size\x18\x03 \x01(\x05\x12\x13\n\x0bpackets_max\x18\x04 \x01(\x05\"V\n\x0bTestRequest\x12\x14\n\x0creturn_error\x18\x01 \x01(\x08\x12\x11\n\tdata_ping\x18\x02 \x01(\t\x12\x1e\n\x16return_error_with_data\x18\x03 \x01(\x08\"!\n\x0cTestResponse\x12\x11\n\tdata_pong\x18\x01 \x01(\t\"%\n\x10TestResponseLong\x12\x11\n\tdata_pong\x18\x01 \x03(\t\"\x19\n\tTestEvent\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\"-\n\x1cToolsListSerialPortsResponse\x12\r\n\x05ports\x18\x01 \x03(\t\"&\n\x16SetInternalModeRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x08\"I\n\x18SetDeviceDbSourceRequest\x12\x13\n\x0bsource_type\x18\x01 \x01(\x05\x12\x18\n\x10url_or_file_path\x18\x02 \x01(\t\"G\n\x1aToggleDeviceDbStoreRequest\x12\x11\n\ttoggle_on\x18\x01 \x01(\x08\x12\x16\n\x0estore_location\x18\x02 \x01(\t\"+\n\x1b\x44\x65viceDbFailedExceptionData\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\"\xa7\x02\n\x14OpenInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x11\n\ttransport\x18\x06 \x01(\x05\x12 \n\x18reject_routed_connection\x18\x07 \x01(\x08\x12\x10\n\x08\x63loud_id\x18\x08 \x01(\t\x12\x17\n\x0f\x63onnection_name\x18\t \x01(\t\x12\r\n\x05realm\x18\n \x01(\t\x12\r\n\x05token\x18\x0b \x01(\t\x12\x0b\n\x03\x61pi\x18\x0c \x01(\t\"-\n\x15OpenInterfaceResponse\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"-\n\x15InterfaceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\"C\n\x1aSetInterfaceTimeoutRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0f\n\x07timeout\x18\x02 \x01(\x05\"N\n\"SetInterfaceChecksumEnabledRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x12\n\nis_enabled\x18\x02 \x01(\x08\"F\n\x10\x41xisEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\"\x83\x01\n\x15GenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x04 \x01(\t\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x05\"\xc8\x01\n\x16GenericCommandResponse\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"e\n GenericCommandResponseCollection\x12\x41\n\tresponses\x18\x02 \x03(\x0b\x32..zaber.motion.protobufs.GenericCommandResponse\"\xdc\x01\n\x14UnknownResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x12\n\nreply_flag\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x06 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x07 \x01(\t\x12\x39\n\x0cmessage_type\x18\x08 \x01(\x0e\x32#.zaber.motion.protobufs.MessageType\"\x83\x01\n\nAlertEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x14\n\x0cwarning_flag\x18\x05 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x06 \x01(\t\"t\n\x11\x44isconnectedEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x32\n\nerror_type\x18\x02 \x01(\x0e\x32\x1e.zaber.motion.protobufs.Errors\x12\x15\n\rerror_message\x18\x03 \x01(\t\"~\n\x15\x44\x65viceIdentifyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12?\n\x0e\x61ssume_version\x18\x03 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\"D\n\x15\x44\x65viceRenumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x15\n\rfirst_address\x18\x02 \x01(\x05\"\xba\x01\n\x13\x44\x65viceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\x12\x44\n\x04type\x18\x03 \x01(\x0e\x32\x36.zaber.motion.protobufs.DeviceDetectRequest.DeviceType\"-\n\nDeviceType\x12\x07\n\x03\x41NY\x10\x00\x12\x16\n\x12PROCESS_CONTROLLER\x10\x01\"\'\n\x14\x44\x65viceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"`\n\x11\x44\x65viceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"n\n\x1a\x44\x65viceWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"\xd0\x02\n\x11\x44\x65viceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12@\n\x04type\x18\x05 \x01(\x0e\x32\x32.zaber.motion.protobufs.DeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\x12\x10\n\x08velocity\x18\x08 \x01(\x01\x12\x15\n\rvelocity_unit\x18\t \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\n \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0b \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"`\n\x11\x44\x65viceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"C\n\x12\x44\x65viceOnAllRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"/\n\x13\x44\x65viceOnAllResponse\x12\x18\n\x10\x64\x65vice_addresses\x18\x01 \x03(\x05\"]\n\x18\x44\x65viceGetWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05\x63lear\x18\x04 \x01(\x08\"*\n\x19\x44\x65viceGetWarningsResponse\x12\r\n\x05\x66lags\x18\x01 \x03(\t\"x\n\x1aWaitToClearWarningsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07timeout\x18\x04 \x01(\x01\x12\x15\n\rwarning_flags\x18\x05 \x03(\t\"Z\n\x1c\x44\x65viceGetAllDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\"/\n\x1d\x44\x65viceGetAllDigitalIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x08\"Y\n\x1b\x44\x65viceGetAllAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\".\n\x1c\x44\x65viceGetAllAnalogIOResponse\x12\x0e\n\x06values\x18\x01 \x03(\x01\"o\n\x19\x44\x65viceGetDigitalIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"n\n\x18\x44\x65viceGetAnalogIORequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x14\n\x0c\x63hannel_type\x18\x03 \x01(\t\x12\x16\n\x0e\x63hannel_number\x18\x04 \x01(\x05\"Y\n!DeviceSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x08\"X\n DeviceSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0e\n\x06values\x18\x03 \x03(\x01\"l\n\x1d\x44\x65viceSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x08\"k\n\x1c\x44\x65viceSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x16\n\x0e\x63hannel_number\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\"6\n\x13SetLogOutputRequest\x12\x0c\n\x04mode\x18\x01 \x01(\x05\x12\x11\n\tfile_path\x18\x02 \x01(\t\"l\n\x17\x44\x65viceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x94\x01\n\x1b\x44\x65viceConvertSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\r\n\x05value\x18\x06 \x01(\x01\x12\x13\n\x0b\x66rom_native\x18\x07 \x01(\x08\"{\n\x17\x44\x65viceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"p\n\x1a\x44\x65viceSetSettingStrRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\"\x9e\x01\n\x15PrepareCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x18\n\x10\x63ommand_template\x18\x04 \x01(\t\x12\x37\n\nparameters\x18\x05 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"M\n\x14WaitToRespondRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\"f\n\x15LockstepEnableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x04 \x03(\x05\"r\n\x16LockstepDisableRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"o\n\x13LockstepHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\"\xe1\x02\n\x13LockstepMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x04 \x01(\x08\x12\x42\n\x04type\x18\x05 \x01(\x0e\x32\x34.zaber.motion.protobufs.LockstepMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x08 \x01(\t\x12\x10\n\x08velocity\x18\t \x01(\x01\x12\x15\n\rvelocity_unit\x18\n \x01(\t\x12\x14\n\x0c\x61\x63\x63\x65leration\x18\x0b \x01(\x01\x12\x19\n\x11\x61\x63\x63\x65leration_unit\x18\x0c \x01(\t\"7\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\x12\x07\n\x03MAX\x10\x03\x12\x07\n\x03MIN\x10\x04\"}\n\x1cLockstepWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x1c\n\x14throw_error_on_fault\x18\x04 \x01(\x08\"W\n\x14LockstepEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\"N\n\x0cLockstepAxes\x12\x0e\n\x06\x61xis_1\x18\x01 \x01(\x05\x12\x0e\n\x06\x61xis_2\x18\x02 \x01(\x05\x12\x0e\n\x06\x61xis_3\x18\x03 \x01(\x05\x12\x0e\n\x06\x61xis_4\x18\x04 \x01(\x05\".\n\x1eLockstepGetAxisNumbersResponse\x12\x0c\n\x04\x61xes\x18\x01 \x03(\x05\"c\n\x12LockstepGetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\x86\x01\n\x12LockstepSetRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x19\n\x11lockstep_group_id\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\x12\x12\n\naxis_index\x18\x06 \x01(\x05\"k\n$OscilloscopeAddSettingChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0f\n\x07setting\x18\x04 \x01(\t\"l\n\x1fOscilloscopeAddIoChannelRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07io_type\x18\x03 \x01(\x05\x12\x12\n\nio_channel\x18\x04 \x01(\x05\"k\n\x1cOscilloscopeStartStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\r\n\x05start\x18\x03 \x01(\x08\x12\x16\n\x0e\x63\x61pture_length\x18\x04 \x01(\x05\",\n\x18OscilloscopeReadResponse\x12\x10\n\x08\x64\x61ta_ids\x18\x01 \x03(\x05\"-\n\x1aOscilloscopeDataIdentifier\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\"\x7f\n\x1dOscilloscopeCaptureProperties\x12\x13\n\x0b\x64\x61ta_source\x18\x01 \x01(\x05\x12\x0f\n\x07setting\x18\x02 \x01(\t\x12\x13\n\x0b\x61xis_number\x18\x03 \x01(\x05\x12\x0f\n\x07io_type\x18\x04 \x01(\x05\x12\x12\n\nio_channel\x18\x05 \x01(\x05\";\n\x1aOscilloscopeDataGetRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\"T\n$OscilloscopeDataGetSampleTimeRequest\x12\x0f\n\x07\x64\x61ta_id\x18\x01 \x01(\x05\x12\x0c\n\x04unit\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\"2\n\"OscilloscopeDataGetSamplesResponse\x12\x0c\n\x04\x64\x61ta\x18\x01 \x03(\x01\"l\n\x16StreamSetupLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04\x61xes\x18\x05 \x03(\x05\"\xa3\x01\n\x1fStreamSetupLiveCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04\x61xes\x18\x05 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\x98\x01\n\x17StreamSetupStoreRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x07 \x03(\x05\"\xcf\x01\n StreamSetupStoreCompositeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12:\n\x04\x61xes\x18\x07 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"\xab\x01\n$StreamSetupStoreArbitraryAxesRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\x12\x12\n\naxes_count\x18\x07 \x01(\x05\"\x84\x01\n\x11StreamCallRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x15\n\rstream_buffer\x18\x05 \x01(\x05\x12\x12\n\npvt_buffer\x18\x06 \x01(\x05\"\xd1\x02\n\x0fPvtPointRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12:\n\x04type\x18\x05 \x01(\x0e\x32,.zaber.motion.protobufs.PvtPointRequest.Type\x12\x36\n\tpositions\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x37\n\nvelocities\x18\x07 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x31\n\x04time\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x85\x02\n\x11StreamLineRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12<\n\x04type\x18\x05 \x01(\x0e\x32..zaber.motion.protobufs.StreamLineRequest.Type\x12\x35\n\x08\x65ndpoint\x18\x06 \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x07 \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xf5\x03\n\x10StreamArcRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12;\n\x04type\x18\x05 \x01(\x0e\x32-.zaber.motion.protobufs.StreamArcRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_x\x18\t \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x32\n\x05\x65nd_y\x18\n \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\x0b \x03(\x05\x12\x35\n\x08\x65ndpoint\x18\x0c \x03(\x0b\x32#.zaber.motion.protobufs.Measurement\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\xdc\x02\n\x13StreamCircleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12>\n\x04type\x18\x05 \x01(\x0e\x32\x30.zaber.motion.protobufs.StreamCircleRequest.Type\x12\x1a\n\x12rotation_direction\x18\x06 \x01(\x05\x12\x35\n\x08\x63\x65nter_x\x18\x07 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x35\n\x08\x63\x65nter_y\x18\x08 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\x12\x1b\n\x13target_axes_indices\x18\t \x03(\x05\"\x18\n\x04Type\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\"\x8c\x01\n\x1dStreamWaitDigitalInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x9e\x01\n\x1cStreamWaitAnalogInputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\x11\n\tcondition\x18\x06 \x01(\t\x12\r\n\x05value\x18\x07 \x01(\x01\"\x8c\x01\n\x1dStreamSetDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x08\"\x8b\x01\n\x1cStreamSetAnalogOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\x12\r\n\x05value\x18\x06 \x01(\x01\"\x80\x01\n StreamToggleDigitalOutputRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x16\n\x0e\x63hannel_number\x18\x05 \x01(\x05\"y\n!StreamSetAllDigitalOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x08\"x\n StreamSetAllAnalogOutputsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0e\n\x06values\x18\x05 \x03(\x01\"u\n\x11StreamWaitRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04time\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n\x1aStreamWaitUntilIdleRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x1c\n\x14throw_error_on_fault\x18\x05 \x01(\x08\"Z\n\x12StreamEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"S\n\x15StreamGetAxesResponse\x12:\n\x04\x61xes\x18\x01 \x03(\x0b\x32,.zaber.motion.protobufs.StreamAxisDefinition\"n\n\x18StreamGetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\x81\x01\n\x18StreamSetMaxSpeedRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x05 \x01(\x08\x12\x11\n\tmax_speed\x18\x06 \x01(\x01\x12\x0c\n\x04unit\x18\x07 \x01(\t\"\x7f\n)StreamGetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa4\x01\n)StreamSetMaxTangentialAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12#\n\x1bmax_tangential_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"\x80\x01\n*StreamGetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0c\n\x04unit\x18\x05 \x01(\t\"\xa6\x01\n*StreamSetMaxCentripetalAccelerationRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12$\n\x1cmax_centripetal_acceleration\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"e\n\x1dStreamBufferGetContentRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"6\n\x1eStreamBufferGetContentResponse\x12\x14\n\x0c\x62uffer_lines\x18\x01 \x03(\t\"`\n\x18StreamBufferEraseRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tbuffer_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\"t\n\x1bStreamGenericCommandRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\x0f\n\x07\x63ommand\x18\x05 \x01(\t\"w\n StreamGenericCommandBatchRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x0b\n\x03pvt\x18\x04 \x01(\x08\x12\r\n\x05\x62\x61tch\x18\x05 \x03(\t\"c\n\x14\x42inaryReplyOnlyEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\xbb\x01\n\x1aOpenBinaryInterfaceRequest\x12=\n\x0einterface_type\x18\x01 \x01(\x0e\x32%.zaber.motion.protobufs.InterfaceType\x12\x11\n\tport_name\x18\x02 \x01(\t\x12\x11\n\tbaud_rate\x18\x03 \x01(\x05\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x0c\n\x04port\x18\x05 \x01(\x05\x12\x17\n\x0fuse_message_ids\x18\x06 \x01(\x08\"i\n\x1aUnknownBinaryResponseEvent\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0e\x64\x65vice_address\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\"\x82\x01\n\x14GenericBinaryRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x05\x12\x14\n\x0c\x63heck_errors\x18\x05 \x01(\x08\x12\x0f\n\x07timeout\x18\x06 \x01(\x01\"F\n\rBinaryMessage\x12\x16\n\x0e\x64\x65vice_address\x18\x01 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x02 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x05\"R\n\x17\x42inaryMessageCollection\x12\x37\n\x08messages\x18\x02 \x03(\x0b\x32%.zaber.motion.protobufs.BinaryMessage\":\n\x12\x44\x65viceEmptyRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\"\xd9\x02\n\x14\x42inaryDeviceIdentity\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12\x15\n\rserial_number\x18\x02 \x01(\r\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x41\n\x10\x66irmware_version\x18\x05 \x01(\x0b\x32\'.zaber.motion.protobufs.FirmwareVersion\x12\x15\n\ris_peripheral\x18\x06 \x01(\x08\x12\x15\n\rperipheral_id\x18\x07 \x01(\x05\x12\x17\n\x0fperipheral_name\x18\x08 \x01(\t\x12L\n\x0b\x64\x65vice_type\x18\t \x01(\x0e\x32\x37.zaber.motion.protobufs.BinaryDeviceIdentity.DeviceType\"1\n\nDeviceType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06LINEAR\x10\x01\x12\n\n\x06ROTARY\x10\x02\"\x99\x01\n\x1d\x42inaryGenericWithUnitsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07\x63ommand\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x01\x12\x11\n\tfrom_unit\x18\x05 \x01(\t\x12\x0f\n\x07to_unit\x18\x06 \x01(\t\x12\x0f\n\x07timeout\x18\x07 \x01(\x01\"^\n\x17\x42inaryDeviceHomeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"\xda\x01\n\x17\x42inaryDeviceMoveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x46\n\x04type\x18\x04 \x01(\x0e\x32\x38.zaber.motion.protobufs.BinaryDeviceMoveRequest.MoveType\x12\x0b\n\x03\x61rg\x18\x05 \x01(\x01\x12\x0c\n\x04unit\x18\x06 \x01(\t\"%\n\x08MoveType\x12\x07\n\x03\x41\x42S\x10\x00\x12\x07\n\x03REL\x10\x01\x12\x07\n\x03VEL\x10\x02\"^\n\x17\x42inaryDeviceStopRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07timeout\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"K\n\x19\x42inaryDeviceDetectRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x18\n\x10identify_devices\x18\x02 \x01(\x08\"-\n\x1a\x42inaryDeviceDetectResponse\x12\x0f\n\x07\x64\x65vices\x18\x01 \x03(\x05\"d\n\x1d\x42inaryDeviceGetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\x0c\n\x04unit\x18\x04 \x01(\t\"s\n\x1d\x42inaryDeviceSetSettingRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0f\n\x07setting\x18\x03 \x01(\x05\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0c\n\x04unit\x18\x05 \x01(\t\"2\n\x1a\x43ustomInterfaceReadRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"D\n\x1b\x43ustomInterfaceWriteRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\"3\n\x1b\x43ustomInterfaceOpenResponse\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\"J\n\x1b\x43ustomInterfaceCloseRequest\x12\x14\n\x0ctransport_id\x18\x01 \x01(\x05\x12\x15\n\rerror_message\x18\x02 \x01(\t\"W\n\x12\x43\x61nSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\"=\n\x17\x43\x61nSetStateAxisResponse\x12\x13\n\x0b\x61xis_number\x18\x01 \x01(\x05\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"p\n\x19\x43\x61nSetStateDeviceResponse\x12\r\n\x05\x65rror\x18\x01 \x01(\t\x12\x44\n\x0b\x61xis_errors\x18\x02 \x03(\x0b\x32/.zaber.motion.protobufs.CanSetStateAxisResponse\"i\n\x0fSetStateRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\r\n\x05state\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x65vice_only\x18\x05 \x01(\x08\"Z\n\x12ServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\"/\n\x10ServoTuningParam\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\"g\n\x0cParamsetInfo\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\x12\x38\n\x06params\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"\x9e\x01\n\x15SetServoTuningRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12?\n\rtuning_params\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"n\n\x0cLoadParamset\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x13\n\x0bto_paramset\x18\x04 \x01(\x05\x12\x15\n\rfrom_paramset\x18\x05 \x01(\x05\"\x8d\x01\n\x18SetServoTuningPIDRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\t\n\x01p\x18\x05 \x01(\x01\x12\t\n\x01i\x18\x06 \x01(\x01\x12\t\n\x01\x64\x18\x07 \x01(\x01\x12\n\n\x02\x66\x63\x18\x08 \x01(\x01\"W\n\tPidTuning\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\t\n\x01p\x18\x03 \x01(\x01\x12\t\n\x01i\x18\x04 \x01(\x01\x12\t\n\x01\x64\x18\x05 \x01(\x01\x12\n\n\x02\x66\x63\x18\x06 \x01(\x01\"\xc2\x01\n\x0fSetSimpleTuning\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x10\n\x08paramset\x18\x04 \x01(\x05\x12\x15\n\rcarriage_mass\x18\x05 \x01(\x01\x12\x11\n\tload_mass\x18\x06 \x01(\x01\x12?\n\rtuning_params\x18\x07 \x03(\x0b\x32(.zaber.motion.protobufs.ServoTuningParam\"d\n\x1bSimpleTuningParamDefinition\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tmin_label\x18\x02 \x01(\t\x12\x11\n\tmax_label\x18\x03 \x01(\t\x12\x11\n\tdata_type\x18\x04 \x01(\t\"m\n&GetSimpleTuningParamDefinitionResponse\x12\x43\n\x06params\x18\x01 \x03(\x0b\x32\x33.zaber.motion.protobufs.SimpleTuningParamDefinition\"\x95\x01\n\x17TranslatorCreateRequest\x12@\n\ndefinition\x18\x01 \x01(\x0b\x32,.zaber.motion.protobufs.TranslatorDefinition\x12\x38\n\x06\x63onfig\x18\x02 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"1\n\x18TranslatorCreateResponse\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"O\n\x18TranslatorAxisDefinition\x12\x15\n\rperipheral_id\x18\x01 \x01(\x05\x12\x1c\n\x14microstep_resolution\x18\x02 \x01(\x05\"\xa1\x01\n\x14TranslatorDefinition\x12\x11\n\tdevice_id\x18\x01 \x01(\x05\x12>\n\x04\x61xes\x18\x02 \x03(\x0b\x32\x30.zaber.motion.protobufs.TranslatorAxisDefinition\x12\x36\n\tmax_speed\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"\xac\x01\n\x10TranslatorConfig\x12\x44\n\raxis_mappings\x18\x01 \x03(\x0b\x32-.zaber.motion.protobufs.TranslatorAxisMapping\x12R\n\x14\x61xis_transformations\x18\x02 \x03(\x0b\x32\x34.zaber.motion.protobufs.TranslatorAxisTransformation\"@\n\x15TranslatorAxisMapping\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x12\n\naxis_index\x18\x02 \x01(\x05\"~\n\x1cTranslatorAxisTransformation\x12\x13\n\x0b\x61xis_letter\x18\x01 \x01(\t\x12\x0f\n\x07scaling\x18\x02 \x01(\x01\x12\x38\n\x0btranslation\x18\x03 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"B\n\x1aTranslatorTranslateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\r\n\x05\x62lock\x18\x02 \x01(\t\"I\n\x10TranslateMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\nfrom_block\x18\x02 \x01(\x05\x12\x10\n\x08to_block\x18\x03 \x01(\x05\"k\n\x1bTranslatorTranslateResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\x12:\n\x08warnings\x18\x02 \x03(\x0b\x32(.zaber.motion.protobufs.TranslateMessage\"@\n\x18GCodeSyntaxExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"C\n\x1bGCodeExecutionExceptionData\x12\x12\n\nfrom_block\x18\x01 \x01(\x05\x12\x10\n\x08to_block\x18\x02 \x01(\x05\"L\n\x1aTranslatorFlushLiveRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x17\n\x0fwait_until_idle\x18\x02 \x01(\x08\"+\n\x17TranslatorFlushResponse\x12\x10\n\x08\x63ommands\x18\x01 \x03(\t\"\x90\x01\n\x1bTranslatorCreateLiveRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x11\n\tstream_id\x18\x03 \x01(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"\x91\x01\n!TranslatorCreateFromDeviceRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xes\x18\x03 \x03(\x05\x12\x38\n\x06\x63onfig\x18\x04 \x01(\x0b\x32(.zaber.motion.protobufs.TranslatorConfig\"/\n\x16TranslatorEmptyRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\"^\n TranslatorSetTraverseRateRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x15\n\rtraverse_rate\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"g\n TranslatorSetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x10\n\x08position\x18\x03 \x01(\x01\x12\x0c\n\x04unit\x18\x04 \x01(\t\"U\n TranslatorGetAxisPositionRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x02 \x01(\t\x12\x0c\n\x04unit\x18\x03 \x01(\t\"n\n\x1eTranslatorGetAxisOffsetRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x19\n\x11\x63oordinate_system\x18\x02 \x01(\t\x12\x0c\n\x04\x61xis\x18\x03 \x01(\t\x12\x0c\n\x04unit\x18\x04 \x01(\t\"R\n$TranslatorSetFeedRateOverrideRequest\x12\x15\n\rtranslator_id\x18\x01 \x01(\x05\x12\x13\n\x0b\x63oefficient\x18\x02 \x01(\x01\"y\n\x17\x44\x65viceSetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x0e\n\x06\x65ncode\x18\x06 \x01(\x08\"j\n\x17\x44\x65viceGetStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\x0e\n\x06\x64\x65\x63ode\x18\x05 \x01(\x08\"o\n\x1d\x44\x65viceSetStorageNumberRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x01\"m\n\x1b\x44\x65viceSetStorageBoolRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\x08\"W\n\x14\x44\x65viceStorageRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\"b\n\x1c\x44\x65viceStorageListKeysRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0e\n\x06prefix\x18\x04 \x01(\t\"\xa1\x01\n\x1f\x44\x65viceSetUnitConversionsRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\x0b\n\x03key\x18\x04 \x01(\t\x12=\n\x0b\x63onversions\x18\x05 \x03(\x0b\x32(.zaber.motion.protobufs.ConversionFactor\"@\n\x10\x43onversionFactor\x12\x0f\n\x07setting\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x01\x12\x0c\n\x04unit\x18\x03 \x01(\t\"^\n\x17ObjectiveChangerRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\"?\n\x1eObjectiveChangerCreateResponse\x12\x0e\n\x06turret\x18\x02 \x01(\x05\x12\r\n\x05\x66ocus\x18\x03 \x01(\x05\"\xb2\x01\n\x1dObjectiveChangerChangeRequest\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x16\n\x0eturret_address\x18\x02 \x01(\x05\x12\x15\n\rfocus_address\x18\x03 \x01(\x05\x12\x11\n\tobjective\x18\x04 \x01(\x05\x12\x39\n\x0c\x66ocus_offset\x18\x05 \x01(\x0b\x32#.zaber.motion.protobufs.Measurement\"]\n\tProcessOn\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12\n\n\x02on\x18\x04 \x01(\x08\x12\x10\n\x08\x64uration\x18\x05 \x01(\x01\"7\n\x17ProcessControllerSource\x12\x0e\n\x06sensor\x18\x01 \x01(\x05\x12\x0c\n\x04port\x18\x02 \x01(\x05\"\x91\x01\n\x1aSetProcessControllerSource\x12\x14\n\x0cinterface_id\x18\x01 \x01(\x05\x12\x0e\n\x06\x64\x65vice\x18\x02 \x01(\x05\x12\x0c\n\x04\x61xis\x18\x03 \x01(\x05\x12?\n\x06source\x18\x04 \x01(\x0b\x32/.zaber.motion.protobufs.ProcessControllerSource*-\n\x0bMessageType\x12\t\n\x05REPLY\x10\x00\x12\x08\n\x04INFO\x10\x01\x12\t\n\x05\x41LERT\x10\x02*\xc0\t\n\x06\x45rrors\x12\x13\n\x0fREQUEST_TIMEOUT\x10\x00\x12\x15\n\x11\x43ONNECTION_CLOSED\x10\x01\x12\x14\n\x10INVALID_ARGUMENT\x10\x02\x12\x16\n\x12OUT_OF_REQUEST_IDS\x10\x03\x12\x12\n\x0eINVALID_PACKET\x10\x04\x12\x15\n\x11\x43ONNECTION_FAILED\x10\x05\x12\x13\n\x0fUNKNOWN_REQUEST\x10\x06\x12\x12\n\x0e\x43OMMAND_FAILED\x10\x07\x12\x14\n\x10\x44\x45VICE_DB_FAILED\x10\x08\x12\x10\n\x0cINVALID_DATA\x10\t\x12\x19\n\x15\x44\x45VICE_NOT_IDENTIFIED\x10\n\x12\x15\n\x11\x43ONVERSION_FAILED\x10\x0b\x12\x1b\n\x17\x44\x45VICE_ADDRESS_CONFLICT\x10\x0c\x12\x13\n\x0fNO_DEVICE_FOUND\x10\r\x12\x18\n\x14MOVEMENT_INTERRUPTED\x10\x0e\x12\x13\n\x0fMOVEMENT_FAILED\x10\x0f\x12\r\n\tIO_FAILED\x10\x10\x12\x14\n\x10INVALID_RESPONSE\x10\x11\x12\x11\n\rNOT_SUPPORTED\x10\x12\x12\x11\n\rDEVICE_FAILED\x10\x13\x12\r\n\tOS_FAILED\x10\x14\x12\x12\n\x0eINTERNAL_ERROR\x10\x16\x12\x19\n\x15\x42INARY_COMMAND_FAILED\x10\x18\x12\x15\n\x11\x43OMMAND_PREEMPTED\x10\x19\x12\x18\n\x14LOCKSTEP_NOT_ENABLED\x10\x1a\x12\x14\n\x10LOCKSTEP_ENABLED\x10\x1b\x12\x1b\n\x17IO_CHANNEL_OUT_OF_RANGE\x10\x1c\x12\x15\n\x11SETTING_NOT_FOUND\x10\x1d\x12\x0f\n\x0bSTREAM_MODE\x10\x1e\x12\x14\n\x10STREAM_EXECUTION\x10\x1f\x12\x1a\n\x16STREAM_MOVEMENT_FAILED\x10 \x12\x17\n\x13STREAM_SETUP_FAILED\x10!\x12\x0f\n\x0b\x44\x45VICE_BUSY\x10\"\x12\x1f\n\x1bSTREAM_MOVEMENT_INTERRUPTED\x10#\x12\x16\n\x12INVALID_PARK_STATE\x10$\x12\x14\n\x10SERIAL_PORT_BUSY\x10%\x12\x1a\n\x16TRANSPORT_ALREADY_USED\x10&\x12\x1f\n\x1bSET_PERIPHERAL_STATE_FAILED\x10\'\x12\x1b\n\x17SET_DEVICE_STATE_FAILED\x10(\x12\x11\n\rG_CODE_SYNTAX\x10)\x12\x14\n\x10G_CODE_EXECUTION\x10*\x12\x15\n\x11INVALID_OPERATION\x10+\x12\x14\n\x10\x43OMMAND_TOO_LONG\x10,\x12\x14\n\x10NO_VALUE_FOR_KEY\x10-\x12\x1b\n\x17\x44\x45VICE_DETECTION_FAILED\x10.\x12\x0b\n\x07TIMEOUT\x10/\x12\x0c\n\x08PVT_MODE\x10\x30\x12\x11\n\rPVT_EXECUTION\x10\x31\x12\x14\n\x10PVT_SETUP_FAILED\x10\x32\x12\x17\n\x13PVT_MOVEMENT_FAILED\x10\x33\x12\x1c\n\x18PVT_MOVEMENT_INTERRUPTED\x10\x34\x12\x15\n\x11PVT_DISCONTINUITY\x10\x35\x12\x18\n\x14STREAM_DISCONTINUITY\x10\x36*Q\n\rInterfaceType\x12\x0f\n\x0bSERIAL_PORT\x10\x00\x12\x07\n\x03TCP\x10\x01\x12\n\n\x06\x43USTOM\x10\x02\x12\x07\n\x03IOT\x10\x03\x12\x11\n\rNETWORK_SHARE\x10\x04\x42$Z\"./protobufs;zaber_motion_protobufsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protobufs.main_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\"./protobufs;zaber_motion_protobufs'
-  _MESSAGETYPE._serialized_start=22390
-  _MESSAGETYPE._serialized_end=22435
-  _ERRORS._serialized_start=22438
-  _ERRORS._serialized_end=23654
-  _INTERFACETYPE._serialized_start=23656
-  _INTERFACETYPE._serialized_end=23737
+  _MESSAGETYPE._serialized_start=22808
+  _MESSAGETYPE._serialized_end=22853
+  _ERRORS._serialized_start=22856
+  _ERRORS._serialized_end=24072
+  _INTERFACETYPE._serialized_start=24074
+  _INTERFACETYPE._serialized_end=24155
   _REQUEST._serialized_start=48
   _REQUEST._serialized_end=74
   _RESPONSE._serialized_start=77
   _RESPONSE._serialized_end=262
   _RESPONSE_RESPONSETYPE._serialized_start=229
   _RESPONSE_RESPONSETYPE._serialized_end=262
   _EVENT._serialized_start=264
@@ -139,318 +139,326 @@
   _ALERTEVENT._serialized_end=4799
   _DISCONNECTEDEVENT._serialized_start=4801
   _DISCONNECTEDEVENT._serialized_end=4917
   _DEVICEIDENTIFYREQUEST._serialized_start=4919
   _DEVICEIDENTIFYREQUEST._serialized_end=5045
   _DEVICERENUMBERREQUEST._serialized_start=5047
   _DEVICERENUMBERREQUEST._serialized_end=5115
-  _DEVICEDETECTREQUEST._serialized_start=5117
-  _DEVICEDETECTREQUEST._serialized_end=5186
-  _DEVICEDETECTRESPONSE._serialized_start=5188
-  _DEVICEDETECTRESPONSE._serialized_end=5227
-  _DEVICEHOMEREQUEST._serialized_start=5229
-  _DEVICEHOMEREQUEST._serialized_end=5325
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=5327
-  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5437
-  _DEVICEMOVEREQUEST._serialized_start=5440
-  _DEVICEMOVEREQUEST._serialized_end=5776
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5721
-  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5776
-  _DEVICESTOPREQUEST._serialized_start=5778
-  _DEVICESTOPREQUEST._serialized_end=5874
-  _DEVICEONALLREQUEST._serialized_start=5876
-  _DEVICEONALLREQUEST._serialized_end=5943
-  _DEVICEONALLRESPONSE._serialized_start=5945
-  _DEVICEONALLRESPONSE._serialized_end=5992
-  _DEVICEGETWARNINGSREQUEST._serialized_start=5994
-  _DEVICEGETWARNINGSREQUEST._serialized_end=6087
-  _DEVICEGETWARNINGSRESPONSE._serialized_start=6089
-  _DEVICEGETWARNINGSRESPONSE._serialized_end=6131
-  _WAITTOCLEARWARNINGSREQUEST._serialized_start=6133
-  _WAITTOCLEARWARNINGSREQUEST._serialized_end=6253
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=6255
-  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=6345
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=6347
-  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=6394
-  _DEVICEGETALLANALOGIOREQUEST._serialized_start=6396
-  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6485
-  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6487
-  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6533
-  _DEVICEGETDIGITALIOREQUEST._serialized_start=6535
-  _DEVICEGETDIGITALIOREQUEST._serialized_end=6646
-  _DEVICEGETANALOGIOREQUEST._serialized_start=6648
-  _DEVICEGETANALOGIOREQUEST._serialized_end=6758
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6760
-  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6849
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6851
-  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=6939
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=6941
-  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=7049
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=7051
-  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=7158
-  _SETLOGOUTPUTREQUEST._serialized_start=7160
-  _SETLOGOUTPUTREQUEST._serialized_end=7214
-  _DEVICEGETSETTINGREQUEST._serialized_start=7216
-  _DEVICEGETSETTINGREQUEST._serialized_end=7324
-  _DEVICECONVERTSETTINGREQUEST._serialized_start=7327
-  _DEVICECONVERTSETTINGREQUEST._serialized_end=7475
-  _DEVICESETSETTINGREQUEST._serialized_start=7477
-  _DEVICESETSETTINGREQUEST._serialized_end=7600
-  _DEVICESETSETTINGSTRREQUEST._serialized_start=7602
-  _DEVICESETSETTINGSTRREQUEST._serialized_end=7714
-  _PREPARECOMMANDREQUEST._serialized_start=7717
-  _PREPARECOMMANDREQUEST._serialized_end=7875
-  _WAITTORESPONDREQUEST._serialized_start=7877
-  _WAITTORESPONDREQUEST._serialized_end=7954
-  _LOCKSTEPENABLEREQUEST._serialized_start=7956
-  _LOCKSTEPENABLEREQUEST._serialized_end=8058
-  _LOCKSTEPDISABLEREQUEST._serialized_start=8060
-  _LOCKSTEPDISABLEREQUEST._serialized_end=8174
-  _LOCKSTEPSTOPREQUEST._serialized_start=8176
-  _LOCKSTEPSTOPREQUEST._serialized_end=8287
-  _LOCKSTEPHOMEREQUEST._serialized_start=8289
-  _LOCKSTEPHOMEREQUEST._serialized_end=8400
-  _LOCKSTEPMOVEREQUEST._serialized_start=8403
-  _LOCKSTEPMOVEREQUEST._serialized_end=8756
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5721
-  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5776
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8758
-  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=8883
-  _LOCKSTEPEMPTYREQUEST._serialized_start=8885
-  _LOCKSTEPEMPTYREQUEST._serialized_end=8972
-  _LOCKSTEPAXES._serialized_start=8974
-  _LOCKSTEPAXES._serialized_end=9052
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=9054
-  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=9100
-  _LOCKSTEPGETREQUEST._serialized_start=9102
-  _LOCKSTEPGETREQUEST._serialized_end=9201
-  _LOCKSTEPSETREQUEST._serialized_start=9204
-  _LOCKSTEPSETREQUEST._serialized_end=9338
-  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_start=9340
-  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_end=9447
-  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_start=9449
-  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_end=9557
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9559
-  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9666
-  _OSCILLOSCOPEREADRESPONSE._serialized_start=9668
-  _OSCILLOSCOPEREADRESPONSE._serialized_end=9712
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9714
-  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9759
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9761
-  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=9888
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=9890
-  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=9949
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=9951
-  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=10035
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=10037
-  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=10087
-  _STREAMSETUPLIVEREQUEST._serialized_start=10089
-  _STREAMSETUPLIVEREQUEST._serialized_end=10197
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=10200
-  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=10363
-  _STREAMSETUPSTOREREQUEST._serialized_start=10366
-  _STREAMSETUPSTOREREQUEST._serialized_end=10518
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=10521
-  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10728
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10731
-  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=10902
-  _STREAMCALLREQUEST._serialized_start=10905
-  _STREAMCALLREQUEST._serialized_end=11037
-  _PVTPOINTREQUEST._serialized_start=11040
-  _PVTPOINTREQUEST._serialized_end=11377
-  _PVTPOINTREQUEST_TYPE._serialized_start=11353
-  _PVTPOINTREQUEST_TYPE._serialized_end=11377
-  _STREAMLINEREQUEST._serialized_start=11380
-  _STREAMLINEREQUEST._serialized_end=11641
-  _STREAMLINEREQUEST_TYPE._serialized_start=11353
-  _STREAMLINEREQUEST_TYPE._serialized_end=11377
-  _STREAMARCREQUEST._serialized_start=11644
-  _STREAMARCREQUEST._serialized_end=12145
-  _STREAMARCREQUEST_TYPE._serialized_start=11353
-  _STREAMARCREQUEST_TYPE._serialized_end=11377
-  _STREAMCIRCLEREQUEST._serialized_start=12148
-  _STREAMCIRCLEREQUEST._serialized_end=12496
-  _STREAMCIRCLEREQUEST_TYPE._serialized_start=11353
-  _STREAMCIRCLEREQUEST_TYPE._serialized_end=11377
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12499
-  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12639
-  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12642
-  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12800
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12803
-  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=12943
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=12946
-  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13085
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13088
-  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13216
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13218
-  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13339
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13341
-  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13461
-  _STREAMWAITREQUEST._serialized_start=13463
-  _STREAMWAITREQUEST._serialized_end=13580
-  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13583
-  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13711
-  _STREAMEMPTYREQUEST._serialized_start=13713
-  _STREAMEMPTYREQUEST._serialized_end=13803
-  _STREAMGETAXESRESPONSE._serialized_start=13805
-  _STREAMGETAXESRESPONSE._serialized_end=13888
-  _STREAMGETMAXSPEEDREQUEST._serialized_start=13890
-  _STREAMGETMAXSPEEDREQUEST._serialized_end=14000
-  _STREAMSETMAXSPEEDREQUEST._serialized_start=14003
-  _STREAMSETMAXSPEEDREQUEST._serialized_end=14132
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14134
-  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14261
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14264
-  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14428
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14431
-  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14559
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14562
-  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14728
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14730
-  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14831
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14833
-  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=14887
-  _STREAMBUFFERERASEREQUEST._serialized_start=14889
-  _STREAMBUFFERERASEREQUEST._serialized_end=14985
-  _STREAMGENERICCOMMANDREQUEST._serialized_start=14987
-  _STREAMGENERICCOMMANDREQUEST._serialized_end=15103
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15105
-  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15224
-  _BINARYREPLYONLYEVENT._serialized_start=15226
-  _BINARYREPLYONLYEVENT._serialized_end=15325
-  _OPENBINARYINTERFACEREQUEST._serialized_start=15328
-  _OPENBINARYINTERFACEREQUEST._serialized_end=15515
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15517
-  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15622
-  _GENERICBINARYREQUEST._serialized_start=15625
-  _GENERICBINARYREQUEST._serialized_end=15755
-  _BINARYMESSAGE._serialized_start=15757
-  _BINARYMESSAGE._serialized_end=15827
-  _BINARYMESSAGECOLLECTION._serialized_start=15829
-  _BINARYMESSAGECOLLECTION._serialized_end=15911
-  _DEVICEEMPTYREQUEST._serialized_start=15913
-  _DEVICEEMPTYREQUEST._serialized_end=15971
-  _BINARYDEVICEIDENTITY._serialized_start=15974
-  _BINARYDEVICEIDENTITY._serialized_end=16319
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16270
-  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16319
-  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16322
-  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16475
-  _BINARYDEVICEHOMEREQUEST._serialized_start=16477
-  _BINARYDEVICEHOMEREQUEST._serialized_end=16571
-  _BINARYDEVICEMOVEREQUEST._serialized_start=16574
-  _BINARYDEVICEMOVEREQUEST._serialized_end=16792
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5721
-  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5758
-  _BINARYDEVICESTOPREQUEST._serialized_start=16794
-  _BINARYDEVICESTOPREQUEST._serialized_end=16888
-  _BINARYDEVICEDETECTREQUEST._serialized_start=16890
-  _BINARYDEVICEDETECTREQUEST._serialized_end=16965
-  _BINARYDEVICEDETECTRESPONSE._serialized_start=16967
-  _BINARYDEVICEDETECTRESPONSE._serialized_end=17012
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=17014
-  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17114
-  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17116
-  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17231
-  _CUSTOMINTERFACEREADREQUEST._serialized_start=17233
-  _CUSTOMINTERFACEREADREQUEST._serialized_end=17283
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17285
-  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17353
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17355
-  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17406
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17408
-  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17482
-  _CANSETSTATEREQUEST._serialized_start=17484
-  _CANSETSTATEREQUEST._serialized_end=17571
-  _CANSETSTATEAXISRESPONSE._serialized_start=17573
-  _CANSETSTATEAXISRESPONSE._serialized_end=17634
-  _CANSETSTATEDEVICERESPONSE._serialized_start=17636
-  _CANSETSTATEDEVICERESPONSE._serialized_end=17748
-  _SETSTATEREQUEST._serialized_start=17750
-  _SETSTATEREQUEST._serialized_end=17855
-  _SERVOTUNINGREQUEST._serialized_start=17857
-  _SERVOTUNINGREQUEST._serialized_end=17947
-  _SERVOTUNINGPARAM._serialized_start=17949
-  _SERVOTUNINGPARAM._serialized_end=17996
-  _PARAMSETINFO._serialized_start=17998
-  _PARAMSETINFO._serialized_end=18101
-  _SETSERVOTUNINGREQUEST._serialized_start=18104
-  _SETSERVOTUNINGREQUEST._serialized_end=18262
-  _LOADPARAMSET._serialized_start=18264
-  _LOADPARAMSET._serialized_end=18374
-  _SETSERVOTUNINGPIDREQUEST._serialized_start=18377
-  _SETSERVOTUNINGPIDREQUEST._serialized_end=18518
-  _PIDTUNING._serialized_start=18520
-  _PIDTUNING._serialized_end=18607
-  _SETSIMPLETUNING._serialized_start=18610
-  _SETSIMPLETUNING._serialized_end=18804
-  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18806
-  _SIMPLETUNINGPARAMDEFINITION._serialized_end=18906
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=18908
-  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=19017
-  _TRANSLATORCREATEREQUEST._serialized_start=19020
-  _TRANSLATORCREATEREQUEST._serialized_end=19169
-  _TRANSLATORCREATERESPONSE._serialized_start=19171
-  _TRANSLATORCREATERESPONSE._serialized_end=19220
-  _TRANSLATORAXISDEFINITION._serialized_start=19222
-  _TRANSLATORAXISDEFINITION._serialized_end=19301
-  _TRANSLATORDEFINITION._serialized_start=19304
-  _TRANSLATORDEFINITION._serialized_end=19465
-  _TRANSLATORCONFIG._serialized_start=19468
-  _TRANSLATORCONFIG._serialized_end=19640
-  _TRANSLATORAXISMAPPING._serialized_start=19642
-  _TRANSLATORAXISMAPPING._serialized_end=19706
-  _TRANSLATORAXISTRANSFORMATION._serialized_start=19708
-  _TRANSLATORAXISTRANSFORMATION._serialized_end=19834
-  _TRANSLATORTRANSLATEREQUEST._serialized_start=19836
-  _TRANSLATORTRANSLATEREQUEST._serialized_end=19902
-  _TRANSLATEMESSAGE._serialized_start=19904
-  _TRANSLATEMESSAGE._serialized_end=19977
-  _TRANSLATORTRANSLATERESPONSE._serialized_start=19979
-  _TRANSLATORTRANSLATERESPONSE._serialized_end=20086
-  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20088
-  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20152
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20154
-  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20221
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20223
-  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20299
-  _TRANSLATORFLUSHRESPONSE._serialized_start=20301
-  _TRANSLATORFLUSHRESPONSE._serialized_end=20344
-  _TRANSLATORCREATELIVEREQUEST._serialized_start=20347
-  _TRANSLATORCREATELIVEREQUEST._serialized_end=20491
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20494
-  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20639
-  _TRANSLATOREMPTYREQUEST._serialized_start=20641
-  _TRANSLATOREMPTYREQUEST._serialized_end=20688
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20690
-  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20784
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20786
-  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=20889
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=20891
-  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=20976
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=20978
-  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21088
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21090
-  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21172
-  _DEVICESETSTORAGEREQUEST._serialized_start=21174
-  _DEVICESETSTORAGEREQUEST._serialized_end=21295
-  _DEVICEGETSTORAGEREQUEST._serialized_start=21297
-  _DEVICEGETSTORAGEREQUEST._serialized_end=21403
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21405
-  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21516
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21518
-  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21627
-  _DEVICESTORAGEREQUEST._serialized_start=21629
-  _DEVICESTORAGEREQUEST._serialized_end=21716
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21718
-  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21816
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21819
-  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=21980
-  _CONVERSIONFACTOR._serialized_start=21982
-  _CONVERSIONFACTOR._serialized_end=22046
-  _OBJECTIVECHANGERREQUEST._serialized_start=22048
-  _OBJECTIVECHANGERREQUEST._serialized_end=22142
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22144
-  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22207
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22210
-  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22388
+  _DEVICEDETECTREQUEST._serialized_start=5118
+  _DEVICEDETECTREQUEST._serialized_end=5304
+  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_start=5259
+  _DEVICEDETECTREQUEST_DEVICETYPE._serialized_end=5304
+  _DEVICEDETECTRESPONSE._serialized_start=5306
+  _DEVICEDETECTRESPONSE._serialized_end=5345
+  _DEVICEHOMEREQUEST._serialized_start=5347
+  _DEVICEHOMEREQUEST._serialized_end=5443
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_start=5445
+  _DEVICEWAITUNTILIDLEREQUEST._serialized_end=5555
+  _DEVICEMOVEREQUEST._serialized_start=5558
+  _DEVICEMOVEREQUEST._serialized_end=5894
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_start=5839
+  _DEVICEMOVEREQUEST_MOVETYPE._serialized_end=5894
+  _DEVICESTOPREQUEST._serialized_start=5896
+  _DEVICESTOPREQUEST._serialized_end=5992
+  _DEVICEONALLREQUEST._serialized_start=5994
+  _DEVICEONALLREQUEST._serialized_end=6061
+  _DEVICEONALLRESPONSE._serialized_start=6063
+  _DEVICEONALLRESPONSE._serialized_end=6110
+  _DEVICEGETWARNINGSREQUEST._serialized_start=6112
+  _DEVICEGETWARNINGSREQUEST._serialized_end=6205
+  _DEVICEGETWARNINGSRESPONSE._serialized_start=6207
+  _DEVICEGETWARNINGSRESPONSE._serialized_end=6249
+  _WAITTOCLEARWARNINGSREQUEST._serialized_start=6251
+  _WAITTOCLEARWARNINGSREQUEST._serialized_end=6371
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_start=6373
+  _DEVICEGETALLDIGITALIOREQUEST._serialized_end=6463
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_start=6465
+  _DEVICEGETALLDIGITALIORESPONSE._serialized_end=6512
+  _DEVICEGETALLANALOGIOREQUEST._serialized_start=6514
+  _DEVICEGETALLANALOGIOREQUEST._serialized_end=6603
+  _DEVICEGETALLANALOGIORESPONSE._serialized_start=6605
+  _DEVICEGETALLANALOGIORESPONSE._serialized_end=6651
+  _DEVICEGETDIGITALIOREQUEST._serialized_start=6653
+  _DEVICEGETDIGITALIOREQUEST._serialized_end=6764
+  _DEVICEGETANALOGIOREQUEST._serialized_start=6766
+  _DEVICEGETANALOGIOREQUEST._serialized_end=6876
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_start=6878
+  _DEVICESETALLDIGITALOUTPUTSREQUEST._serialized_end=6967
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_start=6969
+  _DEVICESETALLANALOGOUTPUTSREQUEST._serialized_end=7057
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_start=7059
+  _DEVICESETDIGITALOUTPUTREQUEST._serialized_end=7167
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_start=7169
+  _DEVICESETANALOGOUTPUTREQUEST._serialized_end=7276
+  _SETLOGOUTPUTREQUEST._serialized_start=7278
+  _SETLOGOUTPUTREQUEST._serialized_end=7332
+  _DEVICEGETSETTINGREQUEST._serialized_start=7334
+  _DEVICEGETSETTINGREQUEST._serialized_end=7442
+  _DEVICECONVERTSETTINGREQUEST._serialized_start=7445
+  _DEVICECONVERTSETTINGREQUEST._serialized_end=7593
+  _DEVICESETSETTINGREQUEST._serialized_start=7595
+  _DEVICESETSETTINGREQUEST._serialized_end=7718
+  _DEVICESETSETTINGSTRREQUEST._serialized_start=7720
+  _DEVICESETSETTINGSTRREQUEST._serialized_end=7832
+  _PREPARECOMMANDREQUEST._serialized_start=7835
+  _PREPARECOMMANDREQUEST._serialized_end=7993
+  _WAITTORESPONDREQUEST._serialized_start=7995
+  _WAITTORESPONDREQUEST._serialized_end=8072
+  _LOCKSTEPENABLEREQUEST._serialized_start=8074
+  _LOCKSTEPENABLEREQUEST._serialized_end=8176
+  _LOCKSTEPDISABLEREQUEST._serialized_start=8178
+  _LOCKSTEPDISABLEREQUEST._serialized_end=8292
+  _LOCKSTEPSTOPREQUEST._serialized_start=8294
+  _LOCKSTEPSTOPREQUEST._serialized_end=8405
+  _LOCKSTEPHOMEREQUEST._serialized_start=8407
+  _LOCKSTEPHOMEREQUEST._serialized_end=8518
+  _LOCKSTEPMOVEREQUEST._serialized_start=8521
+  _LOCKSTEPMOVEREQUEST._serialized_end=8874
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_start=5839
+  _LOCKSTEPMOVEREQUEST_MOVETYPE._serialized_end=5894
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_start=8876
+  _LOCKSTEPWAITUNTILIDLEREQUEST._serialized_end=9001
+  _LOCKSTEPEMPTYREQUEST._serialized_start=9003
+  _LOCKSTEPEMPTYREQUEST._serialized_end=9090
+  _LOCKSTEPAXES._serialized_start=9092
+  _LOCKSTEPAXES._serialized_end=9170
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_start=9172
+  _LOCKSTEPGETAXISNUMBERSRESPONSE._serialized_end=9218
+  _LOCKSTEPGETREQUEST._serialized_start=9220
+  _LOCKSTEPGETREQUEST._serialized_end=9319
+  _LOCKSTEPSETREQUEST._serialized_start=9322
+  _LOCKSTEPSETREQUEST._serialized_end=9456
+  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_start=9458
+  _OSCILLOSCOPEADDSETTINGCHANNELREQUEST._serialized_end=9565
+  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_start=9567
+  _OSCILLOSCOPEADDIOCHANNELREQUEST._serialized_end=9675
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_start=9677
+  _OSCILLOSCOPESTARTSTOPREQUEST._serialized_end=9784
+  _OSCILLOSCOPEREADRESPONSE._serialized_start=9786
+  _OSCILLOSCOPEREADRESPONSE._serialized_end=9830
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_start=9832
+  _OSCILLOSCOPEDATAIDENTIFIER._serialized_end=9877
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_start=9879
+  _OSCILLOSCOPECAPTUREPROPERTIES._serialized_end=10006
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_start=10008
+  _OSCILLOSCOPEDATAGETREQUEST._serialized_end=10067
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_start=10069
+  _OSCILLOSCOPEDATAGETSAMPLETIMEREQUEST._serialized_end=10153
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_start=10155
+  _OSCILLOSCOPEDATAGETSAMPLESRESPONSE._serialized_end=10205
+  _STREAMSETUPLIVEREQUEST._serialized_start=10207
+  _STREAMSETUPLIVEREQUEST._serialized_end=10315
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_start=10318
+  _STREAMSETUPLIVECOMPOSITEREQUEST._serialized_end=10481
+  _STREAMSETUPSTOREREQUEST._serialized_start=10484
+  _STREAMSETUPSTOREREQUEST._serialized_end=10636
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_start=10639
+  _STREAMSETUPSTORECOMPOSITEREQUEST._serialized_end=10846
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_start=10849
+  _STREAMSETUPSTOREARBITRARYAXESREQUEST._serialized_end=11020
+  _STREAMCALLREQUEST._serialized_start=11023
+  _STREAMCALLREQUEST._serialized_end=11155
+  _PVTPOINTREQUEST._serialized_start=11158
+  _PVTPOINTREQUEST._serialized_end=11495
+  _PVTPOINTREQUEST_TYPE._serialized_start=11471
+  _PVTPOINTREQUEST_TYPE._serialized_end=11495
+  _STREAMLINEREQUEST._serialized_start=11498
+  _STREAMLINEREQUEST._serialized_end=11759
+  _STREAMLINEREQUEST_TYPE._serialized_start=11471
+  _STREAMLINEREQUEST_TYPE._serialized_end=11495
+  _STREAMARCREQUEST._serialized_start=11762
+  _STREAMARCREQUEST._serialized_end=12263
+  _STREAMARCREQUEST_TYPE._serialized_start=11471
+  _STREAMARCREQUEST_TYPE._serialized_end=11495
+  _STREAMCIRCLEREQUEST._serialized_start=12266
+  _STREAMCIRCLEREQUEST._serialized_end=12614
+  _STREAMCIRCLEREQUEST_TYPE._serialized_start=11471
+  _STREAMCIRCLEREQUEST_TYPE._serialized_end=11495
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_start=12617
+  _STREAMWAITDIGITALINPUTREQUEST._serialized_end=12757
+  _STREAMWAITANALOGINPUTREQUEST._serialized_start=12760
+  _STREAMWAITANALOGINPUTREQUEST._serialized_end=12918
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_start=12921
+  _STREAMSETDIGITALOUTPUTREQUEST._serialized_end=13061
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_start=13064
+  _STREAMSETANALOGOUTPUTREQUEST._serialized_end=13203
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_start=13206
+  _STREAMTOGGLEDIGITALOUTPUTREQUEST._serialized_end=13334
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_start=13336
+  _STREAMSETALLDIGITALOUTPUTSREQUEST._serialized_end=13457
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_start=13459
+  _STREAMSETALLANALOGOUTPUTSREQUEST._serialized_end=13579
+  _STREAMWAITREQUEST._serialized_start=13581
+  _STREAMWAITREQUEST._serialized_end=13698
+  _STREAMWAITUNTILIDLEREQUEST._serialized_start=13701
+  _STREAMWAITUNTILIDLEREQUEST._serialized_end=13829
+  _STREAMEMPTYREQUEST._serialized_start=13831
+  _STREAMEMPTYREQUEST._serialized_end=13921
+  _STREAMGETAXESRESPONSE._serialized_start=13923
+  _STREAMGETAXESRESPONSE._serialized_end=14006
+  _STREAMGETMAXSPEEDREQUEST._serialized_start=14008
+  _STREAMGETMAXSPEEDREQUEST._serialized_end=14118
+  _STREAMSETMAXSPEEDREQUEST._serialized_start=14121
+  _STREAMSETMAXSPEEDREQUEST._serialized_end=14250
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14252
+  _STREAMGETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14379
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_start=14382
+  _STREAMSETMAXTANGENTIALACCELERATIONREQUEST._serialized_end=14546
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14549
+  _STREAMGETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14677
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_start=14680
+  _STREAMSETMAXCENTRIPETALACCELERATIONREQUEST._serialized_end=14846
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_start=14848
+  _STREAMBUFFERGETCONTENTREQUEST._serialized_end=14949
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_start=14951
+  _STREAMBUFFERGETCONTENTRESPONSE._serialized_end=15005
+  _STREAMBUFFERERASEREQUEST._serialized_start=15007
+  _STREAMBUFFERERASEREQUEST._serialized_end=15103
+  _STREAMGENERICCOMMANDREQUEST._serialized_start=15105
+  _STREAMGENERICCOMMANDREQUEST._serialized_end=15221
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_start=15223
+  _STREAMGENERICCOMMANDBATCHREQUEST._serialized_end=15342
+  _BINARYREPLYONLYEVENT._serialized_start=15344
+  _BINARYREPLYONLYEVENT._serialized_end=15443
+  _OPENBINARYINTERFACEREQUEST._serialized_start=15446
+  _OPENBINARYINTERFACEREQUEST._serialized_end=15633
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_start=15635
+  _UNKNOWNBINARYRESPONSEEVENT._serialized_end=15740
+  _GENERICBINARYREQUEST._serialized_start=15743
+  _GENERICBINARYREQUEST._serialized_end=15873
+  _BINARYMESSAGE._serialized_start=15875
+  _BINARYMESSAGE._serialized_end=15945
+  _BINARYMESSAGECOLLECTION._serialized_start=15947
+  _BINARYMESSAGECOLLECTION._serialized_end=16029
+  _DEVICEEMPTYREQUEST._serialized_start=16031
+  _DEVICEEMPTYREQUEST._serialized_end=16089
+  _BINARYDEVICEIDENTITY._serialized_start=16092
+  _BINARYDEVICEIDENTITY._serialized_end=16437
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_start=16388
+  _BINARYDEVICEIDENTITY_DEVICETYPE._serialized_end=16437
+  _BINARYGENERICWITHUNITSREQUEST._serialized_start=16440
+  _BINARYGENERICWITHUNITSREQUEST._serialized_end=16593
+  _BINARYDEVICEHOMEREQUEST._serialized_start=16595
+  _BINARYDEVICEHOMEREQUEST._serialized_end=16689
+  _BINARYDEVICEMOVEREQUEST._serialized_start=16692
+  _BINARYDEVICEMOVEREQUEST._serialized_end=16910
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_start=5839
+  _BINARYDEVICEMOVEREQUEST_MOVETYPE._serialized_end=5876
+  _BINARYDEVICESTOPREQUEST._serialized_start=16912
+  _BINARYDEVICESTOPREQUEST._serialized_end=17006
+  _BINARYDEVICEDETECTREQUEST._serialized_start=17008
+  _BINARYDEVICEDETECTREQUEST._serialized_end=17083
+  _BINARYDEVICEDETECTRESPONSE._serialized_start=17085
+  _BINARYDEVICEDETECTRESPONSE._serialized_end=17130
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_start=17132
+  _BINARYDEVICEGETSETTINGREQUEST._serialized_end=17232
+  _BINARYDEVICESETSETTINGREQUEST._serialized_start=17234
+  _BINARYDEVICESETSETTINGREQUEST._serialized_end=17349
+  _CUSTOMINTERFACEREADREQUEST._serialized_start=17351
+  _CUSTOMINTERFACEREADREQUEST._serialized_end=17401
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_start=17403
+  _CUSTOMINTERFACEWRITEREQUEST._serialized_end=17471
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_start=17473
+  _CUSTOMINTERFACEOPENRESPONSE._serialized_end=17524
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_start=17526
+  _CUSTOMINTERFACECLOSEREQUEST._serialized_end=17600
+  _CANSETSTATEREQUEST._serialized_start=17602
+  _CANSETSTATEREQUEST._serialized_end=17689
+  _CANSETSTATEAXISRESPONSE._serialized_start=17691
+  _CANSETSTATEAXISRESPONSE._serialized_end=17752
+  _CANSETSTATEDEVICERESPONSE._serialized_start=17754
+  _CANSETSTATEDEVICERESPONSE._serialized_end=17866
+  _SETSTATEREQUEST._serialized_start=17868
+  _SETSTATEREQUEST._serialized_end=17973
+  _SERVOTUNINGREQUEST._serialized_start=17975
+  _SERVOTUNINGREQUEST._serialized_end=18065
+  _SERVOTUNINGPARAM._serialized_start=18067
+  _SERVOTUNINGPARAM._serialized_end=18114
+  _PARAMSETINFO._serialized_start=18116
+  _PARAMSETINFO._serialized_end=18219
+  _SETSERVOTUNINGREQUEST._serialized_start=18222
+  _SETSERVOTUNINGREQUEST._serialized_end=18380
+  _LOADPARAMSET._serialized_start=18382
+  _LOADPARAMSET._serialized_end=18492
+  _SETSERVOTUNINGPIDREQUEST._serialized_start=18495
+  _SETSERVOTUNINGPIDREQUEST._serialized_end=18636
+  _PIDTUNING._serialized_start=18638
+  _PIDTUNING._serialized_end=18725
+  _SETSIMPLETUNING._serialized_start=18728
+  _SETSIMPLETUNING._serialized_end=18922
+  _SIMPLETUNINGPARAMDEFINITION._serialized_start=18924
+  _SIMPLETUNINGPARAMDEFINITION._serialized_end=19024
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_start=19026
+  _GETSIMPLETUNINGPARAMDEFINITIONRESPONSE._serialized_end=19135
+  _TRANSLATORCREATEREQUEST._serialized_start=19138
+  _TRANSLATORCREATEREQUEST._serialized_end=19287
+  _TRANSLATORCREATERESPONSE._serialized_start=19289
+  _TRANSLATORCREATERESPONSE._serialized_end=19338
+  _TRANSLATORAXISDEFINITION._serialized_start=19340
+  _TRANSLATORAXISDEFINITION._serialized_end=19419
+  _TRANSLATORDEFINITION._serialized_start=19422
+  _TRANSLATORDEFINITION._serialized_end=19583
+  _TRANSLATORCONFIG._serialized_start=19586
+  _TRANSLATORCONFIG._serialized_end=19758
+  _TRANSLATORAXISMAPPING._serialized_start=19760
+  _TRANSLATORAXISMAPPING._serialized_end=19824
+  _TRANSLATORAXISTRANSFORMATION._serialized_start=19826
+  _TRANSLATORAXISTRANSFORMATION._serialized_end=19952
+  _TRANSLATORTRANSLATEREQUEST._serialized_start=19954
+  _TRANSLATORTRANSLATEREQUEST._serialized_end=20020
+  _TRANSLATEMESSAGE._serialized_start=20022
+  _TRANSLATEMESSAGE._serialized_end=20095
+  _TRANSLATORTRANSLATERESPONSE._serialized_start=20097
+  _TRANSLATORTRANSLATERESPONSE._serialized_end=20204
+  _GCODESYNTAXEXCEPTIONDATA._serialized_start=20206
+  _GCODESYNTAXEXCEPTIONDATA._serialized_end=20270
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_start=20272
+  _GCODEEXECUTIONEXCEPTIONDATA._serialized_end=20339
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_start=20341
+  _TRANSLATORFLUSHLIVEREQUEST._serialized_end=20417
+  _TRANSLATORFLUSHRESPONSE._serialized_start=20419
+  _TRANSLATORFLUSHRESPONSE._serialized_end=20462
+  _TRANSLATORCREATELIVEREQUEST._serialized_start=20465
+  _TRANSLATORCREATELIVEREQUEST._serialized_end=20609
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_start=20612
+  _TRANSLATORCREATEFROMDEVICEREQUEST._serialized_end=20757
+  _TRANSLATOREMPTYREQUEST._serialized_start=20759
+  _TRANSLATOREMPTYREQUEST._serialized_end=20806
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_start=20808
+  _TRANSLATORSETTRAVERSERATEREQUEST._serialized_end=20902
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_start=20904
+  _TRANSLATORSETAXISPOSITIONREQUEST._serialized_end=21007
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_start=21009
+  _TRANSLATORGETAXISPOSITIONREQUEST._serialized_end=21094
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_start=21096
+  _TRANSLATORGETAXISOFFSETREQUEST._serialized_end=21206
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_start=21208
+  _TRANSLATORSETFEEDRATEOVERRIDEREQUEST._serialized_end=21290
+  _DEVICESETSTORAGEREQUEST._serialized_start=21292
+  _DEVICESETSTORAGEREQUEST._serialized_end=21413
+  _DEVICEGETSTORAGEREQUEST._serialized_start=21415
+  _DEVICEGETSTORAGEREQUEST._serialized_end=21521
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_start=21523
+  _DEVICESETSTORAGENUMBERREQUEST._serialized_end=21634
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_start=21636
+  _DEVICESETSTORAGEBOOLREQUEST._serialized_end=21745
+  _DEVICESTORAGEREQUEST._serialized_start=21747
+  _DEVICESTORAGEREQUEST._serialized_end=21834
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_start=21836
+  _DEVICESTORAGELISTKEYSREQUEST._serialized_end=21934
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_start=21937
+  _DEVICESETUNITCONVERSIONSREQUEST._serialized_end=22098
+  _CONVERSIONFACTOR._serialized_start=22100
+  _CONVERSIONFACTOR._serialized_end=22164
+  _OBJECTIVECHANGERREQUEST._serialized_start=22166
+  _OBJECTIVECHANGERREQUEST._serialized_end=22260
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_start=22262
+  _OBJECTIVECHANGERCREATERESPONSE._serialized_end=22325
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_start=22328
+  _OBJECTIVECHANGERCHANGEREQUEST._serialized_end=22506
+  _PROCESSON._serialized_start=22508
+  _PROCESSON._serialized_end=22601
+  _PROCESSCONTROLLERSOURCE._serialized_start=22603
+  _PROCESSCONTROLLERSOURCE._serialized_end=22658
+  _SETPROCESSCONTROLLERSOURCE._serialized_start=22661
+  _SETPROCESSCONTROLLERSOURCE._serialized_end=22806
 # @@protoc_insertion_point(module_scope)
```

### Comparing `zaber_motion-4.2.0/zaber_motion/protobufs/main_pb2.pyi` & `zaber_motion-4.2.1/zaber_motion/protobufs/main_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1431,25 +1431,41 @@
 
 @typing_extensions.final
 class DeviceDetectRequest(google.protobuf.message.Message):
     """device/detect"""
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    class _DeviceType:
+        ValueType = typing.NewType("ValueType", builtins.int)
+        V: typing_extensions.TypeAlias = ValueType
+
+    class _DeviceTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[DeviceDetectRequest._DeviceType.ValueType], builtins.type):  # noqa: F821
+        DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+        ANY: DeviceDetectRequest._DeviceType.ValueType  # 0
+        PROCESS_CONTROLLER: DeviceDetectRequest._DeviceType.ValueType  # 1
+
+    class DeviceType(_DeviceType, metaclass=_DeviceTypeEnumTypeWrapper): ...
+    ANY: DeviceDetectRequest.DeviceType.ValueType  # 0
+    PROCESS_CONTROLLER: DeviceDetectRequest.DeviceType.ValueType  # 1
+
     INTERFACE_ID_FIELD_NUMBER: builtins.int
     IDENTIFY_DEVICES_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
     interface_id: builtins.int
     identify_devices: builtins.bool
+    type: global___DeviceDetectRequest.DeviceType.ValueType
     def __init__(
         self,
         *,
         interface_id: builtins.int = ...,
         identify_devices: builtins.bool = ...,
+        type: global___DeviceDetectRequest.DeviceType.ValueType = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["identify_devices", b"identify_devices", "interface_id", b"interface_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["identify_devices", b"identify_devices", "interface_id", b"interface_id", "type", b"type"]) -> None: ...
 
 global___DeviceDetectRequest = DeviceDetectRequest
 
 @typing_extensions.final
 class DeviceDetectResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -5397,7 +5413,89 @@
         objective: builtins.int = ...,
         focus_offset: global___Measurement | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["focus_offset", b"focus_offset"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["focus_address", b"focus_address", "focus_offset", b"focus_offset", "interface_id", b"interface_id", "objective", b"objective", "turret_address", b"turret_address"]) -> None: ...
 
 global___ObjectiveChangerChangeRequest = ObjectiveChangerChangeRequest
+
+@typing_extensions.final
+class ProcessOn(google.protobuf.message.Message):
+    """Process Controller
+
+    process-controller/enable
+    process-controller/on
+    process_controller/bridge
+    """
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    AXIS_FIELD_NUMBER: builtins.int
+    ON_FIELD_NUMBER: builtins.int
+    DURATION_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    axis: builtins.int
+    on: builtins.bool
+    duration: builtins.float
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        axis: builtins.int = ...,
+        on: builtins.bool = ...,
+        duration: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axis", b"axis", "device", b"device", "duration", b"duration", "interface_id", b"interface_id", "on", b"on"]) -> None: ...
+
+global___ProcessOn = ProcessOn
+
+@typing_extensions.final
+class ProcessControllerSource(google.protobuf.message.Message):
+    """process_controller/get_source"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    SENSOR_FIELD_NUMBER: builtins.int
+    PORT_FIELD_NUMBER: builtins.int
+    sensor: builtins.int
+    port: builtins.int
+    def __init__(
+        self,
+        *,
+        sensor: builtins.int = ...,
+        port: builtins.int = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["port", b"port", "sensor", b"sensor"]) -> None: ...
+
+global___ProcessControllerSource = ProcessControllerSource
+
+@typing_extensions.final
+class SetProcessControllerSource(google.protobuf.message.Message):
+    """process_controller/set_source"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INTERFACE_ID_FIELD_NUMBER: builtins.int
+    DEVICE_FIELD_NUMBER: builtins.int
+    AXIS_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    interface_id: builtins.int
+    device: builtins.int
+    axis: builtins.int
+    @property
+    def source(self) -> global___ProcessControllerSource: ...
+    def __init__(
+        self,
+        *,
+        interface_id: builtins.int = ...,
+        device: builtins.int = ...,
+        axis: builtins.int = ...,
+        source: global___ProcessControllerSource | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["source", b"source"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["axis", b"axis", "device", b"device", "interface_id", b"interface_id", "source", b"source"]) -> None: ...
+
+global___SetProcessControllerSource = SetProcessControllerSource
```

### Comparing `zaber_motion-4.2.0/zaber_motion/serialization.py` & `zaber_motion-4.2.1/zaber_motion/serialization.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/tools.py` & `zaber_motion-4.2.1/zaber_motion/tools.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion/units.py` & `zaber_motion-4.2.1/zaber_motion/units.py`

 * *Files identical despite different names*

### Comparing `zaber_motion-4.2.0/zaber_motion.egg-info/PKG-INFO` & `zaber_motion-4.2.1/zaber_motion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaber-motion
-Version: 4.2.0
+Version: 4.2.1
 Summary: A library for communicating with Zaber devices
 Home-page: https://gitlab.com/ZaberTech/zaber-motion-lib
 Author: Zaber Technologies Inc.
 Author-email: contact@zaber.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `zaber_motion-4.2.0/zaber_motion.egg-info/SOURCES.txt` & `zaber_motion-4.2.1/zaber_motion.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 zaber_motion/ascii/message_type.py
 zaber_motion/ascii/oscilloscope.py
 zaber_motion/ascii/oscilloscope_capture_properties.py
 zaber_motion/ascii/oscilloscope_data.py
 zaber_motion/ascii/oscilloscope_data_source.py
 zaber_motion/ascii/paramset_info.py
 zaber_motion/ascii/pid_tuning.py
+zaber_motion/ascii/process.py
+zaber_motion/ascii/process_controller.py
+zaber_motion/ascii/process_controller_mode.py
+zaber_motion/ascii/process_controller_source.py
+zaber_motion/ascii/process_controller_source_sensor.py
 zaber_motion/ascii/pvt_axis_definition.py
 zaber_motion/ascii/pvt_axis_type.py
 zaber_motion/ascii/pvt_buffer.py
 zaber_motion/ascii/pvt_mode.py
 zaber_motion/ascii/pvt_sequence.py
 zaber_motion/ascii/response.py
 zaber_motion/ascii/servo_tuner.py
```

