# Comparing `tmp/dramkit-0.5.44.tar.gz` & `tmp/dramkit-0.5.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.44.tar", last modified: Fri Jun  2 01:07:05 2023, max compression
+gzip compressed data, was "dramkit-0.5.45.tar", last modified: Fri Jun 30 07:52:53 2023, max compression
```

## Comparing `dramkit-0.5.44.tar` & `dramkit-0.5.45.tar`

### file list

```diff
@@ -1,193 +1,192 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.934461 dramkit-0.5.44/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.44/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-06-02 01:07:05.932894 dramkit-0.5.44/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.44/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.495039 dramkit-0.5.44/dramkit/
--rw-rw-rw-   0        0        0     1017 2023-05-23 01:38:43.000000 dramkit-0.5.44/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-06-02 01:06:31.000000 dramkit-0.5.44/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.628683 dramkit-0.5.44/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.44/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.44/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.44/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.44/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.44/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.44/dramkit/_tmp/test_await_timeout.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.44/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.44/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.44/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.44/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.44/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.44/dramkit/_tmp/test_multiprocessing.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.44/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.44/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.44/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.44/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.44/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.44/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.44/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.44/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.44/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.638758 dramkit-0.5.44/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.44/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.44/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.675670 dramkit-0.5.44/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21188 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3966740 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-05-31 13:08:27.000000 dramkit-0.5.44/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.44/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    34826 2023-05-20 15:37:28.000000 dramkit-0.5.44/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.731671 dramkit-0.5.44/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.44/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.44/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.44/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.44/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.44/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.44/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.44/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.44/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.44/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.44/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.44/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.44/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.44/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    20288 2023-05-19 06:29:01.000000 dramkit-0.5.44/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    10239 2023-06-01 16:04:12.000000 dramkit-0.5.44/dramkit/datsci/rl_markov.py
--rw-rw-rw-   0        0        0     4510 2023-05-31 14:53:44.000000 dramkit-0.5.44/dramkit/datsci/rl_markov_linprog.py
--rw-rw-rw-   0        0        0    12678 2023-05-31 06:09:33.000000 dramkit-0.5.44/dramkit/datsci/rl_markov_sympy.py
--rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.44/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.44/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.44/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.44/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.44/dramkit/datsci/utils_ml.py
--rw-rw-rw-   0        0        0    21136 2023-05-21 10:05:57.000000 dramkit-0.5.44/dramkit/datsci/zigzag.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.748671 dramkit-0.5.44/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.44/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   127908 2023-05-24 02:23:16.000000 dramkit-0.5.44/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.44/dramkit/install_check.py
--rw-rw-rw-   0        0        0    67350 2023-05-19 01:46:24.000000 dramkit-0.5.44/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.761673 dramkit-0.5.44/dramkit/logtools/
--rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.44/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.44/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.44/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.44/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4494 2023-05-24 02:19:43.000000 dramkit-0.5.44/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.772687 dramkit-0.5.44/dramkit/openai/
--rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.44/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.44/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.44/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.44/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.809674 dramkit-0.5.44/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.44/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.44/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.44/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.44/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.44/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.44/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.44/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.44/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.44/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.44/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.44/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.44/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.835674 dramkit-0.5.44/dramkit/other/
--rw-rw-rw-   0        0        0      831 2023-05-21 07:44:53.000000 dramkit-0.5.44/dramkit/other/_Git_notes.py
--rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.44/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.44/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.44/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.44/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     6013 2023-05-27 15:36:26.000000 dramkit-0.5.44/dramkit/other/debt_cal.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.44/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8757 2023-05-21 07:05:41.000000 dramkit-0.5.44/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.44/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.44/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.851675 dramkit-0.5.44/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.44/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.44/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.44/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.44/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.44/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.44/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.860676 dramkit-0.5.44/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.44/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.44/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.877676 dramkit-0.5.44/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.44/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.44/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.44/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.44/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.44/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.894677 dramkit-0.5.44/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.44/dramkit/speedup/_mp_test1.py
--rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.44/dramkit/speedup/_mp_test2.py
--rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.44/dramkit/speedup/_mp_test3.py
--rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.44/dramkit/speedup/iotools_tmp.py
--rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.44/dramkit/speedup/multi_process_concurrent.py
--rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.44/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.914682 dramkit-0.5.44/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.44/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.44/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.44/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.44/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.44/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.44/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.44/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.44/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.922698 dramkit-0.5.44/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.44/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5427 2023-05-31 05:22:42.000000 dramkit-0.5.44/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.929678 dramkit-0.5.44/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.44/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.44/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-06-02 01:07:05.510002 dramkit-0.5.44/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-06-02 01:07:01.000000 dramkit-0.5.44/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5029 2023-06-02 01:07:04.000000 dramkit-0.5.44/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 01:07:01.000000 dramkit-0.5.44/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-06-02 01:07:01.000000 dramkit-0.5.44/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 01:07:01.000000 dramkit-0.5.44/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 01:07:05.934461 dramkit-0.5.44/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.262866 dramkit-0.5.45/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.45/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-06-30 07:52:53.261866 dramkit-0.5.45/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.45/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.764881 dramkit-0.5.45/dramkit/
+-rw-rw-rw-   0        0        0     1052 2023-06-16 10:22:54.000000 dramkit-0.5.45/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-06-30 07:52:04.000000 dramkit-0.5.45/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.897867 dramkit-0.5.45/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.45/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.45/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0    41819 2023-06-06 08:45:33.000000 dramkit-0.5.45/dramkit/_tmp/feature_selection.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.45/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.45/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0    26310 2023-06-14 06:03:36.000000 dramkit-0.5.45/dramkit/_tmp/step_reg.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.45/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.45/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.45/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.45/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.45/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.45/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.45/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.45/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.45/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.45/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.45/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.45/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.45/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.45/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.45/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.45/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.45/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.906870 dramkit-0.5.45/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.45/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.45/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.954883 dramkit-0.5.45/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3978799 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-06-29 15:17:00.000000 dramkit-0.5.45/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.45/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    35391 2023-06-26 02:06:52.000000 dramkit-0.5.45/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.027951 dramkit-0.5.45/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.45/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     8115 2023-06-08 02:59:55.000000 dramkit-0.5.45/dramkit/datsci/_rl_mab.py
+-rw-rw-rw-   0        0        0    42723 2023-06-29 15:51:40.000000 dramkit-0.5.45/dramkit/datsci/_rl_markov.py
+-rw-rw-rw-   0        0        0    13956 2023-06-29 16:36:06.000000 dramkit-0.5.45/dramkit/datsci/_rl_mcdp.py
+-rw-rw-rw-   0        0        0     2865 2023-06-09 04:28:19.000000 dramkit-0.5.45/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.45/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.45/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.45/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.45/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.45/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.45/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.45/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.45/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.45/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.45/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     7362 2023-06-13 05:23:22.000000 dramkit-0.5.45/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    20428 2023-06-20 07:06:30.000000 dramkit-0.5.45/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0      790 2023-06-14 12:02:47.000000 dramkit-0.5.45/dramkit/datsci/rl_markov_new.py
+-rw-rw-rw-   0        0        0    44419 2023-06-26 08:21:38.000000 dramkit-0.5.45/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    18111 2023-06-26 07:18:32.000000 dramkit-0.5.45/dramkit/datsci/stepreg.py
+-rw-rw-rw-   0        0        0    36092 2023-06-20 06:09:25.000000 dramkit-0.5.45/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.45/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.45/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6869 2023-06-20 06:49:38.000000 dramkit-0.5.45/dramkit/datsci/utils_ml.py
+-rw-rw-rw-   0        0        0    21136 2023-05-21 10:05:57.000000 dramkit-0.5.45/dramkit/datsci/zigzag.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.048868 dramkit-0.5.45/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.45/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   130403 2023-06-28 08:59:48.000000 dramkit-0.5.45/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.45/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67711 2023-06-29 15:42:42.000000 dramkit-0.5.45/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.065881 dramkit-0.5.45/dramkit/logtools/
+-rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.45/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.45/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.45/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.45/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4494 2023-06-18 01:41:28.000000 dramkit-0.5.45/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.078867 dramkit-0.5.45/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.45/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.45/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.45/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.45/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.119869 dramkit-0.5.45/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.45/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.45/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.45/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.45/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.45/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.45/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.45/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.45/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.45/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.45/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.45/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.45/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.148866 dramkit-0.5.45/dramkit/other/
+-rw-rw-rw-   0        0        0      831 2023-05-21 07:44:53.000000 dramkit-0.5.45/dramkit/other/_Git_notes.py
+-rw-rw-rw-   0        0        0     3983 2023-06-13 02:44:22.000000 dramkit-0.5.45/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.45/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.45/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.45/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     6453 2023-06-15 12:19:25.000000 dramkit-0.5.45/dramkit/other/debt_cal.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.45/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8829 2023-06-29 09:50:52.000000 dramkit-0.5.45/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.45/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.45/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.171866 dramkit-0.5.45/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.45/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.45/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.45/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.45/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.45/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     4789 2023-06-12 03:17:06.000000 dramkit-0.5.45/dramkit/plottools/twinx_align.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.45/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.178887 dramkit-0.5.45/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.45/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.45/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.196917 dramkit-0.5.45/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.45/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.45/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.45/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.45/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.45/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.219868 dramkit-0.5.45/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.45/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.45/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.45/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.45/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0      858 2023-06-12 06:03:15.000000 dramkit-0.5.45/dramkit/speedup/job_lib.py
+-rw-rw-rw-   0        0        0     3796 2023-06-15 08:12:44.000000 dramkit-0.5.45/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.45/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.243882 dramkit-0.5.45/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.45/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.45/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6985 2023-06-09 08:58:07.000000 dramkit-0.5.45/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.45/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.45/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.45/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.45/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.45/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.251944 dramkit-0.5.45/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.45/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5427 2023-05-31 05:22:42.000000 dramkit-0.5.45/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:53.258869 dramkit-0.5.45/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.45/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.45/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-06-30 07:52:52.779894 dramkit-0.5.45/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5009 2023-06-30 07:52:51.000000 dramkit-0.5.45/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-30 07:52:48.000000 dramkit-0.5.45/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 07:52:53.263869 dramkit-0.5.45/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.45/setup.py
```

### Comparing `dramkit-0.5.44/LICENSE` & `dramkit-0.5.45/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/PKG-INFO` & `dramkit-0.5.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.44
+Version: 0.5.45
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.44/README.md` & `dramkit-0.5.45/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/__init__.py` & `dramkit-0.5.45/dramkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from ._pkg_info import pkg_info
 __version__ = pkg_info['__version__']
 from .install_check import install_check
 
-from .gentools import isnull
-from .gentools import log_used_time
 from .gentools import GenObject
 from .gentools import TimeRecoder
+from .gentools import isnull
+from .gentools import log_used_time
+from .gentools import raise_error
 from .gentools import tmprint
 
 from .iotools import load_csv
 from .iotools import load_text, write_txt
 from .iotools import load_json, write_json
 from .iotools import pickle_file, unpickle_file
```

### Comparing `dramkit-0.5.44/dramkit/_pkg_info.py` & `dramkit-0.5.45/dramkit/_pkg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.44',
+    '__version__': '0.5.45',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.44/dramkit/_tmp/CRR.py` & `dramkit-0.5.45/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.45/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.45/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.45/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.45/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/VMD.py` & `dramkit-0.5.45/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/cca_test.py` & `dramkit-0.5.45/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.45/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/explore.py` & `dramkit-0.5.45/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/gini.py` & `dramkit-0.5.45/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.45/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.45/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.45/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.45/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/plot_test.py` & `dramkit-0.5.45/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.45/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.45/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.45/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_await_timeout.py` & `dramkit-0.5.45/dramkit/_tmp/test_await_timeout.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.45/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.45/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_code.py` & `dramkit-0.5.45/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.45/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.45/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_grading.py` & `dramkit-0.5.45/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_lr.py` & `dramkit-0.5.45/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.45/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.45/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_tree.py` & `dramkit-0.5.45/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.45/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.45/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.45/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/tmp.py` & `dramkit-0.5.45/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.45/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.45/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.45/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.45/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.45/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.45/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.45/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.45/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/__init__.py` & `dramkit-0.5.45/dramkit/chncal/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/apis.py` & `dramkit-0.5.45/dramkit/chncal/apis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/constants.py` & `dramkit-0.5.45/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/constants_fate.py` & `dramkit-0.5.45/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/constants_hko.py` & `dramkit-0.5.45/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.45/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6113,14 +6113,43 @@
     ("CFFEX", datetime.date(year=2023, month=5, day=25)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=26)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=27)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=28)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=29)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=30)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=31)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=1)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=2)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=3)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=4)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=5)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=6)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=7)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=8)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=9)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=10)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=11)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=12)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=13)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=14)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=15)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=17)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=18)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=19)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=20)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=21)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=22)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=23)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=24)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=25)): 0,
+    ("CFFEX", datetime.date(year=2023, month=6, day=26)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=27)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=28)): 1,
+    ("CFFEX", datetime.date(year=2023, month=6, day=29)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -18032,14 +18061,43 @@
     ("CZCE", datetime.date(year=2023, month=5, day=25)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=26)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=27)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=28)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=29)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=30)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("CZCE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("CZCE", datetime.date(year=2023, month=6, day=29)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -29080,14 +29138,43 @@
     ("DCE", datetime.date(year=2023, month=5, day=25)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=26)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=27)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=28)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=29)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=30)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("DCE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("DCE", datetime.date(year=2023, month=6, day=29)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31279,14 +31366,43 @@
     ("INE", datetime.date(year=2023, month=5, day=25)): 1,
     ("INE", datetime.date(year=2023, month=5, day=26)): 1,
     ("INE", datetime.date(year=2023, month=5, day=27)): 0,
     ("INE", datetime.date(year=2023, month=5, day=28)): 0,
     ("INE", datetime.date(year=2023, month=5, day=29)): 1,
     ("INE", datetime.date(year=2023, month=5, day=30)): 1,
     ("INE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("INE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("INE", datetime.date(year=2023, month=6, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42970,14 +43086,43 @@
     ("SHFE", datetime.date(year=2023, month=5, day=25)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=26)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=27)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=28)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("SHFE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("SHFE", datetime.date(year=2023, month=6, day=29)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54822,14 +54967,43 @@
     ("SSE", datetime.date(year=2023, month=5, day=25)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=26)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=27)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=28)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=29)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=30)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("SSE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("SSE", datetime.date(year=2023, month=6, day=29)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66478,8 +66652,37 @@
     ("SZSE", datetime.date(year=2023, month=5, day=25)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=26)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=27)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=28)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=29)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=30)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=31)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=1)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=2)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=3)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=4)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=5)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=6)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=7)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=8)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=9)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=10)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=11)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=12)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=13)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=14)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=15)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=17)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=18)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=19)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=20)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=21)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=22)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=23)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=24)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=25)): 0,
+    ("SZSE", datetime.date(year=2023, month=6, day=26)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=27)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=28)): 1,
+    ("SZSE", datetime.date(year=2023, month=6, day=29)): 1,
 }
```

### Comparing `dramkit-0.5.44/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.45/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.45/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/chncal/solar_terms.py` & `dramkit-0.5.45/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/cryptotools.py` & `dramkit-0.5.45/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datetimetools.py` & `dramkit-0.5.45/dramkit/datetimetools.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,23 @@
     res = pd.to_datetime(series)
     if pd.isnull(strformat):
         strformat = '%Y{x}%m{x}%d'.format(x=joiner)
     res = res.apply(lambda x: x.strftime(strformat))
     return res
 
 
+def check_dt_format(dt, strformat='%Y%m%d'):
+    '''检查dt的格式是否符合strformat'''
+    try:
+        dt = datetime.datetime.strptime(dt, strformat)
+        return True
+    except:
+        return False
+
+
 def get_datetime_strformat(tstr,
                            ymd = ['-', '', '.', '/'],
                            ymd_hms = [' ', '', '.'],
                            hms = [':', ''],
                            hms_ms = ['.', '']
                            ):
     '''
@@ -686,14 +695,25 @@
         month_end = day.replace(day=MONTH_DAYS[m])
     else:
         next_month = day.replace(day=28) + datetime.timedelta(days=4)
         month_end = next_month - datetime.timedelta(days=next_month.day)
     return copy_format(month_end, date)
 
 
+def get_next_month(month=None, n=1, joiner=''):
+    '''获取下一个月，month格式为%Y{joiner}%m'''
+    if pd.isnull(month):
+        m = today_date('')[:6]
+    else:
+        m = str(month).replace(joiner, '')
+    y, m = int(m[:4]), int(m[-2:])
+    y, m = get_2part_next(y, m, 12, n)
+    return str(y)+joiner+str(m).zfill(2)
+
+
 def get_next_nmonth_start_end(date=None, n=1):
     if pd.isnull(date):
         date = today_date()
     day = x2datetime(date)
     y, m = day.year, day.month
     y, m = get_2part_next(y, m, 12, n)
     month_start = pd.to_datetime('%s-%s-01'%(y, m))
```

### Comparing `dramkit-0.5.44/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.45/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.45/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/ahp.py` & `dramkit-0.5.45/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.45/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/apriori.py` & `dramkit-0.5.45/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/curvature.py` & `dramkit-0.5.45/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/elm_cls.py` & `dramkit-0.5.45/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/elm_reg.py` & `dramkit-0.5.45/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.45/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.45/dramkit/datsci/find_maxmin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.45/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/lr.py` & `dramkit-0.5.45/dramkit/datsci/lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,46 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
+import pandas as pd
+from beartype import beartype
 import statsmodels.api as sm
+from statsmodels.formula import api as smf
+from typing import Union
+from dramkit.gentools import isnull
+
+
+@beartype
+def lr_smf_df(df : pd.DataFrame,
+              ycol: str,
+              xcols : Union[list, tuple, set] = None,
+              intercept : bool = True):
+    '''
+    statsmodels.formula拟合线性回归
+    
+    Examples
+    --------
+    >>> df = pd.DataFrame({'x': [1, 2, 3, 4, 5],
+    >>>                    'y': [2, 3, 4, 5, 6],
+    # >>>                    'y': [2, 4, 6, 8, 10]
+    >>>                   })
+    >>> xcols = ['x']
+    >>> ycol = 'y'
+    >>> mdl1 = lr_smf_df(df, ycol, xcols, intercept=True)
+    >>> mdl2 = lr_smf_df(df, ycol, xcols, intercept=False)
+    >>> print(mdl1.params, '\n', mdl2.params)
+    '''
+    if isnull(xcols):
+        xcols = [x for x in df.columns if x != ycol]
+    if intercept: # 是否有截距
+        formula = '{} ~ {} + 1'.format(ycol, ' + '.join(xcols))
+    else:
+        formula = '{} ~ {} - 1'.format(ycol, ' + '.join(xcols))
+    mdl = smf.ols(formula, df).fit() # 最小二乘法
+    return mdl
 
 
 def lr_fit_sm(X, y):
     '''
     statsmodels线性回归拟合
     '''
```

### Comparing `dramkit-0.5.44/dramkit/datsci/preprocess.py` & `dramkit-0.5.45/dramkit/datsci/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,18 @@
     values[values < lower] = low_cut_val
     try:
         return pd.Series(values, index=series.index)
     except:
         return values
     
     
+def mad(*args, **kwargs):
+    return cut_mad(*args, **kwargs)
+    
+    
 def cut_nstd(series, n=3, up_cut_val=None, low_cut_val=None):
     '''标准差倍数截断方法，极端值处理'''
     df = pd.DataFrame({'s': series})
     mean = df['s'].mean()
     std = df['s'].std()
     upper = mean + n * std
     lower = mean - n * std
@@ -309,18 +313,18 @@
         df_ = pd.DataFrame(df_)
         df_.columns = ['imf'+str(_) for _ in range(1, df_.shape[1]+1)]
         return df_
     df_pca = pca_trans(df)
     if dfs_trans is not None:
         dfs_transed = []
         for df_ in dfs_trans:
-            dfs_transed.append(df_)
+            dfs_transed.append(pca_trans(df_))
     else:
         dfs_transed = None
-    return df_pca, tuple(dfs_transed)
+    return df_pca, tuple(dfs_transed), mdl
 
 
 def scale_skl(df_fit, dfs_trans=None, cols=None, scale_type='std', **kwargs):
     '''
     用sklearn进行数据标准化处理
 
     Parameters
@@ -344,14 +348,15 @@
         df_fit标准化之后的数据
     dfs_transed : None, pandas.DataFrame, tuple
         dfs_trans标准化之后对应的数据
     scaler_info : tuple
         包含scaler即df_fit计算得到的标准化中间变量信息; cols即用到的列名列表
     '''
 
+    # TODO: 增加更多Scaler支持
     sklScaler_map = {'std': StandardScaler, 'z-score': StandardScaler,
                      'maxmin': MinMaxScaler, 'minmax': MinMaxScaler}
     sklScaler = sklScaler_map[scale_type]
 
     cols_all = list(df_fit.columns)
 
     if cols is None:
@@ -478,20 +483,20 @@
     elif return_type == 'df':
         mis_rates = pd.DataFrame(mis_rates).reset_index()
         mis_rates.columns = ['col', 'miss_pct']
         mis_rates.sort_values('miss_pct', ascending=False, inplace=True)
         return mis_rates
     
     
-def drop_miss_feature(data, cols=None, thre=0.8):
+def drop_miss_feature(data, cols=None, thr=0.8):
     '''删除缺失率大于thre的列'''
     loss_rates = get_miss_rate(data, cols=cols)
-    drop_cols = [x for x in loss_rates if loss_rates[x] > thre]
+    drop_cols = [x for x in loss_rates if loss_rates[x] > thr]
     df = data.drop(drop_cols, axis=1)
-    return df
+    return df, loss_rates
 
 
 def drop_miss_sample(data, thre=0.5, cols=None):
     '''
     | 删除数据缺失率大于thre的样本（行）
     | 注：应保证data.index是唯一的
     '''
```

### Comparing `dramkit-0.5.44/dramkit/datsci/stats.py` & `dramkit-0.5.45/dramkit/datsci/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import math
 import numpy as np
 import pandas as pd
 
 from scipy.stats import norm, lognorm, weibull_min, kstest
 from scipy.stats import t, f, chi2
 
+from statsmodels.tools.tools import add_constant
+from statsmodels.stats.outliers_influence import variance_inflation_factor
+
 from sklearn.linear_model import LinearRegression as lr
 
 from dramkit.gentools import isnull
 from dramkit.sorts.insert_sort import rank_of_insert
 from dramkit.sorts.insert_sort_bin import rank_of_insert_bin
 
 
@@ -372,14 +375,24 @@
     Stat, P = kstest(np.log(series), 'weibull_min', args=(c, loc, scale))
     if plot:
         from dramkit.plottools.plot_histdist import plot_histdist
         plot_histdist(series, dists={'weibull': ('-r', None)}, **kwargs_plot)
     return (Stat, P), (k, lmd)
 
 
+def get_at_range_prob_norm(mu, sigma, low, high):
+    '''获取正态分布N(mu,sigma)取值范围在low和high之间的概率'''
+    # 计算标准化的z_score值
+    z_low = (low - mu) / sigma
+    z_high = (high - mu) / sigma
+    # 计算在z-score范围内的概率
+    prob = norm.cdf(z_high) - norm.cdf(z_low)
+    return prob
+
+
 def mse(y_true, y_predict):
     '''
     计算均方误差MSE
 
     Parameters
     ----------
     y_true : np.array, pd.Series
@@ -1257,14 +1270,95 @@
     #                     get_pct_loc(value, values, isnew=True, method=method)
     df['PctLoc'] = df['v'].rolling(lag).apply(lambda x:
               get_pct_loc(x.iloc[-1], x.iloc[:-1], isnew=True, method=method))
     df.index = ori_idx
     return df['PctLoc']
 
 
+def mean_update_inrc(v, mean, n):
+    '''均值增量更新算法(根据新值v和已知均值mean，已知技术n计算新的均值)'''
+    res = (mean * n + v) / (n+1)
+    # res = mean + (v - mean) / (n+1)
+    return res
+
+
+def robbins_morno(vals, alphas=None, mean_init=0):
+    '''Robbins-Monro算法'''
+    n = len(vals)
+    if isnull(alphas):
+        alphas = [1/k for k in range(1, n+1)]
+    m = mean_init
+    for k in range(n):
+        m += alphas[k] * (vals[k] - m)
+    return m
+
+
+def vif(df: pd.DataFrame,
+        cols: list = None,
+        const: bool = False,
+        method: int = 1):
+    '''
+    计算VIF（经测试method=1比method=2快三倍左右）
+    
+    Examples
+    --------
+    >>> df = pd.DataFrame({
+    >>>          'a': [1, 1, 2, 3, 4],#, 5, 8, 19],
+    >>>          'b': [2, 2, 3, 2, 1],#, 6, 9, 20],
+    >>>          'c': [4, 6, 7, 8, 9],#, 7, 3, 1],
+    >>>          'd': [4, 3, 4, 5, 4],#, 4, 9, 30]
+    >>>          })
+    >>> vif(df)
+    {'a': 22.949999999999942,
+     'b': 2.9999999999999964,
+     'c': 12.949999999999967,
+     'd': 2.9999999999999964}
+    >>> vif(df, method=2)
+    {'const': 136.87499999999918,
+     'a': 22.949999999999985,
+     'b': 2.9999999999999987,
+     'c': 12.950000000000006,
+     'd': 3.0000000000000107}
+    >>> vif(df, const=True)
+    {'const': 136.87499999999923,
+     'a': 22.949999999999942,
+     'b': 2.9999999999999964,
+     'c': 12.949999999999967,
+     'd': 2.9999999999999964}
+    
+    References
+    ----------
+    - https://www.zhihu.com/question/270451437/answer/405814593
+    - https://javaforall.cn/135202.html
+    '''
+    if isnull(cols):
+        cols = list(df.columns)
+    df = df[cols]
+    # 方式1，用变量相关系数矩阵的逆矩阵的对角元
+    if method == 1:
+        # rowvar=False表示每列为一个变量，每行为一个样本
+        res = {}
+        if const:
+            x = df.mean().to_frame()
+            x_ = x.transpose()
+            s = np.linalg.inv(np.cov(df, rowvar=False, ddof=0))
+            res = {'const': 1 + np.dot(np.dot(x_, s), x)[0][0]}
+        corr = np.corrcoef(df, rowvar=False)
+        res_ = np.linalg.inv(corr).diagonal()
+        res.update(dict(zip(cols, res_)))
+    elif method == 2:
+        X = add_constant(df)
+        res = [variance_inflation_factor(X.values, i) \
+               for i in range(X.shape[1])]
+        res = dict(zip(X.columns, res))
+    else:
+        raise ValueError('未知别的`method`(只能为1或2)!')
+    return res
+
+
 def parms_est():
     '''各种分布不同方法的参数估计，待实现'''
     raise NotImplementedError
 
 
 def auc():
     '''计算auc，待实现'''
```

### Comparing `dramkit-0.5.44/dramkit/datsci/time_series.py` & `dramkit-0.5.45/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/topsis.py` & `dramkit-0.5.45/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.45/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/datsci/utils_ml.py` & `dramkit-0.5.45/dramkit/datsci/utils_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     return stats.mode(all_preds, axis=1)[0].reshape((-1,))
 
 
 def vote_prob_multi(prob_pred_list):
     '''
     | 投票法生成最终多分类label
     | prob_pred_list为不同预测结果列表，
-      每个预测结果是值为概率的np.array或pd.Series，shape为样本数*类别数
+      每个预测结果是值为概率的np.array或pd.DataFrame，shape为样本数*类别数
     '''
-    probs_sum = sum(prob_pred_list)
+    probs_sum = sum([np.array(x) for x in prob_pred_list])
     return probs_sum.argmax(axis=1)
 
 
 def vote_prob_bin_pcut(prob_pred_list, pcut=0.5):
     '''
     | 投票法生成最终二分类label
     | prob_pred_list为不同预测结果列表，
@@ -56,15 +56,15 @@
     '''
     probs_sum = sum(prob_pred_list)
     label = np.zeros(probs_sum.shape)
     label[np.where(probs_sum >= np.quantile(probs_sum, 1-rate1))] = 1
     return label
 
 
-def auc_bin(y_true, pred_prob, **kwargs):
+def cal_auc(y_true, pred_prob, **kwargs):
     '''
     | 二分类AUC计算
     | y_true为真实标签，pred_prob为预测概率（取y_true中较大值的概率）
     | \**kwargs可设置sklearn.metrics.roc_auc_score函数接收的其它参数
     '''
     return roc_auc_score(y_true, pred_prob, **kwargs)
```

### Comparing `dramkit-0.5.44/dramkit/datsci/zigzag.py` & `dramkit-0.5.45/dramkit/datsci/zigzag.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.45/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/gentools.py` & `dramkit-0.5.45/dramkit/gentools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 # -*- coding: utf-8 -*-
 
 '''
 General toolboxs
 '''
 
-import re
-import sys
-import time
+import argparse
 import copy
-import string
+import datetime
 import inspect
+import logging
 import operator
-import argparse
-import datetime
+import re
+import string
+import sys
+import time
 import traceback
-import numpy as np
-import pandas as pd
 import urllib.parse
-from tqdm import tqdm
-from io import StringIO
-from itertools import product
 from collections import Counter
+from collections.abc import Callable, Iterable
 from functools import reduce, wraps
+from io import StringIO
+from itertools import product
 from random import randint, random, uniform
-from collections.abc import Iterable, Callable
-from typing import Union, NewType, Literal, Any
-from dramkit.logtools.utils_logger import logger_show
-from dramkit.speedup.multi_thread import SingleThread
+from typing import Any, Literal, NewType, Union
 
+import numpy as np
+import pandas as pd
 from beartype import beartype as checkin
 from beartype.typing import List
+from tqdm import tqdm
 
+from dramkit.logtools.utils_logger import logger_show
+from dramkit.speedup.multi_thread import SingleThread
 
-PYTHON_VERSION = float(sys.version[:3])
+PYTHON_VERSION = '.'.join([x.zfill(2) for x in sys.version.split(' ')[0].split('.')])
 
 
 class TimeRecoder(object):
     '''
     运行时间记录器
     
     Examples
@@ -92,18 +93,14 @@
         
     def usedm(self, logger=None):
         self.end_tm = self.now()
         s = self.end_tm - self.strt_tm
         m = round(s/60, 6)
         logger_show('used time: %sm.'%m, self._check_logger(logger))
         return s
-    
-    
-class DirtModifyError(Exception):
-    pass
 
 
 class GenObject(object):
     '''
     | 创建一个数据类型，用于存放变量值，
     | 既可以用.key调用，也可以像字典一样调用[key]调用
     '''
@@ -126,17 +123,16 @@
         _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
         if key in _defaults:
             self.__dict__[key] = value
             return
         if self.dirt_modify:
             self.__dict__[key] = value
         else:
-            # raise DirtModifyError('不允许直接赋值！')
-            raise DirtModifyError(
-                  '不允许直接赋值，请调用`set_key_value`或`set_from_dict`方法！')
+            # raise_error('DirtModifyError', '不允许直接赋值！')
+            raise_error('DirtModifyError', '不允许直接赋值，请调用`set_key_value`或`set_from_dict`方法！')
 
     def __repr__(self):
         '''查看时以key: value格式打印'''
         _defaults = ['__dirt_modify']
         _defaults = ['_%s'%type(self).__name__ + x for x in _defaults]
         return ''.join('{}: {}\n'.format(k, v) for k, v in self.__dict__.items() \
                        if k not in _defaults)
@@ -210,23 +206,19 @@
     def remove(self, key):
         '''删除属性变量key，无返回'''
         del self.__dict__[key]
 
     def clear(self):
         '''清空所有属性变量'''
         self.__dict__.clear()
-        
-        
-class DeprecatedError(Exception):
-    pass
 
 
 class StructureObject(object):
     def __init__(self, *args, **kwargs):
-        raise DeprecatedError('`StructureObject`已弃用，请调用`GenObject`!')
+        raise_error('DeprecatedError', '`StructureObject`已弃用，请调用`GenObject`!')
         
         
 def run_func_with_timeout_thread(func, *args,
                                  timeout=10,
                                  logger_error=False,
                                  logger_timeout=None,
                                  timeout_show_str=None,
@@ -415,14 +407,50 @@
                     if sleep_seconds > 0:
                         time.sleep(sleep_seconds)
                 return result
         return repeater
     return transfunc
 
 
+def raise_error(name: str,
+                msg: str,
+                logger: logging.Logger = None,
+                code: Union[int, str] = None):
+    '''
+    | 抛出异常
+    | name异常名称、msg异常信息、code异常代码、logger日志记录器
+    
+    Examples
+    --------
+    >>> from dramkit import simple_logger
+    >>> logger = simple_logger('./_test/test_raise_error.log', 'a')    
+    >>> raise_error('MyError1', 'test myerror', logger=logger)
+    >>> raise_error('MyError2', 'test myerror', logger=logger, code=1)
+    '''
+    exec('class {}(Exception): pass'.format(name))
+    try:
+        exec('raise {}("{}")'.format(name, msg))
+    except:
+        emsg = traceback.format_exc()
+        if not isnull(code):
+            emsg = 'ErrorCode: %s\n'%code + emsg
+        logger_show(emsg, logger=logger,
+                    level='err', err_exc_info=False)
+        raise
+        
+        
+class RaiseError(object):
+    
+    def __init__(self, logger=None):
+        self.logger = logger
+        
+    def raise_error(self, name, msg, code=None):
+        raise_error(name, msg, logger=self.logger, code=code)
+
+
 def catch_error(logger=None, raise_error=True):
     '''
     作为装饰器捕获函数运行错误
     
     Parameters
     ----------
     logger : None, logging.Logger
@@ -1090,14 +1118,18 @@
     [56.867261610484356, 83.13273838951565]
     >>> rand_weight_sum(80, 2, [20, 10], [100, 90])
     [80.32071140116187, 79.67928859883813]
     >>> rand_weight_sum(80, 2, [20, 10], [100, 90], [0.6, 0.4])
     [88.70409567475888, 66.94385648786168]
     >>> rand_weight_sum(180, 2, [20, 10], [100, 90], [3, 2])
     [23.080418085462018, 55.37937287180697]
+    >>> rand_sum(1, 4, 0, 1)
+    [0, 1, 0, 0]
+    >>> print([round(x, 4) for x in rand_sum(1, 4, 0.0, 1.0)])
+    [0.1896, 0.1913, 0.0797, 0.5394]
     '''
 
     if weights is not None and len(weights) != n:
         raise ValueError('权重列表W的长度必须等于n！')
     if not (isinstance(lowests, int) or isinstance(lowests, float)):
         if len(lowests) != n:
             raise ValueError('下限值列表(数组)lowests长度必须与n相等！')
@@ -2513,14 +2545,18 @@
                 if pd.isnull(x):
                     return True
             except:
                 pass
     return False
 
 
+def isna(*args, **kwargs):
+    return isnull(*args, **kwargs)
+
+
 def x_div_y(x, y, v_x0=None, v_y0=0, v_xy0=1):
     '''
     x除以y
 
     - v_xy0为当x和y同时为0时的返回值
     - v_y0为当y等于0时的返回值
     - v_x0为当x等于0时的返回值
@@ -2837,18 +2873,18 @@
 @checkin
 def get_full_df(df: pd.DataFrame,
                 full_col : str,
                 fulls: Iterable,
                 idcols: Union[str, List[str], None] = None,
                 vcols: Union[str, List[str], None] = None,
                 val_nan: Any = None,
-                fill: Union[FillMethodType, None] = 'ffill',
+                fill: Union[FillMethodType, None, bool] = 'ffill',
                 final_dropna: bool = True,
                 only_fulls: bool = True,
-                method: FullMethodType = 'pivot'):
+                method: FullMethodType = 'product'):
     '''
     df中full_col列的值扩充到fulls
     
     Example
     -------
     >>> df = pd.DataFrame({'t': [2, 3, 5, 7, 9],
     ...                    'a': ['x1', 'x1', 'x3', 'x4', 'x4'],
@@ -2882,14 +2918,17 @@
         if final_dropna:
             res = res.dropna()
     else:
         # 受影响的列
         vcols = check_list_arg(vcols, allow_none=True)
         if isnull(vcols):
             vcols = [x for x in df.columns if not x in idcols+[full_col]]
+        assert all([not x in vcols for x in idcols])
+        assert not full_col in vcols
+        assert not full_col in idcols
         res = df[[full_col]+idcols+vcols].copy()
         if not isnull(val_nan):
             for c in vcols:
                 res[c] = res[c].fillna(val_nan)
         oncols = [full_col]+idcols
         assert res[oncols].isna().sum().sum() == 0
         if method == 'product':
@@ -3336,15 +3375,15 @@
     >>> b = [4, 5, 6]
     >>> c = ['a', 'b']
     >>> d = [a, b]
     >>> link_lists([a, b, c, d])
     [1, 2, 3, 4, 5, 6, 'a', 'b', [1, 2, 3], [4, 5, 6]]
     '''
     assert isinstance(lists, (list, tuple))
-    assert all([isinstance(x, list) for x in lists])
+    assert all([isinstance(x, (list, tuple)) for x in lists])
     newlist = []
     for item in lists:
         newlist.extend(item)
     return newlist
 
 
 def get_lists_inter(lists):
@@ -3417,19 +3456,50 @@
 
 def count_list(l):
     '''对l中的元素计数，返回dict'''
     # return dict(Counter(l))
     return Counter(l)
 
 
+def _get_label_bins_range(bins, labels):
+    assert len(labels) == (len(bins)-1)
+    res = {}
+    for k in range(len(labels)):
+        l = labels[k]
+        res[l] = (bins[k], bins[k+1])
+    return res
+
+
+def get_label_bins_range(bins, labels,
+                         left_close=False,
+                         right_close=False):
+    assert isinstance(bins, (list, tuple))
+    assert isinstance(labels, (list, tuple))
+    if (not left_close) and (not right_close):
+        assert len(labels) == (len(bins)+1)
+        return _get_label_bins_range(
+                [-np.inf]+bins+[np.inf], labels)
+    elif left_close and right_close:
+        return _get_label_bins_range(bins, labels)
+    else:
+        assert len(labels) == len(bins)
+        if left_close:
+            return _get_label_bins_range(bins+[np.inf], labels)
+        else:
+            return _get_label_bins_range([-np.inf]+bins, labels)
+    
+
 def tmprint(*args, **kwargs):
     print(*args, **kwargs)
     print('    [time: {}]'.format(
         datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S.%f')))
-
+    
+    
+def fmt(fstr, *args, **kwargs):
+    return fstr.format(*args, **kwargs)
 
 def url2chn(url):
     '''将url中的中文乱码（实际上为utf-8）转化为正常url'''
     return urllib.parse.unquote(url)
 
 
 def replace_con_blank(string, to):
@@ -3585,16 +3655,16 @@
     else:
         res = df.apply(lambda x:
                  x.nsmallest(n).index.tolist(), axis=axis)
     return res
     
 
 if __name__ == '__main__':
-    from dramkit import load_csv, plot_series
     from finfactory.fintools.fintools import cci
+    from dramkit import load_csv, plot_series
     
     tr = TimeRecoder()
     def test():
         # 50ETF日线行情------------------------------------------------------------
         fpath = './_test/510050.SH_daily_qfq.csv'
         data = load_csv(fpath)
         data.set_index('date', drop=False, inplace=True)
```

### Comparing `dramkit-0.5.44/dramkit/install_check.py` & `dramkit-0.5.45/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/iotools.py` & `dramkit-0.5.45/dramkit/iotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # -*- coding: utf-8 -*-
 
-import re
-import os
-import sys
-import time
+import inspect
 import json
-import yaml
+import logging
+import os
 import pickle
+import platform
+import py_compile
+import re
 import shutil
-import logging
-import zipfile
 import socket
-import inspect
-import platform
-import requests
-import traceback
 import subprocess
-import py_compile
-import pandas as pd
-from tqdm import tqdm
+import sys
+import time
+import traceback
+import zipfile
 from pathlib import Path
 from urllib.request import urlopen
-from dramkit.gentools import (isnull,
-                              check_list_arg,
-                              get_update_kwargs,
+
+import pandas as pd
+import requests
+import yaml
+from tqdm import tqdm
+
+from dramkit.datetimetools import timestamp2str
+from dramkit.gentools import (check_list_arg,
                               cut_range_to_subs,
                               get_tmp_col,
+                              get_update_kwargs,
+                              isnull,
                               merge_df,
+                              run_func_with_timeout_thread,
                               update_df,
-                              run_func_with_timeout_thread)
-from dramkit.logtools.utils_logger import (logger_show,
-                                           close_log_file)
-from dramkit.datetimetools import timestamp2str
+                              raise_error,
+                              fmt)
+from dramkit.logtools.utils_logger import close_log_file, logger_show
 from dramkit.speedup.multi_process_concurrent import multi_process_concurrent
 
 _WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
 _SP = ' '
 _CR = '\r'
 _LF = '\n'
@@ -201,31 +204,42 @@
     file : str
         待读取文件路径
     '''
     with open(file, 'rb') as f:
         return pickle.load(f)
     
     
-def load_yml(fpath, **kwargs_open):
+def _load_yml(fpath, **kwargs_open):
     '''
     | 读取yml文件内容
     | 参考：
     | https://blog.csdn.net/qq_33106045/article/details/108507775
     '''
     with open(fpath, **kwargs_open) as f:
         data = yaml.load(f.read(), Loader=yaml.FullLoader)
     return data
+
+
+def load_yml(*args, **kwargs):
+    if 'encoding' not in kwargs:
+        for en in ['utf-8', None, 'gbk']:
+            try:
+                kwargs.update({'encoding': en})
+                return _load_yml(*args, **kwargs)
+            except:
+                pass
+    return _load_yml(*args, **kwargs)
     
     
 def write_yml():
     '''写入yml文件'''
     raise NotImplementedError
 
 
-def load_json(fpath, encoding=None, logger=None):
+def load_json(fpath, encoding=None, logger=None, **kwargs_open):
     '''
     读取json格式文件
 
     Parameters
     ----------
     fpath : str
         待读取文件路径
@@ -238,26 +252,27 @@
     :returns: `dict` - 返回读取数据
     '''
 
     if not os.path.exists(fpath):
         logger_show('文件不存在，返回None：{}'.format(fpath),
                     logger, 'warn')
         return None
-                
-    for en in [encoding, 'utf-8', 'gbk', None]:
+    
+    ens = [encoding] + list({'utf-8', None, 'gbk'}-{encoding})
+    for en in ens:
         try:
-            with open(fpath, 'r', encoding=en) as f:
+            with open(fpath, 'r', encoding=en, **kwargs_open) as f:
                 data_json = json.load(f)
-            break
+            return data_json
         except:
-            logger_show('读取%s出错，请检查文件（如编码或文件末尾多余字符等问题）！'%fpath,
-                        logger, 'error')
-            raise
-
-    return data_json
+            pass
+        
+    raise_error('JsonFileError',
+                fmt('读取{}出错，请检查文件（如编码或文件末尾多余字符等问题）！', fpath),
+                logger=logger)
 
 
 def write_json(data, fpath, encoding=None, mode='w', **kwargs):
     '''
     把data写入json格式文件
 
     Parameters
@@ -286,30 +301,26 @@
         文件编码格式，若不指定，则尝试用utf-8和gbk编码读取
     logger : None, logging.Logger
         日志记录器
 
 
     :returns: `list` - 文本文件中每行内容列表
     '''
-    try:
-        with open(fpath, 'r', encoding=encoding, **kwargs_open) as f:
-            lines = f.readlines() if split else f.read()
-    except:
+    ens = [encoding] + list({'utf-8', None, 'gbk'}-{encoding})
+    for en in ens:
         try:
-            with open(fpath, 'r', encoding='utf-8', **kwargs_open) as f:
+            with open(fpath, 'r', encoding=en, **kwargs_open) as f:
                 lines = f.readlines() if split else f.read()
+            return lines
         except:
-            try:
-                with open(fpath, 'r', encoding='gbk', **kwargs_open) as f:
-                    lines = f.readlines() if split else f.read()
-            except:
-                logger_show('未正确识别文件编码格式，以二进制读取: %s'%fpath,
-                            logger, 'warn')
-                with open(fpath, 'rb', **kwargs_open) as f:
-                    lines = f.readlines() if split else f.read()
+            pass
+    logger_show('未正确识别文件编码格式，以二进制读取: %s'%fpath,
+                logger, 'warn')
+    with open(fpath, 'rb', **kwargs_open) as f:
+        lines = f.readlines() if split else f.read()
     return lines
 
 
 def write_txt(lines, file, mode='w', check_end=True, **kwargs):
     '''
     将列表lines中的内容写入文本文件中
 
@@ -517,15 +528,16 @@
     _big = False
     if 'chunksize' in kwargs and not isnull(kwargs['chunksize']):
         _big = True
         chunksize, kwargs = get_update_kwargs(
             'chunksize', None, kwargs, func_update=False)
 
     data = None
-    for en in [encoding, 'utf-8', 'gbk']:
+    ens = [encoding] + list({'utf-8', None, 'gbk'}-{encoding})
+    for en in ens:
         try:
             if not _big:
                 data = read_func(fpath, encoding=en, **kwargs)
             else:
                 kwargs.update({'encoding': en})
                 data = _process_df_pd_big(read_func, fpath,
                                           chunksize=chunksize,
@@ -1953,10 +1965,13 @@
     # TODO: path以'./'开头时，得到的res不是以'./'开头，原因待查
     if path.startswith('./') and not res.startswith('./'):
         res = './' + res
     return res
 
 
 if __name__ == '__main__':
-    fpath = './_test/load_text_test_utf8.csv'
+    # fpath = './_test/load_text_test_utf8.csv'
+    # fpath = './_test/load_text_test_utf8_new.csv'
+    fpath = './_test/load_text_test_gbk.csv'
+    # fpath = './_test/load_text_test_gbk_new.csv'
     data1 = load_text(fpath, encoding='gbk')
-    data2 = load_csv(fpath, encoding='gbk')
+    data2 = load_csv(fpath, encoding='utf-8')
```

### Comparing `dramkit-0.5.44/dramkit/logtools/logger_general.py` & `dramkit-0.5.45/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.45/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.45/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/logtools/utils_logger.py` & `dramkit-0.5.45/dramkit/logtools/utils_logger.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.45/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/openai/openai_chat.py` & `dramkit-0.5.45/dramkit/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.45/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/alo.py` & `dramkit-0.5.45/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.45/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/boa.py` & `dramkit-0.5.45/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/cs.py` & `dramkit-0.5.45/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/ga.py` & `dramkit-0.5.45/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/gwo.py` & `dramkit-0.5.45/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.45/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/hho.py` & `dramkit-0.5.45/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.45/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/pso.py` & `dramkit-0.5.45/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.45/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/optimizer/woa.py` & `dramkit-0.5.45/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/_Git_notes.py` & `dramkit-0.5.45/dramkit/other/_Git_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/_Linux_notes.py` & `dramkit-0.5.45/dramkit/other/_Linux_notes.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 # Linux笔记
 
 linux_notes = \
 r'''
 # 参考
 https://blog.csdn.net/changlina_1989/article/details/111144018
 
+# Linux查看当前操作系统版本信息
+cat /proc/version
+# Linux查看版本当前操作系统内核信息
+uname -a
+
 # 命令行运行python并将输出保存日志
 # 日志覆盖：
 python -u xxx.py > xxx.log 2>&1 &
 # 日志追加：
 python -u xxx.py >> xxx.log 2>&1 &
 
 # 后台运行不记录日志
```

### Comparing `dramkit-0.5.44/dramkit/other/_Python_notes.py` & `dramkit-0.5.45/dramkit/other/_Python_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/_Vim_notes.py` & `dramkit-0.5.45/dramkit/other/_Vim_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/debt_cal.py` & `dramkit-0.5.45/dramkit/other/debt_cal.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 
 import numpy as np
 import numpy_financial as npf
 import pandas as pd
 from typing import Union, List
 
 
+def calc_perfect_house_price(month_income,
+                             area=40,
+                             rate=0.3,
+                             debt_year=30):
+    '''
+    | 不考虑其它因素，根据人均月收入month_income、人均住房面积area（平米）、
+    | 房价占收入比rate和还款年限debt_year计算合理的房价（元/平米）
+    '''
+    return ((month_income*12*debt_year)*rate) / area
+
+
 class DebtCal():
     '''
     贷款计算器
     '''
     
     def __init__(self,
                  corpus: float,
```

### Comparing `dramkit-0.5.44/dramkit/other/langconv.py` & `dramkit-0.5.45/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/othertools.py` & `dramkit-0.5.45/dramkit/other/othertools.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,16 +198,18 @@
     if isnull(pkgs):
         pkgs = ['DramKit', 'FinFactory', 'ChnCal']
     if isinstance(pkgs, str):
         pkgs = [pkgs]
     pkg_paths = [x for x in sys.path if any([y in os.path.basename(x) for y in pkgs])]
     files = []
     for fdir in pkg_paths:
+        if not 'file_types' in kwargs:
+            kwargs.update({'file_types': '.py'})
         files.append(find_dir_include_str(tgt_str, root_dir=fdir,
-                                          file_types='.py', **kwargs))
+                                          **kwargs))
     files = pd.concat(files, axis=0)
     return files
 
 
 def _drop_pypkgs_dir(dirname='__pycache__', pkgs=None, **kwargs):
     pkgs = check_list_arg(pkgs, allow_none=True)
     if isnull(pkgs):
```

### Comparing `dramkit-0.5.44/dramkit/other/replace_endblank.py` & `dramkit-0.5.45/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/other/zh_wiki.py` & `dramkit-0.5.45/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/plottools/plot_barline.py` & `dramkit-0.5.45/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/plottools/plot_common.py` & `dramkit-0.5.45/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.45/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.45/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/plottools/utils_plot.py` & `dramkit-0.5.45/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.45/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.45/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.45/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sorts/insert_sort.py` & `dramkit-0.5.45/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.45/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sorts/quick_sort.py` & `dramkit-0.5.45/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/speedup/_mp_test1.py` & `dramkit-0.5.45/dramkit/speedup/_mp_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/speedup/_mp_test2.py` & `dramkit-0.5.45/dramkit/speedup/_mp_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/speedup/_mp_test3.py` & `dramkit-0.5.45/dramkit/speedup/_mp_test3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/speedup/iotools_tmp.py` & `dramkit-0.5.45/dramkit/speedup/iotools_tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/speedup/multi_process_concurrent.py` & `dramkit-0.5.45/dramkit/speedup/multi_process_concurrent.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 _WINDOWS_SYSTEM = 'windows' in platform.system().lower()
 
 #%%
 @print_used_time
 def multi_process_concurrent(func, args_list,
                              keep_order=True,
-                             multi_line=None):
+                             multi_line=None,
+                             **kwargs):
     '''
     多进程，同一个函数执行多次
 
     Parameters
     ----------
     func : function
         需要多进程运行的目标函数
@@ -41,27 +42,27 @@
     Note
     ----
     该函数通过import导入在Windows下会出错
     '''
 
     if multi_line is None:
         multi_line = len(args_list)
-
+    
     # submit方法不能保证results的值顺序与args_list一一对应
     if not keep_order:
         with ProcessPoolExecutor(max_workers=multi_line) as executor:
             futures = [executor.submit(func, *args) for args in args_list]
 
         results = []
         for future in as_completed(futures):
             result = future.result()
             results.append(result)
 
     # 使用map可保证results的值顺序与args_list一一对应
-    if keep_order:        
+    if keep_order:      
         with ProcessPoolExecutor(max_workers=multi_line) as executor:
             results = executor.map(func, args_list)
             results = list(results)
 
     return results
 
 #%%
@@ -87,18 +88,18 @@
         print('task id: {}; slept: {}s.'.format(idx, sleep_tm))
         return [idx, sleep_tm]
 
     def func_new(args):
         return func(*args)
 
     args_list = [[1, 2], [3, 4], [4, 5], [2, 3]]
-    args_list = [[1, 20], [3, 40], [4, 50], [2, 30]]
+    # args_list = [[1, 20], [3, 40], [4, 50], [2, 30]]
 
 
-    # '''
+    '''
     tmprint('multi-process, concurrent...................')
     tr = TimeRecoder()
     if _WINDOWS_SYSTEM:
         results_Order = multi_process_concurrent(_func_test_win_new, args_list,
                                                  keep_order=True)
         results_noOrder = multi_process_concurrent(_func_test_win, args_list,
                                                    keep_order=False)
```

### Comparing `dramkit-0.5.44/dramkit/speedup/multi_thread.py` & `dramkit-0.5.45/dramkit/speedup/multi_thread.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.45/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.45/dramkit/sqltools/_MySQL_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.45/dramkit/sqltools/_Oracle_notes.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,7 +171,30 @@
 SELECT COLUMN_NAME, DATA_TYPE, DATA_LENGTH, NULLABLE
 FROM user_tab_columns
 WHERE table_name = UPPER('TABLE_NAME大写');
 
 # '''
 
 
+install_12c_linux = r'''
+-- https://blog.csdn.net/alongliang/article/details/128300006
+# '''
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `dramkit-0.5.44/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.45/dramkit/sqltools/cxoracle.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/py_hive.py` & `dramkit-0.5.45/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.45/dramkit/sqltools/py_mysql.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.45/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/webtools/utils_html.py` & `dramkit-0.5.45/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit/wechat/qywechat.py` & `dramkit-0.5.45/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.44/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.45/dramkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.44
+Version: 0.5.45
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.44/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.45/dramkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,23 +19,25 @@
 dramkit/_tmp/PIDtest.py
 dramkit/_tmp/PIDtest2.py
 dramkit/_tmp/VMD.py
 dramkit/_tmp/__init__.py
 dramkit/_tmp/cca_test.py
 dramkit/_tmp/dtw_test.py
 dramkit/_tmp/explore.py
+dramkit/_tmp/feature_selection.py
 dramkit/_tmp/gini.py
 dramkit/_tmp/merge_sort.py
 dramkit/_tmp/mouse_move.py
 dramkit/_tmp/mpc_test1.py
 dramkit/_tmp/options_Implied_volatility.py
 dramkit/_tmp/pf_test.py
 dramkit/_tmp/plot_test.py
 dramkit/_tmp/plot_test2.py
 dramkit/_tmp/simple_smooth.py
+dramkit/_tmp/step_reg.py
 dramkit/_tmp/test_async_washs.py
 dramkit/_tmp/test_await_timeout.py
 dramkit/_tmp/test_backtrader.py
 dramkit/_tmp/test_chatgpt_v1.py
 dramkit/_tmp/test_code.py
 dramkit/_tmp/test_find_peaks.py
 dramkit/_tmp/test_get_var_name.py
@@ -51,52 +53,47 @@
 dramkit/_tmp/tfDNNCls_test.py
 dramkit/_tmp/tmp.py
 dramkit/_tmp/tmp_args.py
 dramkit/_tmp/transformer_pytorch.py
 dramkit/_tmp/utils_SignalDec.py
 dramkit/_tmp/utils_TimeSeries.py
 dramkit/_tmp/utils_lottery.py
-dramkit/_tmp/utils_rl.py
-dramkit/_tmp/utils_rl2.py
-dramkit/_tmp/utils_rl3.py
-dramkit/_tmp/utils_rl4.py
-dramkit/_tmp/utils_rl5.py
-dramkit/_tmp/utils_rl6.py
-dramkit/_tmp/utils_rl7.py
 dramkit/_tmp/utils_sem.py
 dramkit/backpacks/__init__.py
 dramkit/backpacks/backpack01_float_dy.py
 dramkit/backpacks/backpack01_int_dy.py
 dramkit/chncal/__init__.py
 dramkit/chncal/apis.py
 dramkit/chncal/constants.py
 dramkit/chncal/constants_fate.py
 dramkit/chncal/constants_hko.py
 dramkit/chncal/constants_trade_dates.py
 dramkit/chncal/constants_wuxing.py
 dramkit/chncal/constants_zodiac_marry.py
 dramkit/chncal/solar_terms.py
 dramkit/datsci/__init__.py
+dramkit/datsci/_rl_mab.py
+dramkit/datsci/_rl_markov.py
+dramkit/datsci/_rl_mcdp.py
 dramkit/datsci/_utils_ann.py
 dramkit/datsci/activate_funcs.py
 dramkit/datsci/ahp.py
 dramkit/datsci/ahp_sim_ri.py
 dramkit/datsci/apriori.py
 dramkit/datsci/curvature.py
 dramkit/datsci/elm_cls.py
 dramkit/datsci/elm_reg.py
 dramkit/datsci/entropy_weight.py
 dramkit/datsci/find_maxmin.py
 dramkit/datsci/freq_item_set.py
 dramkit/datsci/lr.py
 dramkit/datsci/preprocess.py
-dramkit/datsci/rl_markov.py
-dramkit/datsci/rl_markov_linprog.py
-dramkit/datsci/rl_markov_sympy.py
+dramkit/datsci/rl_markov_new.py
 dramkit/datsci/stats.py
+dramkit/datsci/stepreg.py
 dramkit/datsci/time_series.py
 dramkit/datsci/topsis.py
 dramkit/datsci/utils_lgb.py
 dramkit/datsci/utils_ml.py
 dramkit/datsci/zigzag.py
 dramkit/find_addends/__init__.py
 dramkit/find_addends/find_addends_backpack01float.py
@@ -138,28 +135,30 @@
 dramkit/other/replace_endblank.py
 dramkit/other/zh_wiki.py
 dramkit/plottools/__init__.py
 dramkit/plottools/plot_barline.py
 dramkit/plottools/plot_common.py
 dramkit/plottools/plot_histdist.py
 dramkit/plottools/plot_scatter.py
+dramkit/plottools/twinx_align.py
 dramkit/plottools/utils_plot.py
 dramkit/pystyles/__init__.py
 dramkit/pystyles/dramkit_style.py
 dramkit/sorts/__init__.py
 dramkit/sorts/bubble_sort.py
 dramkit/sorts/bucket_sort.py
 dramkit/sorts/insert_sort.py
 dramkit/sorts/insert_sort_bin.py
 dramkit/sorts/quick_sort.py
 dramkit/speedup/__init__.py
 dramkit/speedup/_mp_test1.py
 dramkit/speedup/_mp_test2.py
 dramkit/speedup/_mp_test3.py
 dramkit/speedup/iotools_tmp.py
+dramkit/speedup/job_lib.py
 dramkit/speedup/multi_process_concurrent.py
 dramkit/speedup/multi_thread.py
 dramkit/sqltools/_Hive_notes.py
 dramkit/sqltools/_MySQL_notes.py
 dramkit/sqltools/_Oracle_notes.py
 dramkit/sqltools/__init__.py
 dramkit/sqltools/cxoracle.py
```

### Comparing `dramkit-0.5.44/setup.py` & `dramkit-0.5.45/setup.py`

 * *Files identical despite different names*

