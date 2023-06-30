# Comparing `tmp/ht_pricing_module-0.2.5.tar.gz` & `tmp/ht_pricing_module-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.2.5.tar", last modified: Wed Jun  7 09:52:41 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.2.6.tar", last modified: Fri Jun 30 00:15:25 2023, max compression
```

## Comparing `ht_pricing_module-0.2.5.tar` & `ht_pricing_module-0.2.6.tar`

### file list

```diff
@@ -1,108 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.679877 ht_pricing_module-0.2.5/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0      263 2023-06-07 09:52:41.679877 ht_pricing_module-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-07 09:52:23.000000 ht_pricing_module-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.227616 ht_pricing_module-0.2.5/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.5/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.258534 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      258 2023-05-18 02:19:46.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      468 2023-05-29 08:11:33.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.273493 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.216646 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.296432 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.315382 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    47780 2023-05-31 11:41:37.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-05-16 06:25:50.000000 ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.329492 ht_pricing_module-0.2.5/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.5/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.340554 ht_pricing_module-0.2.5/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.5/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.353352 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.364361 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.380502 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.498188 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5561 2023-06-07 09:46:05.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
--rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.506166 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.538081 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.565009 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.592965 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.613909 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.616901 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     5680 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.628869 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3902 2023-06-05 06:56:38.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.631861 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       95 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     5712 2023-05-31 11:47:11.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
--rw-rw-rw-   0        0        0     6593 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.640837 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.660929 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.667909 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    45285 2023-06-01 06:53:57.000000 ht_pricing_module-0.2.5/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:52:41.241579 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      263 2023-06-07 09:52:41.000000 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5035 2023-06-07 09:52:41.000000 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:52:41.000000 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-07 09:52:41.000000 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-07 09:52:41.000000 ht_pricing_module-0.2.5/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 09:52:41.679877 ht_pricing_module-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-06-07 09:52:16.000000 ht_pricing_module-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.191319 ht_pricing_module-0.2.6/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      263 2023-06-30 00:15:25.190323 ht_pricing_module-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-06-29 02:23:41.000000 ht_pricing_module-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.040725 ht_pricing_module-0.2.6/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.6/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.065656 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      293 2023-06-27 10:58:01.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      558 2023-06-13 01:59:48.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.082610 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.025762 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.085605 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.089595 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    48559 2023-06-29 01:54:18.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3707 2023-06-27 10:58:01.000000 ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.098593 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0      234 2023-06-27 10:54:41.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     2070 2023-06-16 01:17:54.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
+-rw-rw-rw-   0        0        0     1007 2023-06-16 01:16:24.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
+-rw-rw-rw-   0        0        0     8078 2023-06-29 14:15:51.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
+-rw-rw-rw-   0        0        0     5329 2023-06-27 10:17:12.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+-rw-rw-rw-   0        0        0      693 2023-06-16 01:17:54.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/fully_explicit_european.py
+-rw-rw-rw-   0        0        0      736 2023-06-16 01:17:54.000000 ht_pricing_module-0.2.6/ht_pricing_module/finite_difference_engine/fully_implicit_european.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.101562 ht_pricing_module-0.2.6/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-06-19 06:14:01.000000 ht_pricing_module-0.2.6/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.104553 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.107544 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.112530 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.128488 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5561 2023-06-07 10:16:58.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.130482 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.134473 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.148434 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-06-27 02:32:08.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     2393 2023-06-26 13:08:59.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
+-rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     2263 2023-06-26 13:08:59.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
+-rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     2963 2023-06-26 13:12:34.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
+-rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+-rw-rw-rw-   0        0        0     3503 2023-06-26 13:08:59.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.153421 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.158407 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.160402 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     5693 2023-06-27 10:58:01.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.164392 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3902 2023-06-05 06:56:38.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.173373 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0      194 2023-06-27 11:31:24.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     5753 2023-06-28 02:47:53.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+-rw-rw-rw-   0        0        0     5075 2023-06-29 14:30:14.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
+-rw-rw-rw-   0        0        0     6870 2023-06-28 09:02:37.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+-rw-rw-rw-   0        0        0     6930 2023-06-29 11:03:38.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
+-rw-rw-rw-   0        0        0     4852 2023-06-29 13:27:41.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.176360 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.183341 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-06-27 02:30:19.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     3801 2023-06-26 13:08:59.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
+-rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     3157 2023-06-26 01:22:55.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.188328 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-06-13 02:30:48.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    45943 2023-06-28 09:02:37.000000 ht_pricing_module-0.2.6/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-06-30 00:15:25.060669 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-06-30 00:15:24.000000 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6098 2023-06-30 00:15:25.000000 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 00:15:24.000000 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 00:15:24.000000 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 00:15:24.000000 ht_pricing_module-0.2.6/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 00:15:25.191319 ht_pricing_module-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1158 2023-06-29 02:23:07.000000 ht_pricing_module-0.2.6/setup.py
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,16 @@
     FIXED_ACC_BARRIER_ENHANCED_AS       = 32;
     LINEAR_ACC_FIXED_ENHANCED_AS        = 33;
     DISCRETE_BINARY_MC                  = 34;
     LINEAR_ACC_FUSING_AS                = 35;
 
     QUOTIENT_AS                         = 36;
     SNOWBALL_DISCOUNTED_MC              = 37;
+    SNOWBALL_PDE                        = 38;
+    SNOWBALL_DISCOUNTED_PDE             = 39;
 }
 
 message PricerReply {
     PriceType price_type                = 1;
     double result                       = 2;
 }
 
@@ -157,22 +159,38 @@
         int32 index                             = 1;
         PricerType pricer_type                  = 2;
         google.protobuf.Any pricer_request      = 3;
     }
     repeated RequestItem batch_pricer_request   = 1;
 }
 
+message BatchPdePricerRequest {
+    message RequestItem {
+        google.protobuf.Any pricer_request      = 1;
+    }
+    PricerType pricer_type                      = 1;
+    google.protobuf.Any param                   = 2;
+    repeated RequestItem batch_pricer_request   = 3;
+}
+
 message BatchPricerReply {
     message ReplyItem {
         int32 index                             = 1;
         PricerReply pricer_reply                = 2;
     }
     repeated ReplyItem batch_pricer_reply       = 1;
 }
 
+message BatchPdePricerReply {
+    message ReplyItem {
+        PricerReply pricer_reply                = 1;
+    }
+    repeated ReplyItem batch_pricer_reply       = 1;
+}
+
 // ACCUMULATOR
 message FixedAccAkoRequest {
     PriceType price_type                = 1;
     FixedAccAko param                   = 2;
 }
 
 message FixedAccAko {
@@ -758,20 +776,20 @@
     double riskfree_rate                = 9; //无风险利率
     double dividend                     = 10; //分红率
     repeated PayoffObservation obs_date = 11; // 观察日序列
     int32 year_base                     = 12;
 }
 
 // SNOWBALL
-message SnowballMcRequest {
+message SnowballRequest {
     PriceType price_type                = 1;
-    SnowballMc param                    = 2;
+    Snowball param                      = 2;
 }
 
-message SnowballMc {
+message Snowball {
     double notional                                 = 1; // 单位数量名义金额
     double spot_price                               = 2; // 当前价
     double entrance_price                           = 3; // 入场价
     double knock_in_barrier_price                   = 4; // 敲入价
     double knock_out_barrier_price                  = 5; // 敲出价
     int32 expiry_date                               = 6; // 到日期
     double floor_rate                               = 7; // 保底比例
@@ -783,23 +801,24 @@
     double volatility                               = 13; // 波动率
     double riskfree_rate                            = 14; // 无风险利率
     double dividend                                 = 15; // 分红率
     int32 year_base                                 = 16;
     repeated KnockObservation knock_in_obs_date     = 17; // 敲入观察序列
     repeated KnockObservation knock_out_obs_date    = 18; // 敲出观察序列
     double participation_rate                       = 19;
+    double knock_in_strike_price                    = 20;
 }
 
 // SNOWBALL_DISCOUNTED
-message SnowballDiscountedMcRequest {
+message SnowballDiscountedRequest {
     PriceType price_type                = 1;
-    SnowballDiscountedMc param          = 2;
+    SnowballDiscounted param          = 2;
 }
 
-message SnowballDiscountedMc {
+message SnowballDiscounted {
     double notional                                 = 1; // 单位数量名义金额
     double spot_price                               = 2; // 当前价
     double entrance_price                           = 3; // 入场价
     double knock_in_barrier_price                   = 4; // 敲入价
     double knock_out_barrier_price                  = 5; // 敲出价
     int32 expiry_date                               = 6; // 到日期
     double floor_rate                               = 7; // 保底比例
@@ -997,14 +1016,20 @@
 service PricerService {
     rpc batchPricer (BatchPricerRequest) returns (BatchPricerReply) {
         option (google.api.http) = {
             post: "/pricer/batch_pricer"
         };
     };
 
+    rpc batchPdePricer (BatchPdePricerRequest) returns (BatchPdePricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/batch_pde_pricer"
+        };
+    };
+
     rpc fixedAccAko (FixedAccAkoRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/fixed_acc_ako_as"
         };
     };
 
     rpc linearAccAko (LinearAccAkoRequest) returns (PricerReply) {
@@ -1159,23 +1184,23 @@
 
     rpc sharkfinSeries (SharkfinSeriesRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/sharkfin_series"
         };
     };
 
-    rpc snowballMc (SnowballMcRequest) returns (PricerReply) {
+    rpc snowball (SnowballRequest) returns (PricerReply) {
         option (google.api.http) = {
-            post: "/pricer/snowball_mc"
+            post: "/pricer/snowball"
         };
     };
 
-        rpc snowballDiscountedMc (SnowballDiscountedMcRequest) returns (PricerReply) {
+        rpc snowballDiscounted (SnowballDiscountedRequest) returns (PricerReply) {
         option (google.api.http) = {
-            post: "/pricer/snowball_discounted_mc"
+            post: "/pricer/snowball_discounted"
         };
     };
 
     rpc ratioSpread (RatioSpreadRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/ratio_spread_as"
         };
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.2.6/ht_pricing_module/api_and_utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from .packages import DataFrame
-from .packages import Union
-from .packages import deepcopy
+from .packages import DataFrame, Union, deepcopy, np, norm
 
 
 class _Const(object):
     def __setattr__(self, name, value):
         if name in self.__dict__:
             raise TypeError(f"rebind const({name}) is not allowed")
         self.__dict__[name] = value
@@ -88,7 +86,20 @@
 
         for i in range(_length):
             struct = Struct()
             for k in _keys:
                 setattr(struct, k, input[k][i])
             output.append(struct)
         return output
+
+
+class ParamsBase:
+    def __init__(self, param):
+        self.param = Struct(param) if isinstance(param, dict) else param
+
+
+def BlackScholesVectorize(S, K, r, q, v, T, t, cp):
+    if T - t <= 0 or v == 0:
+        return np.maximum(cp * (S - K), 0)
+    d1 = (np.log(S / K) + (r - q + v * v / 2) * (T - t)) / (v * np.sqrt(T - t))
+    d2 = d1 - v * np.sqrt(T - t)
+    return cp * S * np.exp(-q * (T - t)) * norm.cdf(cp * d1) - cp * K * np.exp(-r * (T - t)) * norm.cdf(cp * d2)
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.2.6/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from ..monte_carlo_engine import *
 from ..api_and_utils import *
+from ..finite_difference_engine import *
 
 
-class OneAssetOptionBase:
+class OneAssetOptionBase(ParamsBase):
 
     def __init__(self, param):
-        self.param = Params(param) if isinstance(param, dict) else param
+        super().__init__(param)
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
     @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     first_ki_idx = np.where(np.max(ki_mat_flag, axis=1), ki_obs_idx[ki_idx], np.nan)
     first_ko_idx = np.where(np.max(ko_mat_flag, axis=1), ko_obs_idx[ko_idx], np.nan)
 
     # 先敲入再敲出或仅敲入
     discount_factor = 1 if is_knock_in else 1 / np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
     ki_arr_flag = np.logical_or(np.logical_or(is_knock_in, np.logical_and(~np.isnan(first_ki_idx), np.isnan(first_ko_idx))), first_ki_idx < first_ko_idx)
-    ki_payoff = ki_arr_flag * discount_factor * notional * (phi * (price[:, -1] - knock_in_strike_price) / entrance_price - margin_rate * (1 / discount_factor - 1))
+    ki_payoff = ki_arr_flag * discount_factor * notional * (phi * (price[:, -1] - knock_in_strike_price) / entrance_price - margin_rate * (np.exp(riskfree_rate * (expiry_date - intraday) / year_base) - 1))
 
     # 先敲出再敲入或仅敲出
     discount_factor = 1 / np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base)
     ko_arr_flag = np.logical_and(1 - is_knock_in, np.logical_or(first_ko_idx < first_ki_idx, np.logical_and(~np.isnan(first_ko_idx), np.isnan(first_ki_idx))))
     ko_payoff = ko_arr_flag * discount_factor * notional * (ko_coupon[ko_idx] - margin_rate * (np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base) - 1))
 
     # 未敲入未敲出
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from ..one_asset_option_base import *
 
 
-def __mc_snowball__(notional, spot_price, entrance_price, knock_in_barrier_price, knock_out_barrier_price,
+def __mc_snowball__(notional, spot_price, entrance_price, knock_in_barrier_price, knock_out_barrier_price, knock_in_strike_price,
                     floor_rate, margin_rate, bonus_rate, option_type, is_knock_in, riskfree_rate, dividend, volatility,
                     residual_intraday, expiry_date, year_base, knock_in_obs, knock_out_obs, participation_rate=0):
     """
     雪球期权
     :param knock_in_obs 敲入观测日, 包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲入价格)
     :param knock_out_obs 敲出观测日，包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲出价格)，coupon_rate票息(已经过敲出日期调整)
     :param floor_rate 保护价
@@ -21,18 +21,19 @@
         ki_flag = False if len(ki_flag) == 0 else ki_flag[0]
 
         ko_adj = knock_out_obs['adjust_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)]
         ko_flag = phi * (spot_price - knock_out_barrier_price * ko_adj) >= 0
         ko_flag = False if len(ko_flag) == 0 else ko_flag[0]
         if ko_flag:
             # 敲出损益
-            rst = notional * knock_out_obs['coupon_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)][0]
+            rst = notional * (knock_out_obs['coupon_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)][0]
+                              + phi * participation_rate * (spot_price - knock_out_barrier_price * ko_adj[0]) / entrance_price)
         elif is_knock_in or ki_flag:
             # 敲入损益
-            rst = notional * max((floor_rate - 1), min(phi * (spot_price / entrance_price - 1), 0))
+            rst = notional * max((floor_rate - 1), min(phi * (spot_price - knock_in_strike_price) / entrance_price, 0))
         else:
             # 未敲入未敲出
             rst = notional * bonus_rate
         return rst
 
     intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
     price = spot_price * McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
@@ -57,22 +58,22 @@
     ki_mat_flag = np.zeros((M, 1), dtype=bool) if len(ki_obs_idx) == 0 else phi * (price[:, ki_obs_idx] - knock_in_barrier_price) <= 0
     ko_mat_flag = np.zeros((M, 1), dtype=bool) if len(ko_obs_idx) == 0 else phi * (price[:, ko_obs_idx] - knock_out_barrier_price) >= 0
     ko_idx = ko_mat_flag.argmax(axis=1)
 
     # 敲出
     discount_factor = 1 / np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base)
     ko_arr_flag = np.max(ko_mat_flag, axis=1)
-    ko_payoff = ko_arr_flag * discount_factor * notional * (ko_coupon[ko_idx] + phi * participation_rate * ((price[:, ko_obs_idx] / knock_out_barrier_price - 1)[np.arange(M), ko_idx])
+    ko_payoff = ko_arr_flag * discount_factor * notional * (ko_coupon[ko_idx] + phi * participation_rate * (((price[:, ko_obs_idx] - knock_out_barrier_price) / entrance_price)[np.arange(M), ko_idx])
                                                             - margin_rate * (np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base) - 1))
 
     # 敲入未敲出
     discount_factor = 1 / np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
     ki_arr_flag = np.logical_or(is_knock_in, np.max(ki_mat_flag, axis=1))
     ki_no_ko_arr_flag = np.logical_and(ki_arr_flag, np.logical_not(ko_arr_flag))
-    ki_no_ko_payoff = ki_no_ko_arr_flag * discount_factor * notional * (np.maximum((floor_rate - 1), np.minimum(phi * (price[:, -1] / entrance_price - 1), 0))
+    ki_no_ko_payoff = ki_no_ko_arr_flag * discount_factor * notional * (np.maximum((floor_rate - 1), np.minimum(phi * (price[:, -1] - knock_in_strike_price) / entrance_price, 0))
                                                                         - margin_rate * (1 / discount_factor - 1))
 
     # 未敲入未敲出
     discount_factor = 1 / np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
     no_ki_no_ko_arr_flag = np.logical_and(np.logical_not(ki_arr_flag), np.logical_not(ko_arr_flag))
     no_ki_no_ko_payoff = no_ki_no_ko_arr_flag * discount_factor * notional * (bonus_rate - margin_rate * (1 / discount_factor - 1))
 
@@ -87,14 +88,15 @@
         current_date_index = math.floor(self.param.current_date)
         return __mc_snowball__(
             notional=self.param.notional,
             spot_price=self.param.spot_price,
             entrance_price=self.param.entrance_price,
             knock_in_barrier_price=self.param.knock_in_barrier_price,
             knock_out_barrier_price=self.param.knock_out_barrier_price,
+            knock_in_strike_price=self.param.knock_in_strike_price,
             floor_rate=self.param.floor_rate,
             margin_rate=self.param.margin_rate,
             bonus_rate=self.param.bonus_rate,
             option_type=self.param.option_type,
             is_knock_in=self.param.is_knock_in,
             riskfree_rate=self.param.riskfree_rate,
             dividend=self.param.dividend,
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.2.6/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.2.6/ht_pricing_module/simple_pricer_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -563,15 +563,15 @@
             margin_rate:                Union[int, float],
             bonus_rate:                 Union[int, float],
             year_base:                  int,
             knock_in_obs_date:          Union[dict, list, DataFrame],
             knock_out_obs_date:         Union[dict, list, DataFrame],
             is_knock_in:                Union[int] = 0,
             option_type:                int = OptionType.STANDARD,
-            pricing_method:             int = PricingMethod.MC,
+            pricing_method:             int = PricingMethod.PDE,
             participation_rate:         Union[int, float] = 0,
             is_discount:                Union[int] = 0,
             entrance_price:             Union[int, float] = None,
             knock_in_strike_price:      Union[int, float] = None,
     ):
         """
 
@@ -594,15 +594,15 @@
         :param knock_in_obs_date: 雪球MC敲入观测日，dict， Dataframe类型
                或RepeatedStruct返回结果: [Params(), ...], Struct(obs_index, adjust_rate)
         :param knock_out_obs_date: 雪球MC敲出观测日，dict， Dataframe类型
                或RepeatedStruct返回结果: [Params(), ...], Struct(obs_index, adjust_rate, coupon_rate)
         :param is_knock_in: 1为已敲入0为未敲入
         :param participation_rate: 增强雪球敲出参与率
         :param is_discount: 是否为折价减仓雪球
-        :param knock_in_strike_price 折价建仓雪球执行价
+        :param knock_in_strike_price 折价建仓雪球执行价，默认值为敲入价 或 OTM雪球敲入执行价，默认值为入场价
         :return: 雪球期权定价引擎
         """
 
         assert is_knock_in in [0, 1], "param: is_knock_in should be either 0 or 1"
         assert is_discount in [0, 1], "param: is_discount should be either 0 or 1"
         assert option_type in [OptionType.STANDARD, OptionType.REVERSE], option_type
 
@@ -618,33 +618,38 @@
         param['is_knock_in'] = is_knock_in
         param['riskfree_rate'] = riskfree_rate
         param['dividend'] = dividend
         param['volatility'] = volatility
         param['current_date'] = current_date
         param['expiry_date'] = expiry_date
         param['year_base'] = year_base
+        param['participation_rate'] = participation_rate
+
+        adjust_rate = 'adjust_rate'
+        if adjust_rate not in knock_in_obs_date.keys():
+            knock_in_obs_date[adjust_rate] = np.ones_like(knock_in_obs_date['obs_index'])
+        if adjust_rate not in knock_out_obs_date.keys():
+            knock_out_obs_date[adjust_rate] = np.ones_like(knock_out_obs_date['obs_index'])
+
         param['knock_in_obs_date'] = Params.RepeatedStruct(knock_in_obs_date)
         param['knock_out_obs_date'] = Params.RepeatedStruct(knock_out_obs_date)
-        param['participation_rate'] = participation_rate
+        param['entrance_price'] = spot_price if entrance_price is None else entrance_price
 
-        if entrance_price is None:
-            param['entrance_price'] = spot_price
+        if is_discount:
+            param['knock_in_strike_price'] = param['knock_in_barrier_price'] if knock_in_strike_price is None else knock_in_strike_price
+            if pricing_method == PricingMethod.MC:  # SnowballDiscountMc
+                return SnowballDiscountedMc(param)
+            elif pricing_method == PricingMethod.PDE:   # SnowballDiscountPde
+                return SnowballDiscountedPde(param)
         else:
-            param['entrance_price'] = entrance_price
-
-        # SnowballMc
-        if not is_discount and pricing_method == PricingMethod.MC:
-            return SnowballMc(param)
-        # SnowballDiscountMc
-        elif is_discount and pricing_method == PricingMethod.MC:
-            if knock_in_strike_price is None:
-                param['knock_in_strike_price'] = knock_in_barrier_price
-            else:
-                param['knock_in_strike_price'] = knock_in_strike_price
-            return SnowballDiscountedMc(param)
+            param['knock_in_strike_price'] = param['entrance_price'] if knock_in_strike_price is None else knock_in_strike_price
+            if pricing_method == PricingMethod.MC:  # SnowballMc
+                return SnowballMc(param)
+            elif pricing_method == PricingMethod.PDE:   # SnowballPde
+                return SnowballPde(param)
 
     @classmethod
     def airbag(
             cls,
             spot_price:                 Union[int, float],
             strike_price:               Union[int, float],
             barrier_price:              Union[int, float],
```

### Comparing `ht_pricing_module-0.2.5/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.2.6/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 ht_pricing_module/api_and_utils/protos/__init__.py
 ht_pricing_module/api_and_utils/protos/pricer.proto
 ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
 ht_pricing_module/api_and_utils/protos/google/api/http.proto
 ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
 ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
 ht_pricing_module/finite_difference_engine/__init__.py
+ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
+ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
+ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
 ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+ht_pricing_module/finite_difference_engine/fully_explicit_european.py
+ht_pricing_module/finite_difference_engine/fully_implicit_european.py
 ht_pricing_module/monte_carlo_engine/__init__.py
 ht_pricing_module/monte_carlo_engine/mc_path_generator.py
 ht_pricing_module/multi_asset_pricing_module/__init__.py
 ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
 ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
 ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
 ht_pricing_module/one_asset_pricing_module/__init__.py
@@ -44,19 +49,23 @@
 ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
 ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
 ht_pricing_module/one_asset_pricing_module/asian/__init__.py
 ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
 ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
 ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
 ht_pricing_module/one_asset_pricing_module/basket/__init__.py
 ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
 ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
 ht_pricing_module/one_asset_pricing_module/binary/__init__.py
 ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
 ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
 ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
@@ -64,18 +73,23 @@
 ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
 ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
+ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
 ht_pricing_module/one_asset_pricing_module/spread/__init__.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
 ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
 ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
 ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
 ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
 ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
 ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
 ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
```

### Comparing `ht_pricing_module-0.2.5/setup.py` & `ht_pricing_module-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.2.5"
+VERSION = "0.2.6"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

