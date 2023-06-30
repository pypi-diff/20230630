# Comparing `tmp/ht_pricing_module-0.3.0.tar.gz` & `tmp/ht_pricing_module-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.3.0.tar", last modified: Fri Jun 30 03:05:00 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.3.1.tar", last modified: Fri Jun 30 08:43:24 2023, max compression
```

## Comparing `ht_pricing_module-0.3.0.tar` & `ht_pricing_module-0.3.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.356487 ht_pricing_module-0.3.0/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0      263 2023-06-30 03:05:00.356487 ht_pricing_module-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      408 2023-06-30 03:03:44.000000 ht_pricing_module-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.754098 ht_pricing_module-0.3.0/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.3.0/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.777036 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      293 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      558 2023-06-13 01:59:48.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.789005 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.742130 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.814935 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.833884 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    48559 2023-06-29 01:54:18.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3707 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.883752 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0      234 2023-06-27 10:54:41.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     2070 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
--rw-rw-rw-   0        0        0     1007 2023-06-16 01:16:24.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
--rw-rw-rw-   0        0        0     8053 2023-06-30 03:02:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
--rw-rw-rw-   0        0        0     5329 2023-06-27 10:17:12.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
--rw-rw-rw-   0        0        0      693 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fully_explicit_european.py
--rw-rw-rw-   0        0        0      736 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fully_implicit_european.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.897742 ht_pricing_module-0.3.0/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-06-19 06:14:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.909682 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.916664 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.931623 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.055321 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5561 2023-06-07 10:16:58.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
--rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.066263 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.098179 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.164999 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-06-27 02:32:08.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     2393 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
--rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     2263 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
--rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     2963 2023-06-26 13:12:34.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
--rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
--rw-rw-rw-   0        0        0     3503 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.185944 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.224839 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.226833 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     5693 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.238802 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3902 2023-06-05 06:56:38.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.265730 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0      194 2023-06-27 11:31:24.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     5753 2023-06-28 02:47:53.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
--rw-rw-rw-   0        0        0     5077 2023-06-30 02:53:01.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
--rw-rw-rw-   0        0        0     6870 2023-06-28 09:02:37.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
--rw-rw-rw-   0        0        0     6932 2023-06-30 02:54:24.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
--rw-rw-rw-   0        0        0     4852 2023-06-29 13:27:41.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.281688 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.330557 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-06-27 02:30:19.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     3801 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
--rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     3157 2023-06-26 01:22:55.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:05:00.344519 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-06-13 02:30:48.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    45943 2023-06-28 09:02:37.000000 ht_pricing_module-0.3.0/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-06-30 03:04:59.766066 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      263 2023-06-30 03:04:59.000000 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6098 2023-06-30 03:04:59.000000 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 03:04:59.000000 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-30 03:04:59.000000 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-30 03:04:59.000000 ht_pricing_module-0.3.0/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 03:05:00.357484 ht_pricing_module-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-06-30 03:03:44.000000 ht_pricing_module-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.168760 ht_pricing_module-0.3.1/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      263 2023-06-30 08:43:24.168760 ht_pricing_module-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2023-06-30 08:43:11.000000 ht_pricing_module-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.557395 ht_pricing_module-0.3.1/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.3.1/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.581331 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      293 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      558 2023-06-13 01:59:48.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.593298 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.545428 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.619229 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.638179 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    48559 2023-06-29 01:54:18.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3707 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.688045 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0      234 2023-06-27 10:54:41.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     2070 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py
+-rw-rw-rw-   0        0        0     1007 2023-06-16 01:16:24.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py
+-rw-rw-rw-   0        0        0     8051 2023-06-30 08:24:13.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py
+-rw-rw-rw-   0        0        0     5329 2023-06-27 10:17:12.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+-rw-rw-rw-   0        0        0      693 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fully_explicit_european.py
+-rw-rw-rw-   0        0        0      736 2023-06-16 01:17:54.000000 ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fully_implicit_european.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.702008 ht_pricing_module-0.3.1/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-06-19 06:14:01.000000 ht_pricing_module-0.3.1/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.714974 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.719960 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.735917 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.859587 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5561 2023-06-07 10:16:58.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.870557 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.902472 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.969294 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-06-27 02:32:08.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     2393 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py
+-rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     2263 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py
+-rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     2963 2023-06-26 13:12:34.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py
+-rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+-rw-rw-rw-   0        0        0     3503 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.990238 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.020157 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.022152 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     5693 2023-06-27 10:58:01.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.034120 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3902 2023-06-05 06:56:38.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.082989 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0      194 2023-06-27 11:31:24.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     5753 2023-06-28 02:47:53.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+-rw-rw-rw-   0        0        0     5077 2023-06-30 02:53:01.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py
+-rw-rw-rw-   0        0        0     6870 2023-06-28 09:02:37.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+-rw-rw-rw-   0        0        0     6932 2023-06-30 02:54:24.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py
+-rw-rw-rw-   0        0        0     4852 2023-06-29 13:27:41.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.092963 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.142830 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-06-27 02:30:19.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     3801 2023-06-26 13:08:59.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py
+-rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     3157 2023-06-26 01:22:55.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:24.156792 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-06-13 02:30:48.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    45943 2023-06-28 09:02:37.000000 ht_pricing_module-0.3.1/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-06-30 08:43:23.570360 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-06-30 08:43:23.000000 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6098 2023-06-30 08:43:23.000000 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 08:43:23.000000 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-30 08:43:23.000000 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-30 08:43:23.000000 ht_pricing_module-0.3.1/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 08:43:24.168760 ht_pricing_module-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1158 2023-06-30 08:43:11.000000 ht_pricing_module-0.3.1/setup.py
```

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/packages.py` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/packages.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.3.1/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_american.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_european.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/crank_nicolson_snowball.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 
 class CrankNicolsonSnowball(ParamsBase):
 
     def __init__(self, param, Ns=None, theta=1):
         super().__init__(param)
 
-        self.Smin = 0.2 * min(self.param.spot_price, self.param.entrance_price)
-        self.Smax = 2 * max(self.param.spot_price, self.param.entrance_price)
+        self.Smin = 0 * min(self.param.spot_price, self.param.entrance_price)
+        self.Smax = 3 * max(self.param.spot_price, self.param.entrance_price)
 
         self._T0 = round(self.param.current_date, 4)
         self._TT = round(self.param.expiry_date, 4)
         self._Ns = pow(10, 3) if Ns is None else int(Ns)
         self._Nt = int(round(self._TT - int(self._T0), 4))
 
         self._Tau = round(self._T0 - int(self._T0), 4)
```

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fully_explicit_european.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fully_explicit_european.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/finite_difference_engine/fully_implicit_european.py` & `ht_pricing_module-0.3.1/ht_pricing_module/finite_difference_engine/fully_implicit_european.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.3.1/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_american_knock_out_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/barrier_knock_out_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_knock_out_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/barrier/discrete_double_barrier_knock_out_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/snowball/snowball_pde_v0.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_double_one_touch_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_pde.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.3.1/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.3.1/ht_pricing_module/simple_pricer_engine.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.3.1/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.3.0/setup.py` & `ht_pricing_module-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

