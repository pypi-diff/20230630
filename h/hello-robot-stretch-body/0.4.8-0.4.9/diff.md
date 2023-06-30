# Comparing `tmp/hello_robot_stretch_body-0.4.8.tar.gz` & `tmp/hello_robot_stretch_body-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hello_robot_stretch_body-0.4.8.tar", last modified: Mon Sep 12 17:09:44 2022, max compression
+gzip compressed data, was "hello_robot_stretch_body-0.4.9.tar", last modified: Fri Sep 23 17:39:06 2022, max compression
```

## Comparing `hello_robot_stretch_body-0.4.8.tar` & `hello_robot_stretch_body-0.4.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-12 17:09:44.472120 hello_robot_stretch_body-0.4.8/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      916 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/LICENSE.md
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2412 2022-09-12 17:09:44.472120 hello_robot_stretch_body-0.4.8/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1937 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/README.md
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-12 17:09:44.464120 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2412 2022-09-12 17:09:44.000000 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/PKG-INFO
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1637 2022-09-12 17:09:44.000000 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/SOURCES.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2022-09-12 17:09:44.000000 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/dependency_links.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      514 2022-09-12 17:09:44.000000 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/requires.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2022-09-12 17:09:44.000000 hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/top_level.txt
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2022-09-12 17:09:44.472120 hello_robot_stretch_body-0.4.8/setup.cfg
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1912 2022-09-12 17:04:14.000000 hello_robot_stretch_body-0.4.8/setup.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-12 17:09:44.468120 hello_robot_stretch_body-0.4.8/stretch_body/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      948 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    33711 2022-09-07 19:18:50.000000 hello_robot_stretch_body-0.4.8/stretch_body/base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3996 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/cobbs_framing.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5518 2022-09-07 19:18:50.000000 hello_robot_stretch_body-0.4.8/stretch_body/device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    36111 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    10775 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_X_chain.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    39292 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3528 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      571 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2929 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21149 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/stretch_body/hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1000 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27808 2022-08-29 23:43:09.000000 hello_robot_stretch_body-0.4.8/stretch_body/pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26762 2022-09-07 19:18:50.000000 hello_robot_stretch_body-0.4.8/stretch_body/prismatic_joint.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14301 2022-08-29 23:43:09.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8433 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_collision.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6479 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_collision_models.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6859 2022-08-29 23:43:09.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_monitor.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6736 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    25176 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_params_RE1V0.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    18715 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/stretch_body/robot_params_RE2V0.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11660 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/scope.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    49692 2022-09-07 19:18:50.000000 hello_robot_stretch_body-0.4.8/stretch_body/stepper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3814 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    28383 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    13897 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/transport.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      213 2022-09-12 17:03:05.000000 hello_robot_stretch_body-0.4.8/stretch_body/version.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12090 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/wacc.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1919 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/stretch_body/wrist_yaw.py
--rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9733 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/stretch_body/xbox_controller.py
-drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-12 17:09:44.472120 hello_robot_stretch_body-0.4.8/test/
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/__init__.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/test/test_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6818 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/test/test_base.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_collisions.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3196 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/test/test_device.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_dxl_comms.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_dynamixel_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2022-09-09 21:57:04.000000 hello_robot_stretch_body-0.4.8/test/test_dynamixel_hello_XL430.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_end_of_arm.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_end_of_arm_tools.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/test/test_head.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21963 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_hello_utils.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_lift.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_pimu.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9004 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/test/test_robot.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_robot_params.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_steppers.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_stretch_gripper.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_sync.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_timing_stats.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2022-07-06 22:59:31.000000 hello_robot_stretch_body-0.4.8/test/test_trajectories.py
--rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2022-08-26 18:26:17.000000 hello_robot_stretch_body-0.4.8/test/test_wrist_yaw.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      916 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/LICENSE.md
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2449 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1937 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/README.md
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.552698 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2449 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/PKG-INFO
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1637 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/SOURCES.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        1 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/dependency_links.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      553 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/requires.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       18 2022-09-23 17:39:06.000000 hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/top_level.txt
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       38 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/setup.cfg
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2035 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/setup.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.556697 hello_robot_stretch_body-0.4.9/stretch_body/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)       34 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      948 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    33711 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3996 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/cobbs_framing.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5518 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    36111 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    10775 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_X_chain.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    39292 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3528 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      571 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm_tools.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2929 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21149 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1000 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    27808 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26762 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/prismatic_joint.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14301 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     8433 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_collision.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6479 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_collision_models.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6869 2022-09-23 16:03:21.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_monitor.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6929 2022-09-23 17:19:29.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    25176 2022-09-23 17:09:48.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE1V0.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    18715 2022-09-23 17:06:19.000000 hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE2V0.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)    11660 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/scope.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    49692 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/stepper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3814 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    28383 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    13897 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/transport.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)      213 2022-09-23 17:38:49.000000 hello_robot_stretch_body-0.4.9/stretch_body/version.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    12090 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/wacc.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1919 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/wrist_yaw.py
+-rwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)     9733 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/stretch_body/xbox_controller.py
+drwxrwxr-x   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 17:39:06.560696 hello_robot_stretch_body-0.4.9/test/
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)        0 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/__init__.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     5384 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6818 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_base.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9977 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_collisions.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3198 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_device.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1111 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dxl_comms.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     7882 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dynamixel_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    14520 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_dynamixel_hello_XL430.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1435 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_end_of_arm.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1914 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_end_of_arm_tools.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3833 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_head.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    21963 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_hello_utils.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4761 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_lift.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2069 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_pimu.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     9004 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_robot.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     2391 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_robot_params.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    26117 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_steppers.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     1657 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_stretch_gripper.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     6263 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_sync.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     4381 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_timing_stats.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)    29747 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_trajectories.py
+-rw-rw-r--   0 hello-robot  (1000) hello-robot  (1000)     3918 2022-09-23 15:47:39.000000 hello_robot_stretch_body-0.4.9/test/test_wrist_yaw.py
```

### Comparing `hello_robot_stretch_body-0.4.8/LICENSE.md` & `hello_robot_stretch_body-0.4.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/PKG-INFO` & `hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: hello_robot_stretch_body
-Version: 0.4.8
+Name: hello-robot-stretch-body
+Version: 0.4.9
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Stretch Body
@@ -67,7 +69,9 @@
 
 Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
 
 Deploying
 ---------
 
 Increment the version number and run the `deploy.sh` script.
+
+
```

### Comparing `hello_robot_stretch_body-0.4.8/README.md` & `hello_robot_stretch_body-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/PKG-INFO` & `hello_robot_stretch_body-0.4.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: hello-robot-stretch-body
-Version: 0.4.8
+Name: hello_robot_stretch_body
+Version: 0.4.9
 Summary: Stretch Body low level Python API
 Home-page: https://github.com/hello-robot/stretch_body
 Author: Hello Robot Inc.
 Author-email: support@hello-robot.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 Stretch Body
@@ -67,7 +69,9 @@
 
 Now, make desired edits to the [stretch_body/body/stretch_body/robot.py](./stretch_body/robot.py) file. Software using Stretch Body is now using the modified `stretch_body.robot.Robot` class.
 
 Deploying
 ---------
 
 Increment the version number and run the `deploy.sh` script.
+
+
```

### Comparing `hello_robot_stretch_body-0.4.8/hello_robot_stretch_body.egg-info/SOURCES.txt` & `hello_robot_stretch_body-0.4.9/hello_robot_stretch_body.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/setup.py` & `hello_robot_stretch_body-0.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,20 @@
     classifiers=[
         "Programming Language :: Python :: 2",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
     ],
     install_requires=['numpy', 'scipy', 'matplotlib', 'ipython', 'pandas', 'sympy', 'nose',
                       'inputs', 'drawnow', 'rplidar-roboticia', 'snakeviz', 'pyusb', 'SpeechRecognition', 'pixel-ring',
-                      'click', 'cma', 'opencv-contrib-python', 'colorama',
+                      'click', 'cma', 'colorama',
                       'scikit-image', 'open3d', 'pyrealsense2', 'pathlib', 'psutil', 'gitpython', 'urdfpy',
+                      'opencv-contrib-python', 'renamed-opencv-python-inference-engine; python_version >= "3.0.0"', # resolve cv2 conflict for py3
                       'jsonschema==2.6.0; python_version < "3.0"', 'qtconsole==4.7.7; python_version < "3.0"', 'jupyter', # required by juypter
                       'llvmlite==0.31.0; python_version < "3.0"', 'numba', # numba required by stretch_funmap, depends on old llvmlite for py2
                       'terminado==0.8.3; python_version < "3.0"', # depend on old terminado for py2
                       'dynamixel-sdk>=3.1; python_version >= "3.0.0"', # py2 gets dynamixel-sdk through ROS
                       'pyyaml>=5.1', # required for yaml.FullLoader
                       'hello-robot-stretch-tool-share>=0.2.5', # defines other Stretch end effectors
                       'hello-robot-stretch-factory>=0.3.5','hello-robot-stretch-body-tools>=0.4.2'
+
                       ]
 )
```

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/arm.py` & `hello_robot_stretch_body-0.4.9/stretch_body/arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/base.py` & `hello_robot_stretch_body-0.4.9/stretch_body/base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/cobbs_framing.py` & `hello_robot_stretch_body-0.4.9/stretch_body/cobbs_framing.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/device.py` & `hello_robot_stretch_body-0.4.9/stretch_body/device.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_XL430.py` & `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_X_chain.py` & `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_X_chain.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.4.9/stretch_body/dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/end_of_arm.py` & `hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/end_of_arm_tools.py` & `hello_robot_stretch_body-0.4.9/stretch_body/end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/head.py` & `hello_robot_stretch_body-0.4.9/stretch_body/head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/hello_utils.py` & `hello_robot_stretch_body-0.4.9/stretch_body/hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/lift.py` & `hello_robot_stretch_body-0.4.9/stretch_body/lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/pimu.py` & `hello_robot_stretch_body-0.4.9/stretch_body/pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/prismatic_joint.py` & `hello_robot_stretch_body-0.4.9/stretch_body/prismatic_joint.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_collision.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_collision.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_collision_models.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_collision_models.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_monitor.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,49 +56,49 @@
             self.monitor_over_tilt_alert()
 
 
     # ##################################
     def monitor_base_cliff_event(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['cliff_event'] and  self.monitor_history['monitor_base_cliff_event']==0:
-                self.logger.info("Base cliff event")
+                self.logger.debug("Base cliff event")
             self.monitor_history['monitor_base_cliff_event'] = self.robot.pimu.status['cliff_event']
 
     # ##################################
     def monitor_base_bump_event(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['bump_event_cnt'] != self.monitor_history['monitor_base_bump_event']:
-                self.logger.info("Base bump event")
+                self.logger.debug("Base bump event")
             self.monitor_history['monitor_base_bump_event'] = self.robot.pimu.status['bump_event_cnt']
 
     # ##################################
     def monitor_over_tilt_alert(self):
         if self.robot.pimu is not None:
             if self.robot.pimu.status['over_tilt_alert'] and self.monitor_history['monitor_over_tilt_alert'] == 0:
-                self.logger.info("Over Tilt Alert")
+                self.logger.debug("Over Tilt Alert")
             self.monitor_history['monitor_over_tilt_alert'] = self.robot.pimu.status['over_tilt_alert']
 
     # ##################################
     def monitor_wrist_single_tap(self):
         if self.robot.wacc is not None:
             if self.robot.wacc.status['single_tap_count']!=self.monitor_history['monitor_wrist_single_tap']:
-                self.logger.info("Wrist single tap: %d" % self.robot.wacc.status['single_tap_count'])
+                self.logger.debug("Wrist single tap: %d" % self.robot.wacc.status['single_tap_count'])
             self.monitor_history['monitor_wrist_single_tap']=self.robot.wacc.status['single_tap_count']
 
     # ##################################
     def monitor_guarded_contact(self):
         joints=[self.robot.lift, self.robot.arm]
         mn='monitor_guarded_contact'
         for j in joints:
             if j is not None:
                 if j.name not in self.monitor_history[mn]:# Init history
                     self.monitor_history[mn][j.name] = 0
                 if j is not None:
                     if self.monitor_history[mn][j.name]==0 and j.motor.status['in_guarded_event']:
-                        self.logger.info("Guarded contact %s"%j.name)
+                        self.logger.debug("Guarded contact %s"%j.name)
                 self.monitor_history[mn][j.name] =j.motor.status['in_guarded_event']
 
     # ##################################
     def monitor_dynamixel_flags(self):
         chains=[self.robot.head,self.robot.end_of_arm]
         mn='monitor_dynamixel_flags'
         errs = ['overheating_error', 'overload_error']
@@ -111,38 +111,38 @@
                         self.monitor_history[mn][c.name][k] = {}
                         for e in errs:
                             self.monitor_history[mn][c.name][k][e]=0
                 #Flag changes from 0 to 1 on error
                 for k in c.motors.keys():
                     for e in errs:
                         if c.motors[k].status[e] and not self.monitor_history[mn][c.name][k][e]:
-                            self.logger.info("Dynamixel %s on %s:%s"%(e,c.name,k))
+                            self.logger.debug("Dynamixel %s on %s:%s"%(e,c.name,k))
                         self.monitor_history[mn][c.name][k][e] = c.motors[k].status[e]
 
     # ##################################
     def monitor_runstop(self):
         if self.robot.status['pimu']['runstop_event'] != self.monitor_history['monitor_runstop']:
             if self.robot.status['pimu']['runstop_event']:
-                self.logger.info("Runstop activated")
+                self.logger.debug("Runstop activated")
             else:
-                self.logger.info("Runstop deactivated")
+                self.logger.debug("Runstop deactivated")
         self.monitor_history['monitor_runstop']=self.robot.status['pimu']['runstop_event']
 
     # ##################################
     def monitor_voltage(self):
         v=self.robot.pimu.status['voltage']
         if v < self.robot.pimu.config['low_voltage_alert']:
             if v-self.monitor_history['monitor_voltage']<-0.5:#every 0.5V of drop allow to report
-                self.logger.info('Low voltage of: %.2f'%v)
+                self.logger.debug('Low voltage of: %.2f'%v)
                 self.monitor_history['monitor_voltage']=v
         else:
             self.monitor_history['monitor_voltage'] =v
 
     # ##################################
     def monitor_current(self):
         i=self.robot.pimu.status['current']
         if i > self.robot.pimu.config['high_current_alert']:
             if i-self.monitor_history['monitor_current']>0.25:#every 0.25A of rise allow to report
-                self.logger.info('High current of: %.2f'%i)
+                self.logger.debug('High current of: %.2f'%i)
                 self.monitor_history['monitor_current']=i
         else:
             self.monitor_history['monitor_current'] =i
```

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_params.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     else:
         _user_params = hello_utils.read_fleet_yaml('stretch_user_params.yaml')
         _config_params = hello_utils.read_fleet_yaml('stretch_configuration_params.yaml')
         _robot_params=nominal_system_params
         param_module_name = 'stretch_body.robot_params_'+_config_params['robot']['model_name']
         _nominal_params = getattr(importlib.import_module(param_module_name), 'nominal_params')
         hello_utils.overwrite_dict(_robot_params, _nominal_params)
+        for external_params_module in _config_params.get('params', []):
+            hello_utils.overwrite_dict(_robot_params,getattr(importlib.import_module(external_params_module), 'params'))
         for external_params_module in _user_params.get('params', []):
             hello_utils.overwrite_dict(_robot_params,getattr(importlib.import_module(external_params_module), 'params'))
         hello_utils.overwrite_dict(_robot_params, _config_params)
         hello_utils.overwrite_dict(_robot_params, _user_params)
         _valid_params=True
 
     @classmethod
```

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_params_RE1V0.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE1V0.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             'i_safety_feedforward': 0.4,
             'pKd_d': 20.0,
             'pKi_d': 0.05,
             'pKi_limit': 100.0,
             'pKp_d': 10.0,
             'pLPF': 60,
             'phase_advance_d': 1.8,
-            'pos_near_setpoint_d': 4.0,
+            'pos_near_setpoint_d': 6.0,
             'safety_hold': 1,
             'safety_stiffness': 0.0,
             'vKd_d': 0,
             'vKi_d': 0.005,
             'vKi_limit': 200,
             'vKp_d': 0.2,
             'vLPF': 30,
```

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/robot_params_RE2V0.py` & `hello_robot_stretch_body-0.4.9/stretch_body/robot_params_RE2V0.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 configuration_params_header='#Parameters that are specific to this robot\n' \
                             '#Do not edit, instead edit stretch_user_params.yaml\n'
 
 configuration_params_template={
     'arm':{
         'contact_models':{
             'effort_pct':{
-                'contact_thresh_default':[-45.0, 45.0],
-                'contact_thresh_homing':[-45.0, 45.0]}},
+                'contact_thresh_default':[-55.0, 55.0],
+                'contact_thresh_homing':[-55.0, 55.0]}},
         'range_m':[0.0,0.52]},
     'lift': {
         'contact_models':{
             'effort_pct': {
-                'contact_thresh_default': [-69.0, 69.0],
-                'contact_thresh_homing': [-69.0, 69.0]}},
+                'contact_thresh_default': [-10.0, 69.0],
+                'contact_thresh_homing': [-10.0, 69.0]}},
         'i_feedforward': 1.2,
         'range_m': [0.0, 1.10]},
     'base':{
         'wheel_separation_m': 0.3153},
     'head_pan':{
         'range_t': [0, 3827],
         'zero_t': 1250},
@@ -319,15 +319,15 @@
             'i_safety_feedforward': 1.2,
             'pKd_d': 25.0,
             'pKi_d': 0.05,
             'pKi_limit': 100.0,
             'pKp_d': 6.0,
             'pLPF': 100,
             'phase_advance_d': 1.8,
-            'pos_near_setpoint_d': 4.0,
+            'pos_near_setpoint_d': 6.0,
             'safety_hold': 1,
             'safety_stiffness': 0.0,
             'vKd_d': 0,
             'vKi_d': 0.005,
             'vKi_limit': 200,
             'vKp_d': 0.2,
             'vLPF': 30,
```

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/scope.py` & `hello_robot_stretch_body-0.4.9/stretch_body/scope.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/stepper.py` & `hello_robot_stretch_body-0.4.9/stretch_body/stepper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/stretch_gripper.py` & `hello_robot_stretch_body-0.4.9/stretch_body/stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/trajectories.py` & `hello_robot_stretch_body-0.4.9/stretch_body/trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/transport.py` & `hello_robot_stretch_body-0.4.9/stretch_body/transport.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/wacc.py` & `hello_robot_stretch_body-0.4.9/stretch_body/wacc.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/wrist_yaw.py` & `hello_robot_stretch_body-0.4.9/stretch_body/wrist_yaw.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/stretch_body/xbox_controller.py` & `hello_robot_stretch_body-0.4.9/stretch_body/xbox_controller.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_arm.py` & `hello_robot_stretch_body-0.4.9/test/test_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_base.py` & `hello_robot_stretch_body-0.4.9/test/test_base.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_collisions.py` & `hello_robot_stretch_body-0.4.9/test/test_collisions.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_device.py` & `hello_robot_stretch_body-0.4.9/test/test_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 class TestDevice(unittest.TestCase):
 
 
     def test_write_configuration_params(self):
         """
         Check that we don't mangle the format when writing config params to YAML
         """
+
         print('\nUnittest: test_write_configuration_params')
+
         d=stretch_body.device.Device(req_params=False)
         cp = stretch_body.hello_utils.read_fleet_yaml('stretch_configuration_params.yaml')
         for k in cp.keys(): #Write existing values up to 3 dict layers deep
             key1=k
             d.write_configuration_param_to_YAML(key1,cp[k])
             if type(cp[k]) is dict:
                 for j in cp[k].keys():
```

### Comparing `hello_robot_stretch_body-0.4.8/test/test_dxl_comms.py` & `hello_robot_stretch_body-0.4.9/test/test_dxl_comms.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_dynamixel_XL430.py` & `hello_robot_stretch_body-0.4.9/test/test_dynamixel_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_dynamixel_hello_XL430.py` & `hello_robot_stretch_body-0.4.9/test/test_dynamixel_hello_XL430.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_end_of_arm.py` & `hello_robot_stretch_body-0.4.9/test/test_end_of_arm.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_end_of_arm_tools.py` & `hello_robot_stretch_body-0.4.9/test/test_end_of_arm_tools.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_head.py` & `hello_robot_stretch_body-0.4.9/test/test_head.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_hello_utils.py` & `hello_robot_stretch_body-0.4.9/test/test_hello_utils.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_lift.py` & `hello_robot_stretch_body-0.4.9/test/test_lift.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_pimu.py` & `hello_robot_stretch_body-0.4.9/test/test_pimu.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_robot.py` & `hello_robot_stretch_body-0.4.9/test/test_robot.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_robot_params.py` & `hello_robot_stretch_body-0.4.9/test/test_robot_params.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_steppers.py` & `hello_robot_stretch_body-0.4.9/test/test_steppers.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_stretch_gripper.py` & `hello_robot_stretch_body-0.4.9/test/test_stretch_gripper.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_sync.py` & `hello_robot_stretch_body-0.4.9/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_timing_stats.py` & `hello_robot_stretch_body-0.4.9/test/test_timing_stats.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_trajectories.py` & `hello_robot_stretch_body-0.4.9/test/test_trajectories.py`

 * *Files identical despite different names*

### Comparing `hello_robot_stretch_body-0.4.8/test/test_wrist_yaw.py` & `hello_robot_stretch_body-0.4.9/test/test_wrist_yaw.py`

 * *Files identical despite different names*

