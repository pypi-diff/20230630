# Comparing `tmp/AFR-0.2.2.tar.gz` & `tmp/AFR-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AFR-0.2.2.tar", last modified: Sat Mar 25 14:18:19 2023, max compression
+gzip compressed data, was "dist/AFR-0.2.7.tar", last modified: Fri Jun 30 08:09:23 2023, max compression
```

## Comparing `AFR-0.2.2.tar` & `AFR-0.2.7.tar`

### file list

```diff
@@ -1,40 +1,23 @@
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.750142 AFR-0.2.2/
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.741842 AFR-0.2.2/AFR/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      815 2023-03-25 14:17:44.000000 AFR-0.2.2/AFR/__init__.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      956 2023-03-23 18:06:27.000000 AFR-0.2.2/AFR/adjr2_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      997 2023-03-23 17:39:30.000000 AFR-0.2.2/AFR/aic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1011 2023-03-23 17:39:47.000000 AFR-0.2.2/AFR/bic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2112 2023-03-23 17:57:07.000000 AFR-0.2.2/AFR/check_betas.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2302 2023-03-22 14:08:47.000000 AFR-0.2.2/AFR/checkdata.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2165 2023-03-23 10:29:48.000000 AFR-0.2.2/AFR/corsel.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      768 2023-03-23 16:57:47.000000 AFR-0.2.2/AFR/dec_plot.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      298 2023-03-25 14:06:07.000000 AFR-0.2.2/AFR/finratKZ.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      275 2023-03-25 14:06:07.000000 AFR-0.2.2/AFR/macroKZ.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1225 2023-03-23 14:36:17.000000 AFR-0.2.2/AFR/opt_size.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1331 2023-03-20 10:35:47.000000 AFR-0.2.2/AFR/pt_multi.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1171 2023-03-20 10:23:59.000000 AFR-0.2.2/AFR/pt_one.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1275 2023-03-23 16:54:05.000000 AFR-0.2.2/AFR/reg_test.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     3852 2023-03-20 06:19:52.000000 AFR-0.2.2/AFR/regsel_f.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1039 2023-03-23 17:41:23.000000 AFR-0.2.2/AFR/sbic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      962 2023-03-06 09:18:06.000000 AFR-0.2.2/AFR/vif_reg.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13441 2023-03-25 12:01:16.000000 AFR-0.2.2/AFR manual.md
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.743624 AFR-0.2.2/AFR.egg-info/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13849 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      669 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/SOURCES.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/dependency_links.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/requires.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        4 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/top_level.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.2/LICENSE.rtf
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      111 2023-03-25 13:53:52.000000 AFR-0.2.2/MANIFEST.in
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13849 2023-03-25 14:18:19.749833 AFR-0.2.2/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.2/example_process.ipynb
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.748867 AFR-0.2.2/load/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    62368 2023-02-28 05:06:29.000000 AFR-0.2.2/load/finratKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    10137 2023-02-28 06:28:15.000000 AFR-0.2.2/load/finratKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1843 2023-03-15 10:12:56.000000 AFR-0.2.2/load/finratKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    18665 2023-03-01 15:07:14.000000 AFR-0.2.2/load/macroKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13295 2023-02-27 21:25:57.000000 AFR-0.2.2/load/macroKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     4178 2023-02-27 21:25:57.000000 AFR-0.2.2/load/macroKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      133 2023-03-25 05:55:12.000000 AFR-0.2.2/requirements.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-03-25 14:18:19.750238 AFR-0.2.2/setup.cfg
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      981 2023-03-25 14:17:23.000000 AFR-0.2.2/setup.py
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 08:09:23.732329 AFR-0.2.7/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 08:09:23.717356 AFR-0.2.7/AFR/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 08:09:23.724212 AFR-0.2.7/AFR/AFR.egg-info/
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-30 08:09:23.000000 AFR-0.2.7/AFR/AFR.egg-info/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      402 2023-06-30 08:09:23.000000 AFR-0.2.7/AFR/AFR.egg-info/SOURCES.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-30 08:09:23.000000 AFR-0.2.7/AFR/AFR.egg-info/dependency_links.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-06-30 08:09:23.000000 AFR-0.2.7/AFR/AFR.egg-info/requires.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-30 08:09:23.000000 AFR-0.2.7/AFR/AFR.egg-info/top_level.txt
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-30 08:09:23.731023 AFR-0.2.7/AFR/load/
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    62311 2023-06-21 10:38:03.000000 AFR-0.2.7/AFR/load/finratKZ.csv
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    10137 2023-02-28 06:28:15.000000 AFR-0.2.7/AFR/load/finratKZ_dataset.html
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1843 2023-03-15 10:12:56.000000 AFR-0.2.7/AFR/load/finratKZ_dataset.rst
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    19643 2023-06-13 10:48:38.000000 AFR-0.2.7/AFR/load/macroKZ.csv
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13295 2023-03-28 09:46:08.000000 AFR-0.2.7/AFR/load/macroKZ_dataset.html
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     4178 2023-03-28 09:43:27.000000 AFR-0.2.7/AFR/load/macroKZ_dataset.rst
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14541 2023-06-19 13:01:26.000000 AFR-0.2.7/AFR manual.md
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.7/LICENSE.rtf
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      123 2023-06-29 20:01:11.000000 AFR-0.2.7/MANIFEST.in
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-30 08:09:23.731988 AFR-0.2.7/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.7/example_process.ipynb
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      159 2023-06-29 19:54:34.000000 AFR-0.2.7/requirements.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-06-30 08:09:23.732440 AFR-0.2.7/setup.cfg
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      959 2023-06-30 02:55:44.000000 AFR-0.2.7/setup.py
```

### Comparing `AFR-0.2.2/AFR manual.md` & `AFR-0.2.7/AFR/AFR.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: AFR
+Version: 0.2.7
+Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
+Home-page: https://github.com/AFRKZ/AFR
+Author: Timur Abilkassymov, Alua Makhmetova
+Author-email: alua.makhmetova@gmail.com
+License: 3-clause BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE.rtf
+
 # Package ‘AFR’
 
 
 Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data.
 
 It was designed by the team of the Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market (ARDFM).
 
@@ -31,15 +42,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -72,98 +83,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -318,14 +329,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/AFR.egg-info/PKG-INFO` & `AFR-0.2.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AFR
-Version: 0.2.2
+Version: 0.2.7
 Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
 Home-page: https://github.com/AFRKZ/AFR
 Author: Timur Abilkassymov, Alua Makhmetova
 Author-email: alua.makhmetova@gmail.com
 License: 3-clause BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.rtf
@@ -42,15 +42,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -83,98 +83,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -329,14 +329,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/LICENSE.rtf` & `AFR-0.2.7/LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/PKG-INFO` & `AFR-0.2.7/AFR manual.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: AFR
-Version: 0.2.2
-Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
-Home-page: https://github.com/AFRKZ/AFR
-Author: Timur Abilkassymov, Alua Makhmetova
-Author-email: alua.makhmetova@gmail.com
-License: 3-clause BSD
-Description-Content-Type: text/markdown
-License-File: LICENSE.rtf
-
 # Package ‘AFR’
 
 
 Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data.
 
 It was designed by the team of the Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market (ARDFM).
 
@@ -42,15 +31,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -83,98 +72,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -329,14 +318,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/example_process.ipynb` & `AFR-0.2.7/example_process.ipynb`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/load/finratKZ.csv` & `AFR-0.2.7/AFR/load/finratKZ.csv`

 * *Files 0% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 0,1.68,0.78,1.09,5.51,0.85,0.03,97.08,0.23,0.31,1.33,0.47,5.33,-1.21,0.00,-0.63,-0.10,-0.16,-0.20,0.07,0.09,0.04,0.10,0.07,17.89,4.64,186.44,1.57,3.79,3.20
 0,1.40,1.34,2.01,2.51,0.27,0.11,166.65,0.30,0.49,1.63,1.31,58.77,-0.73,0.00,-1.00,-0.12,-0.28,-0.65,0.28,0.67,0.13,0.18,0.16,28.16,2.30,71.82,2.22,76.82,4.14
 0,0.80,0.23,1.20,0.89,0.67,0.11,35.66,0.31,0.84,2.69,0.29,13.52,1.65,27.57,0.44,0.07,0.17,0.40,0.07,0.18,0.03,0.07,0.04,5.21,37.13,8.25,2.56,7.96,-29.18
 0,1.20,1.82,1.59,2.55,0.96,0.01,263.23,0.16,1.22,7.41,0.79,2.75,-0.77,0.00,-0.58,-0.18,-0.10,-0.86,0.06,0.56,0.12,0.68,0.23,2.17,3.85,0.58,0.53,2.92,1.03
 0,1.00,1.00,1.00,6.56,4.70,2.72,33.15,0.01,0.08,11.86,19.50,290.50,-2.26,0.00,-32.51,-0.23,-0.24,-5.11,0.10,2.01,0.09,0.33,0.10,7.62,110.08,20.22,1.07,7.23,1.35
 0,0.31,0.30,1.91,10.63,0.48,0.09,13.96,0.08,0.08,1.09,1.21,0.00,-2.54,0.00,-3.03,-0.51,-0.30,-0.33,0.10,0.10,0.16,0.24,0.20,22.24,0.61,148.71,0.60,6.08,0.57
 0,2.46,5.27,1.15,12.69,2.60,0.39,48.66,0.00,0.00,1.09,1.00,0.00,0.08,0.00,0.00,0.02,0.02,0.03,0.11,0.14,0.10,1.00,0.10,7.50,0.00,0.01,1.16,74.42,1.36
-0,5.64,2.46,4.48,1.20,0.54,0.21,44.43,0.00,0.00,5.90,1.00,0.00,1.77,0.00,0.00,0.10,0.26,1.44,0.12,0.66,0.05,0.10,0.06,9.55,6.76,7.64,2.61,1 284.55,8.91
+0,5.64,2.46,4.48,1.20,0.54,0.21,44.43,0.00,0.00,5.90,1.00,0.00,1.77,0.00,0.00,0.10,0.26,1.44,0.12,0.66,0.05,0.10,0.06,9.55,6.76,7.64,2.61,1284.55,8.91
 0,4.43,44.77,1.15,4.22,3.07,0.14,54.63,0.01,0.01,1.17,218.00,18.03,0.00,11.82,0.02,0.00,0.00,0.00,0.12,0.14,0.06,0.08,0.07,6.24,18.29,15.34,1.96,3.46,3.83
 0,1.44,1.86,1.57,1.93,1.83,0.53,20.45,0.13,0.28,2.27,1.69,35.59,0.21,29.53,0.44,0.01,0.07,0.15,0.22,0.45,0.03,0.07,0.04,9.49,267.43,18.82,6.59,479.77,10.10
 0,3.36,-1.00,0.78,1.09,1.04,1.00,357.05,0.00,0.00,3.44,0.00,0.00,-6.50,0.00,0.00,0.43,0.63,1.33,-0.12,-0.24,-0.08,0.97,-0.07,22.87,1.07,0.14,1.46,6.82,16.25
 0,2.64,9.10,1.93,1.49,1.24,1.05,-12.65,0.06,0.11,2.04,6.04,39.42,1.71,77.35,10.35,0.21,0.81,1.53,0.43,0.81,0.11,0.15,0.12,38.10,20.29,9.08,3.81,16.74,10.67
 0,1.22,0.00,0.98,3.91,0.08,0.06,173.73,0.09,0.11,1.20,-0.19,-1.52,8.46,6.26,-1.63,-0.09,-0.13,-0.18,-0.02,-0.02,-0.01,0.40,-0.01,364.65,1.81,12.51,1.42,4.31,3.15
-0,1.00,1.00,1.00,0.95,0.19,0.18,90.76,0.27,3.05,11.18,0.21,464.47,-2.97,-1 199.18,-0.63,-0.68,-0.24,-3.85,0.08,1.31,0.23,0.29,0.23,65.11,4.29,0.74,0.36,1.46,-6.75
+0,1.00,1.00,1.00,0.95,0.19,0.18,90.76,0.27,3.05,11.18,0.21,464.47,-2.97,-1199.18,-0.63,-0.68,-0.24,-3.85,0.08,1.31,0.23,0.29,0.23,65.11,4.29,0.74,0.36,1.46,-6.75
 0,0.98,-1.00,0.37,0.80,0.41,0.41,-12.08,0.32,9.62,29.68,-0.52,-3.15,-0.29,2.90,0.15,0.05,0.06,0.79,-0.07,-0.92,-0.06,0.18,-0.18,287.46,8.44,6.45,1.06,1.44,-16.98
 0,1.06,0.84,0.00,0.65,0.20,0.06,29.60,0.89,-3.62,-4.07,0.63,8.00,-10.29,20.34,1.47,0.25,1.31,-7.24,-0.13,0.72,-0.03,0.11,0.11,24.10,8.41,12.61,5.21,29.72,-11.97
 0,1.48,0.10,0.00,1.67,0.91,0.08,19.23,1.18,-5.63,-4.77,0.00,0.03,9.46,1.67,0.02,0.07,0.04,-0.14,0.00,-0.01,0.01,1.00,0.01,18.98,0.00,0.00,0.50,0.53,19.24
 0,1.00,1.00,2.26,1.37,0.56,0.02,464.94,0.23,3.25,14.27,0.31,0.00,1.13,0.00,0.18,0.11,0.07,0.83,0.06,0.74,0.09,0.18,0.18,2.05,1.19,19.39,0.63,18.73,1.51
 0,1.51,0.94,0.00,26.29,15.76,0.26,296.86,0.56,-2.77,-4.95,0.18,4.75,1.72,-18.07,-0.75,-0.87,-0.59,0.74,-0.35,0.44,-0.51,-0.21,0.21,1.62,2.61,5.31,0.68,4.63,0.64
 0,1.00,1.00,1.00,1.18,0.58,0.09,61.51,0.28,0.67,2.42,0.14,0.61,0.91,2.23,0.13,0.04,0.04,0.09,0.02,0.04,0.02,0.28,0.04,4.00,2.43,2.03,0.86,1.80,10.88
 0,0.97,1.09,1.05,8.10,5.96,1.64,106.00,0.00,0.00,2.27,1.00,0.33,2.53,2.23,0.00,0.05,0.05,0.13,0.02,0.05,0.02,0.65,0.02,5.96,4.32,9.17,1.03,1.53,3.62
 0,2.39,1.17,1.55,0.73,0.07,0.00,269.86,0.05,0.83,15.56,0.61,0.00,7.62,0.00,4.64,0.58,0.31,4.66,0.03,0.43,0.05,0.28,0.08,13.61,1.00,3.03,0.54,1.34,-1.76
-0,4.64,0.00,0.00,0.48,0.00,0.00,-276.05,0.64,-4.22,-6.59,-0.08,-0.60,-2.00,2.30,0.16,2.02,0.11,-0.84,-0.05,0.42,-1.01,0.94,-1.01,1 689.97,0.32,1.32,0.05,0.06,-0.47
+0,4.64,0.00,0.00,0.48,0.00,0.00,-276.05,0.64,-4.22,-6.59,-0.08,-0.60,-2.00,2.30,0.16,2.02,0.11,-0.84,-0.05,0.42,-1.01,0.94,-1.01,1689.97,0.32,1.32,0.05,0.06,-0.47
 0,1.15,1.56,0.08,1.16,0.10,0.10,59.64,0.12,0.34,2.94,4.60,6.49,1.33,11.07,6.11,0.25,0.70,0.31,0.33,0.14,0.12,0.47,0.19,0.00,2.91,5.54,2.80,7.82,30.62
 0,0.39,0.23,0.86,3.47,1.86,0.00,261.56,0.43,1.57,3.70,0.09,0.91,0.23,1.09,-0.02,-0.05,-0.01,-0.03,-0.04,-0.12,-0.23,0.24,0.24,1.09,0.97,5.01,0.18,0.27,0.69
 0,0.95,1.20,1.36,1.17,0.37,0.00,243.50,0.47,2.62,5.57,0.41,5.48,0.61,3.55,0.19,0.27,0.12,0.58,0.19,0.91,0.43,0.59,0.59,7.20,1.84,60.83,0.44,0.53,13.82
 0,1.35,-1.00,0.78,0.65,0.19,0.06,62.30,0.58,2.65,4.59,-0.01,-0.15,-16.16,5.97,0.20,0.16,0.11,0.45,-0.06,-0.25,-0.08,0.53,-0.01,23.44,7.81,0.01,0.69,0.80,-8.90
 0,1.61,87.56,1.15,1.02,0.78,0.00,112.80,0.30,2.70,8.87,0.48,4.71,-3.96,-0.91,-0.25,-0.02,-0.06,-0.72,0.01,0.14,0.00,0.05,0.05,3.49,27.40,72.08,2.50,33.97,149.86
 0,0.00,0.00,0.53,28.49,27.42,27.42,0.00,0.27,0.38,1.42,-0.45,-47.31,-5.57,273.25,2.51,0.00,0.58,0.66,-0.10,-0.12,0.00,0.00,0.00,0.00,0.00,0.41,0.00,0.00,0.00
 0,0.81,1.00,1.23,0.84,0.45,0.02,154.34,0.63,5.69,9.04,0.12,1.36,-4.94,-6.92,-0.44,-0.37,-0.29,-2.76,0.05,0.46,0.06,0.18,0.07,2.24,2.15,2.04,0.78,2.51,-5.73
@@ -48,15 +48,15 @@
 0,0.50,1.00,0.00,0.75,0.46,0.03,200.19,0.16,-0.96,-6.07,1.31,14.28,-1.38,-14.14,-1.52,-0.11,-0.14,1.01,0.08,-0.61,0.07,0.16,0.08,2.45,7.09,0.82,1.23,13.46,-7.54
 0,1.22,2.10,2.72,1.19,0.21,0.03,142.94,0.09,0.64,7.55,1.02,27.06,-0.08,0.43,-0.08,-0.01,-0.01,-0.08,0.10,0.92,0.08,0.23,0.08,8.11,2.05,4.58,1.25,0.00,6.55
 0,2.08,1.81,0.00,0.41,0.00,0.00,121.72,0.22,-0.24,-1.07,0.46,0.66,6.25,5.12,2.64,1.13,0.65,-0.65,-0.06,0.06,-0.10,0.25,0.19,12.59,5.24,-15.79,0.58,2.25,-0.49
 0,1.48,1.16,1.74,3.02,3.01,3.00,325.47,0.30,0.70,2.29,0.74,6.75,1.00,8.70,0.73,0.55,0.26,0.64,0.19,0.46,0.39,1.00,0.55,24.99,0.00,-1.17,0.47,65.65,0.60
 0,1.14,1.00,0.12,0.92,0.14,0.05,91.65,0.54,199.24,369.36,0.13,0.77,1.51,2.17,0.20,0.04,0.11,8.67,-0.02,-1.57,-0.01,0.17,0.03,28.19,2.67,6.29,2.46,26.08,-30.32
 0,1.21,1.60,0.99,4.45,0.30,0.14,236.99,0.15,0.22,1.48,0.76,2.80,-0.16,4.48,-0.07,-0.01,-0.01,-0.02,0.05,0.07,0.04,0.26,0.06,59.41,1.19,4.82,1.16,5.34,1.93
 0,7.12,1.23,4.02,3.16,0.18,0.10,-52.81,0.64,10.71,16.68,0.15,1.90,-0.29,0.00,-0.02,0.00,-0.01,-0.34,0.04,1.20,0.01,1.00,0.02,17.35,0.00,4.94,4.73,155.53,9.24
-0,1 444.83,1 741.52,1 362.36,1.15,0.60,0.06,93.48,0.26,0.62,2.42,0.74,5.04,1.23,8.13,0.61,0.09,0.16,0.77,0.10,0.51,0.06,0.21,0.08,6.04,5.73,11.92,1.69,4.45,21.26
+0,1444.83,1741.52,1362.36,1.15,0.60,0.06,93.48,0.26,0.62,2.42,0.74,5.04,1.23,8.13,0.61,0.09,0.16,0.77,0.10,0.51,0.06,0.21,0.08,6.04,5.73,11.92,1.69,4.45,21.26
 0,1.56,1.00,1.14,4.22,3.93,3.91,25.88,0.13,0.16,1.17,0.99,8.12,0.72,10.31,0.72,0.21,0.10,0.12,0.14,0.16,0.28,0.57,0.25,232.93,11.50,49.16,0.49,0.84,1.50
 0,-1.00,3.05,4.29,1.01,1.01,0.00,0.00,0.54,31.50,58.33,0.23,2.83,-0.02,1.00,-0.01,0.00,0.00,-0.26,0.01,1.14,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 0,0.58,0.00,1.05,2.00,0.56,0.04,462.26,0.28,0.41,1.46,0.00,1.05,-1.80,1.09,-0.20,-0.11,-0.06,-0.08,0.02,0.03,0.04,0.38,0.06,1.83,1.26,13.76,0.50,1.31,1.62
 0,0.56,2.40,32.24,2.38,0.99,0.00,315.26,0.05,0.09,1.72,0.27,6.48,0.01,1.95,0.00,0.00,0.00,0.00,0.02,0.06,0.03,0.05,0.02,1.56,2.51,5.73,0.68,122.99,1.07
 0,1.00,1.00,1.33,1.79,0.32,0.14,105.37,0.21,0.63,2.97,0.95,19.66,0.79,27.91,0.73,0.17,0.20,0.53,0.26,0.69,0.22,0.55,0.18,17.60,2.08,4.01,1.20,2.30,4.25
 0,1.03,0.23,3.72,1.00,1.00,1.00,0.00,0.40,0.85,2.11,0.08,0.00,4.59,0.00,0.36,0.77,0.26,0.48,0.05,0.10,0.16,1.00,0.17,0.00,0.00,0.00,0.33,0.34,13.90
 0,0.74,0.61,2.85,1.33,0.48,0.47,328.05,0.54,1.17,2.17,0.11,0.78,1.00,1.84,0.04,0.06,0.03,0.06,0.04,0.08,0.07,0.13,0.06,7.24,1.18,11.63,0.50,1.83,1.81
@@ -76,39 +76,39 @@
 0,0.75,0.74,1.53,2.17,1.90,0.01,102.24,0.32,0.60,1.86,0.68,9.15,-0.67,-3.55,-0.45,-0.07,-0.16,-0.32,0.21,0.42,0.10,0.17,0.11,2.84,26.97,9.22,2.21,268.18,3.67
 0,1.82,4.18,1.79,1.25,0.34,0.03,18.22,0.31,0.91,2.91,1.19,15.14,0.01,4.38,0.02,0.00,0.01,0.02,0.29,0.88,0.15,0.45,0.23,10.49,5.37,4.32,1.99,6.78,12.71
 0,1.24,2.98,1.58,3.36,1.82,1.15,27.33,0.19,0.28,1.48,1.55,126.41,1.00,128.41,1.55,0.27,0.30,0.54,0.30,0.54,0.27,0.33,0.27,13.39,6.31,6.32,1.12,1.97,3.57
 0,2.93,2.85,1.51,1.61,1.11,0.45,31.27,0.10,0.18,1.76,2.92,10.18,0.83,11.34,2.27,0.08,0.28,0.48,0.24,0.41,0.07,0.19,0.10,15.18,8.84,10.72,3.41,9.92,12.56
 0,1.56,1.00,1.14,4.22,3.93,3.91,25.88,0.13,0.16,1.17,0.99,8.12,0.72,10.31,0.72,0.21,0.10,0.12,0.14,0.16,0.28,0.57,0.25,232.93,11.50,49.16,0.49,0.84,1.50
 0,3.02,-1.00,0.18,0.70,0.69,0.30,85.14,0.85,33.63,39.39,-0.05,-2.21,10.36,-27.36,-0.66,-1.82,-0.83,-6.86,-0.06,-0.51,-0.13,1.00,-0.13,4.29,0.00,-0.05,0.45,0.54,-8.54
 0,1.37,0.60,1.16,1.02,0.62,0.10,22.35,0.11,2.26,21.40,0.21,1.56,5.23,7.52,0.39,0.03,0.04,0.94,0.01,0.15,0.01,0.12,0.02,2.48,19.03,2.54,1.37,86.20,57.39
-0,1.07,1.33,1.68,1.80,1.51,0.00,329.88,0.28,1.64,5.93,0.25,10.29,17.45,182.77,4.34,1.51,1.40,8.92,0.08,0.51,0.09,0.11,0.09,1.89,2.67,0.48,0.92,5 051.63,1.78
+0,1.07,1.33,1.68,1.80,1.51,0.00,329.88,0.28,1.64,5.93,0.25,10.29,17.45,182.77,4.34,1.51,1.40,8.92,0.08,0.51,0.09,0.11,0.09,1.89,2.67,0.48,0.92,5051.63,1.78
 0,0.97,0.73,1.30,1.00,1.00,1.00,0.00,0.26,0.35,1.35,0.72,8.93,1.05,10.73,0.75,0.38,0.22,0.30,0.18,0.24,0.31,1.00,0.36,0.00,0.00,0.00,0.59,0.66,3.80
-0,514.98,1.01,1 636.40,1.16,0.41,0.04,85.00,0.10,0.51,5.04,0.00,1.26,-0.01,-0.46,0.00,0.00,0.00,0.00,0.03,0.16,0.04,0.11,0.00,2.42,3.61,2.19,0.71,9.87,2.82
+0,514.98,1.01,1636.40,1.16,0.41,0.04,85.00,0.10,0.51,5.04,0.00,1.26,-0.01,-0.46,0.00,0.00,0.00,0.00,0.03,0.16,0.04,0.11,0.00,2.42,3.61,2.19,0.71,9.87,2.82
 0,1.31,1.83,0.00,0.64,0.31,0.19,35.80,0.27,-19.04,-69.96,0.34,12.96,0.84,12.67,0.15,0.06,0.07,-5.78,0.09,-6.86,0.07,1.00,0.07,10.20,0.00,0.15,1.30,3.37,-2.28
 0,1.60,2.67,1.19,1.81,0.35,0.05,152.30,0.13,0.28,2.15,0.98,14.28,15.31,233.29,13.78,1.64,1.77,4.13,0.10,0.23,0.09,0.15,0.11,6.32,1.41,2.23,1.08,2.24,2.49
 0,1.50,14.84,1.10,1.50,0.91,0.19,64.62,0.20,0.56,2.89,0.39,4.49,3.91,19.69,1.20,0.14,0.27,0.71,0.04,0.10,0.02,0.14,0.04,5.99,11.93,13.55,1.97,5.51,8.15
-0,0.86,2.15,1.70,3.42,0.08,0.08,147.91,0.24,0.75,3.08,0.34,1.95,1.86,2.89,0.95,0.63,0.25,0.90,0.13,0.48,0.34,0.45,0.22,2 546.35,1.62,4.71,0.40,0.49,2.92
+0,0.86,2.15,1.70,3.42,0.08,0.08,147.91,0.24,0.75,3.08,0.34,1.95,1.86,2.89,0.95,0.63,0.25,0.90,0.13,0.48,0.34,0.45,0.22,2546.35,1.62,4.71,0.40,0.49,2.92
 0,1.24,1.41,2.13,2.46,0.81,0.10,169.54,0.52,6.71,12.94,0.21,1.62,1.00,0.00,0.21,0.08,0.15,1.89,0.06,0.72,0.03,0.24,0.08,83.36,1.72,7.69,1.92,259.53,2.34
 0,1.14,1.13,1.34,5.04,4.29,2.86,145.05,0.32,0.54,1.70,1.56,42.02,0.09,21.39,0.14,0.06,0.06,0.09,0.48,0.73,0.51,0.81,0.65,5.72,3.22,11.32,0.93,2.07,1.95
 0,1.34,1.48,1.30,2.55,2.55,2.55,0.00,0.35,0.54,1.54,0.54,0.00,0.00,1.04,0.00,0.00,0.00,0.00,0.18,0.29,0.31,1.00,0.31,0.00,0.00,-0.01,0.59,5.84,0.99
 0,1.55,1.62,1.31,1.01,0.56,0.12,-3.26,0.23,1.05,4.63,0.59,4.34,1.00,6.18,0.36,0.06,0.09,0.43,0.07,0.35,0.05,0.31,0.06,7.13,2.99,2.07,1.60,6.86,142.77
 0,0.14,-1.00,0.78,2.10,1.13,1.33,-58.12,0.37,2.24,6.13,-0.03,0.00,1.00,0.00,-0.03,-0.09,-0.01,-0.07,-0.04,-0.27,-0.35,0.15,-0.09,-6.28,0.23,0.06,0.12,13.01,0.27
 0,0.71,0.88,1.12,7.27,4.21,3.25,58.93,0.07,0.08,1.11,1.56,27.87,0.00,0.00,0.00,0.00,0.00,0.00,0.12,0.14,0.10,0.19,0.09,20.94,4.31,8.44,1.20,4.09,2.01
-0,1.47,2.02,3.30,4.44,1.38,0.54,153.92,0.31,0.45,1.45,0.55,0.00,1.00,0.00,0.55,0.23,0.29,0.38,0.29,0.38,0.23,0.31,0.23,15.52,2.79,1 111.21,1.24,2.23,2.94
+0,1.47,2.02,3.30,4.44,1.38,0.54,153.92,0.31,0.45,1.45,0.55,0.00,1.00,0.00,0.55,0.23,0.29,0.38,0.29,0.38,0.23,0.31,0.23,15.52,2.79,1111.21,1.24,2.23,2.94
 0,2.62,1.00,1.09,1.67,1.28,0.35,256.19,0.09,0.14,1.68,2.25,2.76,1.00,3.84,0.33,0.02,0.03,0.05,0.03,0.05,0.02,0.84,0.02,9.08,1.69,0.88,1.74,3.99,6.47
 0,1.31,1.83,0.00,0.64,0.31,0.19,35.80,0.27,-19.04,-69.96,0.34,12.96,0.84,12.67,0.15,0.06,0.07,-5.78,0.09,-6.86,0.07,1.00,0.07,10.20,0.00,0.15,1.30,3.37,-2.28
 0,0.96,-1.00,0.00,0.25,0.14,0.00,99.98,0.00,0.00,-0.35,0.00,0.00,-0.04,0.00,0.00,0.00,0.01,-0.02,-0.14,0.36,-0.09,0.85,-0.09,36.76,4.05,0.49,1.51,1.62,-3.93
 0,1.14,1.68,1.00,0.44,0.18,0.01,-15.35,0.19,0.92,4.94,0.36,1.96,-2.08,-2.99,-0.73,-0.11,-0.15,-0.68,0.04,0.16,0.03,0.11,0.05,8.54,11.89,4.11,1.40,2.17,-3.07
 0,2.86,2.61,2.11,1.02,0.83,0.00,20.72,0.26,11.75,45.50,0.12,1.82,-15.13,0.00,-0.82,-0.08,-0.25,-13.03,0.01,0.72,0.00,0.23,0.01,3.97,11.43,3.54,2.99,217.88,116.47
 0,1.04,1.16,2.26,1.00,1.00,1.00,191.04,0.66,1.90,2.90,0.38,2.21,0.46,3.10,0.18,0.20,0.20,0.47,0.40,0.94,0.40,0.49,0.43,0.00,1.91,0.00,1.00,1.41,3.13
-0,162.51,78.06,0.29,1.00,0.72,0.00,114.36,0.32,1 980.79,6 102.90,0.04,7.99,-0.03,-0.46,0.00,0.00,0.00,-1.08,0.02,33.39,0.02,0.03,0.03,1.44,13.13,2.20,1.03,1 569.33,3 429.77
+0,162.51,78.06,0.29,1.00,0.72,0.00,114.36,0.32,1980.79,6102.90,0.04,7.99,-0.03,-0.46,0.00,0.00,0.00,-1.08,0.02,33.39,0.02,0.03,0.03,1.44,13.13,2.20,1.03,1569.33,3429.77
 0,1.58,0.13,1.99,1.05,0.48,0.23,33.12,0.12,0.59,5.00,0.09,0.00,1.61,11.45,1.55,0.10,0.28,1.22,0.17,0.76,0.06,0.12,0.01,10.76,5.65,5.58,2.75,18.95,42.62
 0,1.01,1.16,1.03,1.51,0.28,0.03,191.63,0.38,0.77,2.00,0.22,1.29,15.09,39.87,2.36,0.69,0.91,1.84,0.01,0.03,0.01,0.21,0.05,10.65,1.81,8.16,1.31,5.94,5.09
 0,1.40,1.20,1.51,1.23,0.90,0.73,13.53,0.21,0.81,3.82,0.64,5.77,6.54,39.61,3.19,0.58,1.04,3.11,0.14,0.41,0.08,0.21,0.09,9.29,7.16,4.76,1.80,10.39,7.31
-0,0.95,3.26,1.08,22.70,0.04,0.02,16.46,0.24,0.32,1.32,0.33,0.00,0.63,3.67,0.15,0.16,0.04,0.05,0.06,0.08,0.26,1.00,0.37,5 664.70,0.00,-22.26,0.22,0.23,3.02
+0,0.95,3.26,1.08,22.70,0.04,0.02,16.46,0.24,0.32,1.32,0.33,0.00,0.63,3.67,0.15,0.16,0.04,0.05,0.06,0.08,0.26,1.00,0.37,5664.70,0.00,-22.26,0.22,0.23,3.02
 0,0.85,0.88,0.00,0.76,0.24,0.07,-137.54,0.10,-1.89,-19.88,0.17,0.00,1.15,2.76,0.35,0.05,0.03,-0.69,0.00,0.05,0.00,0.07,0.02,4.29,0.99,1.64,0.62,3.22,-2.60
 0,0.66,2.14,3.23,1.35,0.23,0.11,32.75,0.61,9.42,15.41,0.24,0.46,1.00,1.46,0.09,0.05,0.05,1.24,0.00,0.05,0.00,0.86,0.05,8.57,1.35,1.30,0.88,1.58,8.59
 0,0.85,2.43,0.95,1.25,0.39,0.04,114.74,0.06,0.13,2.02,1.55,15.50,0.70,15.49,0.98,0.08,0.06,0.12,0.07,0.16,0.10,0.18,0.11,8.27,2.33,4.25,0.74,1.37,7.16
 0,0.94,0.98,1.29,0.20,0.01,0.04,-1.90,0.21,0.32,1.54,1.11,20.25,0.90,19.19,1.00,0.66,0.23,0.36,0.25,0.40,0.73,1.00,0.73,-191.67,0.00,0.00,0.35,0.62,-2.79
 0,1.00,0.00,0.56,1.03,0.85,0.38,411.49,0.52,2.48,4.74,-0.25,-5.97,1.00,-4.92,-0.27,-0.40,-0.18,-0.48,-0.21,-0.57,-0.48,0.89,-0.41,4.58,1.10,0.36,0.45,0.63,34.44
 0,5.72,4.21,1.22,0.87,0.66,0.01,205.16,0.16,0.33,2.00,0.76,13.44,-1.23,-9.07,-0.75,-0.28,-0.16,-0.27,0.12,0.20,0.21,0.59,0.23,2.77,4.59,60.37,0.57,0.78,-7.31
 0,1.24,1.17,1.32,5.58,4.12,2.81,63.66,0.24,0.46,1.93,0.93,16.31,-0.74,2.73,-0.40,-0.12,-0.11,-0.21,0.15,0.28,0.15,0.95,0.16,5.73,0.29,0.78,0.95,2.68,1.70
@@ -120,57 +120,57 @@
 0,1.38,1.84,12.94,3.63,1.27,0.04,44.96,0.00,0.00,1.21,1.00,98.63,0.98,98.58,0.00,0.12,0.42,0.69,0.42,0.69,0.12,0.17,0.12,17.11,12.14,56.78,3.41,7.14,7.93
 0,1.50,2.34,1.89,1.59,1.21,0.39,34.54,0.20,0.48,2.44,1.36,14.01,4.79,70.00,5.66,0.59,1.61,3.58,0.29,0.64,0.11,0.19,0.12,6.72,17.10,8.88,2.74,14.67,6.09
 0,6.92,1.67,1.51,0.06,0.06,0.06,1.07,0.10,0.11,1.11,1.97,0.00,1.00,0.00,1.97,0.75,0.23,0.27,0.23,0.26,0.73,0.79,0.75,0.00,342.26,0.00,0.31,0.31,-2.79
 0,1.05,1.17,6.32,1.98,1.89,0.11,180.92,0.16,0.43,2.64,1.61,5.89,0.20,7.96,0.16,0.01,0.03,0.12,0.12,0.48,0.04,0.90,0.05,5.52,3.18,0.34,3.16,15.28,6.46
 0,1.39,1.44,0.72,1.00,1.00,1.00,16.66,0.42,0.72,1.72,0.84,5.11,1.42,8.04,0.99,0.48,0.37,0.59,0.32,0.50,0.41,0.82,0.41,0.00,21.90,0.78,0.78,0.80,19.98
 0,0.87,1.06,1.17,2.81,0.31,0.29,338.83,0.09,0.15,1.61,0.93,16.77,1.00,46.82,2.49,0.41,0.26,0.41,0.10,0.15,0.15,0.41,0.15,124.88,1.07,85.78,0.63,2.98,1.11
 0,0.96,0.84,1.02,0.71,0.51,0.14,-4.88,0.11,0.16,1.45,0.46,-0.54,-4.89,21.34,0.68,0.38,0.08,0.11,-0.02,-0.02,-0.08,0.09,-0.03,8.36,26.77,5.87,0.21,0.22,-11.23
-0,0.58,0.59,0.46,1.03,0.33,0.16,50.50,0.56,19.30,34.31,0.14,771.34,-3.94,-4.57,-0.57,-0.22,-0.42,-6.97,0.09,1.56,0.05,0.16,0.06,9.14,5.32,6.29,1.92,30 783.19,50.63
+0,0.58,0.59,0.46,1.03,0.33,0.16,50.50,0.56,19.30,34.31,0.14,771.34,-3.94,-4.57,-0.57,-0.22,-0.42,-6.97,0.09,1.56,0.05,0.16,0.06,9.14,5.32,6.29,1.92,30783.19,50.63
 0,1.20,2.20,1.00,1.24,0.31,0.12,-305.24,0.47,8.78,18.80,0.29,7.00,0.02,2.14,0.01,0.00,0.00,-0.44,0.08,-12.75,0.11,0.52,0.19,10.10,0.49,1.07,0.79,6.38,4.15
 0,0.77,0.71,1.03,3.24,1.19,1.19,47.81,0.07,0.08,1.21,0.74,2.63,37.74,167.22,47.00,1.52,3.26,3.96,0.05,0.06,0.02,0.10,0.02,0.00,4.82,13.06,2.14,4.84,5.42
 0,1.51,1.18,1.34,0.52,0.51,0.07,47.79,0.31,1.17,3.76,1.21,4.78,1.84,11.25,0.58,0.09,0.19,0.78,0.07,0.29,0.03,1.00,0.05,7.64,0.00,0.00,2.08,3.77,-5.91
 0,1.09,1.31,1.31,0.84,0.40,0.00,250.72,0.39,2.14,5.52,0.90,0.92,19.49,27.40,2.17,0.50,0.91,5.28,0.05,0.27,0.03,0.91,0.03,10.49,1.69,0.35,1.81,2.98,-23.97
 0,-1.00,0.97,1.04,5.01,4.82,4.24,0.00,0.18,0.22,1.25,0.46,-4.84,-0.27,2.73,0.21,0.00,0.04,0.05,0.04,0.05,0.00,0.00,0.00,0.00,0.00,0.23,0.00,0.00,0.00
 0,1.00,1.00,1.42,5.39,2.09,0.20,91.30,0.08,0.10,1.34,3.41,29.55,0.18,6.80,0.58,0.02,0.05,0.07,0.29,0.38,0.12,0.27,0.12,10.19,5.06,21.94,2.47,96.75,2.61
 0,0.49,-1.00,0.95,1.02,0.36,0.01,181.64,0.17,1.43,8.21,-0.03,-2.86,5.28,6.53,0.69,0.10,0.10,0.95,-0.01,-0.05,-0.01,0.07,0.00,4.50,2.09,4.93,1.07,15.80,57.89
 0,0.89,0.46,0.77,2.58,1.61,0.44,98.19,0.08,0.12,1.54,1.17,4.35,2.26,41.51,1.70,0.08,0.12,0.18,0.01,0.01,0.00,0.14,0.03,3.95,10.55,12.62,1.57,13.13,3.46
 0,1.44,1.36,2.42,0.80,0.41,0.41,129.34,0.06,0.38,6.39,1.81,6.89,6.30,0.00,9.75,0.67,0.69,5.23,0.11,0.83,0.11,0.36,0.12,0.00,2.82,0.95,1.04,2.55,-5.27
 0,1.65,1.70,1.09,1.24,0.86,0.07,4.89,0.10,0.30,2.96,1.41,0.00,-0.81,-4.45,-1.14,-0.05,-0.14,-0.36,0.09,0.23,0.03,0.16,0.06,6.76,16.96,5.17,2.96,12.36,15.27
 0,2.16,6.01,1.04,1.48,1.23,0.02,38.29,0.09,0.14,1.58,2.45,8.91,0.89,15.37,1.63,0.15,0.15,0.23,0.10,0.16,0.10,0.48,0.16,4.48,11.79,4.92,1.01,1.40,8.74
 0,0.95,1.03,1.13,8.94,1.35,0.40,32.33,0.09,0.10,1.10,1.63,12.09,0.08,2.26,0.10,0.01,0.01,0.01,0.11,0.12,0.15,0.31,0.17,11.29,0.89,0.00,0.74,2.60,1.07
-0,1 096.46,1 724.41,2 436.22,1.74,0.42,0.07,86.17,0.12,0.30,2.46,2.03,30.42,2.42,1 630.26,4.99,0.54,1.21,2.99,0.48,1.18,0.21,0.29,0.22,14.47,3.62,9.17,2.25,9.98,3.42
+0,1096.46,1724.41,2436.22,1.74,0.42,0.07,86.17,0.12,0.30,2.46,2.03,30.42,2.42,1630.26,4.99,0.54,1.21,2.99,0.48,1.18,0.21,0.29,0.22,14.47,3.62,9.17,2.25,9.98,3.42
 0,1.14,1.23,0.82,1.00,1.00,1.00,-20.81,0.57,1.34,2.34,0.75,7.92,0.84,7.78,0.63,0.14,0.38,0.76,0.45,0.91,0.16,0.24,0.16,0.00,30.63,11.15,2.82,3.66,14.06
 0,1.20,1.68,2.25,1.21,0.34,0.09,60.50,0.23,0.76,3.30,0.91,6.14,0.00,1.32,0.00,0.00,0.00,0.00,0.20,0.77,0.08,0.22,0.08,11.39,4.50,6.92,2.42,11.41,14.29
 0,1.19,2.17,0.76,1.03,0.09,0.02,56.42,0.27,5.64,20.69,0.41,2.53,0.90,2.22,0.13,0.02,0.04,0.65,0.04,0.60,0.02,0.01,0.04,17.83,2.78,3.83,2.22,183.83,75.79
-0,504.34,1 076.28,1 516.57,2.78,1.10,0.01,61.18,0.12,0.19,1.65,1.52,6.49,-0.61,-2.39,-0.82,-0.32,-0.19,-0.32,0.41,0.68,0.68,0.76,0.52,2.00,0.60,3.00,0.61,2.71,0.61
+0,504.34,1076.28,1516.57,2.78,1.10,0.01,61.18,0.12,0.19,1.65,1.52,6.49,-0.61,-2.39,-0.82,-0.32,-0.19,-0.32,0.41,0.68,0.68,0.76,0.52,2.00,0.60,3.00,0.61,2.71,0.61
 0,1.76,1.53,4.47,1.00,1.00,1.00,39.65,0.34,0.53,1.53,1.11,0.00,0.17,2.89,0.19,0.03,0.12,0.16,0.60,0.81,0.15,0.57,0.18,0.00,9.20,0.00,3.93,4.71,11.91
-0,1 745.54,1 262.51,1 497.47,3.11,2.23,1.43,26.99,0.19,0.24,1.24,1.44,10.38,1.05,12.09,1.52,0.13,0.59,0.73,0.50,0.61,0.11,0.18,0.13,31.85,23.50,0.00,4.45,9.76,6.02
+0,1745.54,1262.51,1497.47,3.11,2.23,1.43,26.99,0.19,0.24,1.24,1.44,10.38,1.05,12.09,1.52,0.13,0.59,0.73,0.50,0.61,0.11,0.18,0.13,31.85,23.50,0.00,4.45,9.76,6.02
 0,2.24,1.31,2.25,1.00,1.00,1.00,159.70,0.00,0.00,1.00,1.00,36.53,1.10,41.05,0.00,0.09,0.11,0.35,0.10,0.31,0.08,0.11,0.08,6.28,2.01,4.57,1.33,36.57,3.19
 0,1.32,1.00,0.00,0.85,0.00,0.02,172.03,0.26,-1.58,-6.20,0.03,0.00,20.80,10.16,0.60,0.25,0.17,-0.94,0.01,-0.03,0.01,0.66,0.01,-43.57,0.40,-2.02,0.65,60.65,-3.55
 0,3.64,47.13,2.84,1.53,0.40,0.33,38.40,0.12,0.24,1.98,3.15,0.00,0.32,14.91,0.95,0.03,0.16,0.34,0.49,1.06,0.10,0.42,0.11,70.95,5.95,13.01,4.88,13.15,18.37
 0,1.35,1.35,1.17,8.27,3.52,2.11,-67.54,0.68,2.32,3.42,0.28,0.00,1.00,4.41,0.09,0.16,0.06,0.22,0.06,0.22,0.16,0.97,0.16,10.50,0.66,3.57,0.39,0.84,1.63
 0,1.51,1.93,0.91,0.95,0.00,0.06,-27.36,0.02,0.04,1.58,4.50,0.00,-113.58,195.74,10.98,0.45,0.30,0.40,-0.01,-0.01,-0.01,0.23,0.00,-188.15,14.56,7.23,0.67,0.82,-66.45
 0,1.14,1.00,1.26,0.42,0.29,0.09,51.49,0.52,8.49,16.18,0.94,13.17,0.16,4.12,0.15,0.12,0.08,1.44,0.03,0.53,0.04,1.00,0.71,7.09,0.00,0.01,0.68,0.90,-1.80
 0,0.58,1.00,1.05,2.00,0.56,0.04,462.26,0.28,0.41,1.46,0.11,1.01,-1.80,1.11,-0.20,-0.11,-0.06,-0.08,0.02,0.03,0.04,0.38,0.06,1.83,1.26,13.76,0.50,1.31,1.62
 0,1.06,2.76,6.29,2.75,0.55,0.24,78.88,0.26,0.50,1.93,0.20,0.00,0.96,0.00,0.19,0.02,0.05,0.17,0.03,0.10,0.01,0.07,0.02,28.90,4.29,19.36,2.18,8.40,4.20
 0,4.81,4.31,1.76,1.00,1.00,1.00,0.00,0.36,0.56,1.56,0.81,0.00,1.00,0.00,0.81,0.59,0.33,0.57,0.31,0.55,0.57,1.00,0.59,0.00,0.00,0.00,0.56,0.62,2.72
 0,1.10,1.11,1.35,1.87,0.56,0.07,194.38,0.18,0.38,2.11,0.58,9.23,-0.95,6.52,-0.46,-0.07,-0.09,-0.20,0.10,0.23,0.08,0.19,0.09,7.99,1.48,3.73,1.19,46.77,2.50
 0,1.82,1.84,1.03,1.00,1.00,1.00,0.00,0.09,0.10,1.10,0.66,3.92,0.81,6.33,0.73,0.81,0.07,0.08,0.06,0.07,0.73,1.00,0.73,0.00,0.00,0.00,0.09,0.09,168.41
 0,0.85,2.43,0.95,1.25,0.39,0.04,114.74,0.06,0.13,2.02,1.55,15.50,0.70,15.49,0.98,0.08,0.06,0.12,0.07,0.16,0.10,0.18,0.11,8.27,2.33,4.25,0.74,1.37,7.16
 0,1.41,1.98,1.49,2.81,1.04,0.27,156.74,0.16,0.25,1.53,2.15,18.32,1.01,23.14,2.13,0.17,0.35,0.64,0.28,0.51,0.14,0.44,0.17,8.72,2.02,5.54,2.02,153.19,3.22
 0,448.34,564.28,849.72,0.82,0.31,0.01,85.24,0.22,0.99,4.46,0.16,3.73,0.98,5.18,0.27,0.07,0.12,0.54,0.11,0.48,0.06,0.22,0.04,7.14,5.33,10.60,1.66,4.54,-5.91
-0,882.42,152.38,66.98,1.00,1.00,1.00,15.44,0.99,125.30,126.30,0.03,0.00,1.00,1.17,0.03,0.00,0.05,6.29,0.05,6.29,0.00,0.15,0.00,2 327.46,23.90,-27 945.25,15.11,176.14,8.27
-0,42 749.53,1.00,0.00,0.26,0.16,0.04,60.41,0.14,-1.78,-13.11,0.37,2.40,-9.03,-99.58,-3.31,-0.75,-0.90,11.78,0.10,-1.30,0.08,0.35,0.08,8.80,19.34,-5 415.99,1.20,1.67,-0.76
+0,882.42,152.38,66.98,1.00,1.00,1.00,15.44,0.99,125.30,126.30,0.03,0.00,1.00,1.17,0.03,0.00,0.05,6.29,0.05,6.29,0.00,0.15,0.00,2327.46,23.90,-27945.25,15.11,176.14,8.27
+0,42749.53,1.00,0.00,0.26,0.16,0.04,60.41,0.14,-1.78,-13.11,0.37,2.40,-9.03,-99.58,-3.31,-0.75,-0.90,11.78,0.10,-1.30,0.08,0.35,0.08,8.80,19.34,-5415.99,1.20,1.67,-0.76
 0,1.39,0.98,1.18,0.00,0.18,0.22,-113.83,0.08,0.10,1.16,2.29,162.28,-1.36,-3.02,-2.56,-0.27,-0.22,-0.27,0.16,0.20,0.20,0.88,0.20,59.95,4.48,1.81,0.80,0.91,-5.11
-0,925.66,892.21,1 330.91,0.37,0.08,0.02,-162.83,0.25,0.40,1.59,0.55,4.03,1.00,5.03,0.55,0.54,0.28,0.44,0.21,0.33,0.41,0.81,0.54,80.71,5.59,1.57,0.51,0.54,-3.41
+0,925.66,892.21,1330.91,0.37,0.08,0.02,-162.83,0.25,0.40,1.59,0.55,4.03,1.00,5.03,0.55,0.54,0.28,0.44,0.21,0.33,0.41,0.81,0.54,80.71,5.59,1.57,0.51,0.54,-3.41
 0,0.11,1.13,1.77,2.55,2.45,1.96,38.46,0.00,0.00,1.60,1.00,0.00,3.89,0.00,0.00,0.22,0.22,0.95,0.06,0.24,0.06,0.50,0.06,1.74,101.83,2.09,1.00,22.56,3.55
 0,2.95,19.52,0.28,1.16,0.33,0.04,102.87,0.22,12.41,56.74,0.88,21.81,-0.15,2.28,-0.13,-0.06,-0.04,-0.73,0.25,4.55,0.38,0.91,0.40,3.55,0.26,0.83,0.66,315.11,3.47
 0,1.58,1.09,1.80,1.21,1.12,0.04,-18.12,0.18,3.44,19.47,0.26,12.65,0.00,0.00,0.00,0.00,0.00,0.00,0.05,0.90,0.02,0.16,0.02,4.09,115.68,3.30,3.08,42.34,13.75
-0,1 838.62,1 227.25,1 037.03,1.00,1.00,1.00,104.52,0.21,0.27,1.27,0.08,0.00,2.46,0.00,0.21,0.25,0.09,0.11,0.03,0.04,0.09,0.13,0.09,0.00,3.49,2 495.39,0.36,0.40,1.89
-0,1.21,1.23,4.23,1.01,1.01,0.00,22.98,0.66,2.09,3.17,0.23,1.81,0.00,1.00,0.00,0.00,0.00,0.00,0.28,0.79,0.18,0.50,0.18,68.10,9.80,18.60,1.56,1.73,5 409.96
+0,1838.62,1227.25,1037.03,1.00,1.00,1.00,104.52,0.21,0.27,1.27,0.08,0.00,2.46,0.00,0.21,0.25,0.09,0.11,0.03,0.04,0.09,0.13,0.09,0.00,3.49,2495.39,0.36,0.40,1.89
+0,1.21,1.23,4.23,1.01,1.01,0.00,22.98,0.66,2.09,3.17,0.23,1.81,0.00,1.00,0.00,0.00,0.00,0.00,0.28,0.79,0.18,0.50,0.18,68.10,9.80,18.60,1.56,1.73,5409.96
 0,0.80,0.55,1.52,5.37,1.95,0.92,97.47,0.20,0.25,1.25,0.48,0.00,0.28,0.00,0.13,0.05,0.03,0.04,0.07,0.10,0.12,0.43,0.18,24.05,4.18,71.19,0.61,0.69,5.46
 0,1.11,1.11,1.00,5.61,5.54,3.10,335.44,0.48,1.12,2.33,0.27,0.00,0.00,5.09,0.00,0.00,0.00,0.00,0.00,0.00,0.00,1.00,0.00,1.09,0.00,0.00,0.15,0.23,0.29
 0,1.57,2.27,1.54,16.82,7.49,0.20,29.15,0.30,0.44,1.48,5.15,94.37,0.00,0.00,0.00,0.00,0.00,0.00,1.68,2.61,0.25,0.48,0.26,36.28,13.53,46.34,6.68,12.07,13.44
 0,0.95,0.93,1.28,1.77,0.63,0.53,102.26,0.26,0.49,1.86,0.57,25.70,0.66,19.18,0.34,0.08,0.10,0.19,0.14,0.25,0.11,0.26,0.14,22.28,2.85,8.67,1.24,4.08,3.66
 0,1.01,1.58,0.89,1.05,0.43,0.02,83.38,0.64,3.68,5.74,0.15,1.46,-17.85,-5.03,-0.49,-0.16,-0.36,-1.69,0.02,0.11,0.01,0.14,0.03,9.14,7.03,43.05,2.29,5.96,60.03
 0,1.01,1.58,0.89,1.05,0.43,0.02,83.38,0.64,3.68,5.74,0.15,1.46,-17.85,-5.03,-0.49,-0.16,-0.36,-1.69,0.02,0.11,0.01,0.14,0.03,9.14,7.03,43.05,2.29,5.96,60.03
 0,0.99,1.15,1.23,247.31,69.88,59.61,-46.62,0.15,0.18,1.18,1.26,12.77,0.27,5.21,0.31,0.11,0.05,0.06,0.17,0.21,0.37,0.61,0.44,28.22,0.58,6.13,0.45,0.81,0.94
@@ -212,26 +212,26 @@
 1,1.19,0.88,1.16,2.01,0.54,0.04,343.30,0.59,5.39,9.20,0.16,1.41,-2.77,-12.24,-0.31,-1.06,-0.20,-1.82,0.02,0.15,0.09,0.64,0.37,1.06,0.55,0.73,0.18,0.43,0.56
 1,0.93,0.08,1.06,2.34,0.73,0.00,236.47,0.32,0.50,1.59,0.24,2.35,0.16,2.09,0.04,0.03,0.01,0.02,0.04,0.06,0.09,0.22,0.20,1.45,0.47,24.42,0.39,5.66,0.79
 1,5.21,4.37,1.96,1.65,0.29,0.05,10.81,0.78,10.82,13.87,0.22,1.43,0.55,1.84,0.10,0.08,0.15,1.49,0.07,0.65,0.04,0.20,0.15,46.54,21.15,25.53,1.88,2.17,27.66
 1,1.95,0.76,1.48,6.02,0.16,0.08,-301.44,0.40,2.13,5.31,0.29,1.82,0.19,1.44,0.06,0.06,0.03,0.15,0.05,0.27,0.10,0.32,0.28,40.71,0.31,1.18,0.45,0.00,0.50
 1,1.00,1.00,1.00,30.94,5.88,0.05,199.66,0.38,0.63,1.65,0.26,2.75,-0.12,1.12,-0.03,-0.03,-0.01,-0.02,0.05,0.08,0.14,0.29,0.27,1.83,0.36,0.00,0.38,3.65,0.36
 1,0.00,0.00,0.00,15.27,0.04,0.00,251.05,2.16,-1.78,-0.82,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,-0.01,0.01,0.00,0.00,0.00,0.00,1.25,8.78,0.00,0.00,0.00
 1,-1.00,-1.00,0.19,25.70,22.95,0.05,0.00,0.59,1.59,2.70,0.00,-1.38,-1.89,3.91,0.30,0.00,0.10,0.15,-0.05,-0.08,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
-1,0.64,-1.00,0.00,0.74,0.01,0.00,112.11,0.19,835.68,4 303.80,-0.16,0.00,-3.69,0.00,0.60,0.09,0.08,0.26,-0.02,-0.07,-0.02,0.10,-0.02,2.14,10.42,3.91,0.89,2.53,-6.42
+1,0.64,-1.00,0.00,0.74,0.01,0.00,112.11,0.19,835.68,4303.80,-0.16,0.00,-3.69,0.00,0.60,0.09,0.08,0.26,-0.02,-0.07,-0.02,0.10,-0.02,2.14,10.42,3.91,0.89,2.53,-6.42
 1,1.02,-1.00,0.86,1.31,0.49,0.01,339.85,0.24,3.20,13.43,-0.05,-0.20,-1.23,1.82,0.06,0.05,0.01,0.18,-0.01,-0.15,-0.04,0.87,-0.04,3.13,1.64,0.86,0.27,0.36,4.65
 1,-1.00,-1.00,0.00,0.78,0.56,0.53,0.00,1.24,-3.55,-2.85,-0.02,0.00,-7.90,5.36,0.46,0.00,0.50,-2.04,-0.11,0.45,0.00,0.00,0.00,0.00,0.00,0.01,0.00,0.00,0.00
 1,2.26,0.00,0.95,0.98,0.87,0.00,22.75,0.14,0.49,3.39,0.00,-0.07,-100.19,0.00,0.34,0.06,0.06,0.16,-0.01,-0.02,-0.01,0.18,0.00,2.19,9.94,2.02,1.01,2.36,-85.00
 1,1.09,0.00,0.00,24.29,3.50,2.15,92.56,2.62,-0.93,-0.36,-0.01,0.00,-0.81,0.00,0.01,0.12,0.01,-0.01,-0.02,0.01,-0.15,0.30,-0.15,7.73,8.05,0.14,0.11,0.14,0.64
 1,1.23,4.33,0.00,119.18,3.27,1.80,30.36,1.06,-4.37,-4.11,0.02,0.12,0.59,1.10,0.00,0.04,0.00,-0.02,-0.05,0.26,-0.46,0.12,0.07,12.02,0.12,0.08,0.11,0.77,0.14
 1,0.98,1.35,0.90,0.79,0.24,0.06,110.62,0.54,5.06,9.31,0.13,0.87,0.00,0.00,0.00,0.00,0.00,0.00,-0.01,-0.12,-0.02,0.21,0.10,2.79,2.36,2.09,0.73,1.92,-4.84
 1,1.02,1.19,0.00,0.62,0.60,0.00,97.54,0.65,-0.64,-0.99,0.04,0.41,0.00,0.00,0.00,0.00,0.00,0.00,-0.07,0.12,-0.48,0.22,0.15,0.16,3.74,0.09,0.13,0.96,-0.35
 1,2.84,0.00,1.07,5.84,1.25,0.51,231.79,0.39,0.74,1.91,0.00,-0.09,11.99,-40.09,-0.08,-0.18,-0.03,-0.06,0.01,0.03,0.08,0.22,-0.01,1.81,3.19,4.33,0.17,0.47,0.28
 1,1.84,1.00,1.00,1.33,0.26,0.17,223.67,0.80,9.28,11.58,0.04,0.53,-1.13,0.88,-0.04,-0.09,-0.03,-2.42,-0.04,-3.05,-0.11,0.58,0.12,15.46,1.27,4.14,0.33,0.47,4.06
 1,0.53,-1.00,0.00,0.34,0.08,0.03,164.38,0.56,-1.19,-2.14,-0.10,-1.57,-0.21,1.80,0.04,0.21,0.02,-0.05,-0.10,0.24,-0.99,1.00,-0.61,2.22,0.00,0.01,0.10,0.15,-0.17
-1,1.21,0.44,0.00,0.08,0.00,0.00,-67.21,0.69,-83.53,-120.32,0.09,0.00,0.79,2.95,0.06,0.04,0.08,-7.73,0.10,-9.76,0.05,0.17,0.05,1 434.40,56.31,4.94,2.09,2.17,-3.82
+1,1.21,0.44,0.00,0.08,0.00,0.00,-67.21,0.69,-83.53,-120.32,0.09,0.00,0.79,2.95,0.06,0.04,0.08,-7.73,0.10,-9.76,0.05,0.17,0.05,1434.40,56.31,4.94,2.09,2.17,-3.82
 1,1.00,0.00,0.00,1.74,0.00,0.00,15.49,1.62,-1.92,-1.19,-0.11,-0.79,-0.30,1.23,0.03,0.67,0.05,-0.07,-0.18,0.24,-2.27,0.80,-2.27,23.56,0.04,0.07,0.08,0.13,0.47
 1,0.97,1.26,0.36,1.60,1.01,0.06,335.33,0.65,4.27,6.56,0.39,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.09,0.47,0.31,0.87,0.50,1.09,0.29,0.45,0.29,1.11,1.89
 1,3.10,0.00,0.00,0.11,0.11,0.08,18.92,1.19,-1.82,-1.53,-0.03,-0.31,-2.25,1.70,0.08,0.44,0.09,-0.14,0.00,0.00,0.00,1.00,-0.19,19.29,0.10,0.00,0.21,0.40,-0.51
 1,0.44,0.65,1.03,1.13,0.07,0.00,133.31,0.22,1.05,4.77,0.15,1.99,0.00,1.00,0.00,0.00,0.00,0.00,0.01,0.04,0.04,0.31,0.15,2.74,0.30,0.62,0.27,0.93,2.91
 1,0.66,0.00,0.73,0.75,0.16,0.07,33.58,0.26,1.55,5.93,-0.55,-6.74,-0.01,1.07,0.01,0.00,0.00,0.01,-0.14,-0.72,-0.26,-0.09,-0.26,10.75,6.72,6.67,0.55,1.16,-3.83
 1,0.63,0.97,1.00,4.21,0.25,0.12,76.80,0.25,0.41,1.64,0.26,2.90,1.00,3.46,0.22,0.65,0.06,0.09,0.03,0.04,0.30,0.85,0.77,15.01,6.95,0.44,0.10,0.11,0.61
 1,0.02,0.00,0.00,1.86,1.11,0.21,0.00,0.68,-13.95,-20.52,-0.06,-0.62,0.00,1.00,0.00,0.00,0.00,0.00,-0.06,1.82,-7.59,-2.63,-7.59,0.03,0.09,0.11,0.01,0.03,0.02
@@ -265,36 +265,36 @@
 1,1.66,2.27,0.00,0.21,0.14,0.10,11.90,1.96,-1.39,-0.71,0.18,0.08,0.27,2.08,0.08,0.27,0.14,-0.11,0.14,-0.11,0.27,1.00,0.02,30.68,0.00,0.00,0.54,0.59,-1.60
 1,1.02,1.16,1.28,1.35,0.53,0.11,76.74,0.66,2.21,3.35,0.20,1.95,1.36,4.00,0.28,0.05,0.20,0.68,0.07,0.25,0.02,0.10,0.03,14.92,6.85,356.27,4.33,48.14,15.98
 1,0.13,0.23,1.03,3.03,0.09,0.00,0.00,0.59,7.36,12.44,0.03,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.01,0.13,1.05,0.02,0.01,0.22,0.04,0.00,0.01,1.92,0.01
 1,1.00,0.00,7.90,1.37,0.89,0.07,31.72,0.00,0.00,1.84,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.13,0.22,0.03,1.00,0.09,11.51,0.03,0.68,4.17,10.37,12.93
 1,1.00,1.00,1.01,3.48,0.00,0.00,-283.58,0.11,0.12,1.14,0.26,1.70,0.47,1.33,0.05,0.05,0.01,0.01,0.01,0.01,0.11,0.42,0.27,0.00,5.30,1.04,0.10,0.11,9.62
 1,0.12,0.91,-1.00,0.07,0.04,0.00,409.24,2.30,-1.13,-0.49,0.18,0.00,0.01,0.00,0.00,0.02,0.00,-0.02,0.37,-2.00,2.70,0.59,2.51,1.81,1.76,0.23,0.14,0.18,-0.06
 1,1.35,0.00,0.41,0.62,0.61,0.21,132.03,0.83,6.29,7.55,0.00,9.34,0.00,0.00,0.00,0.00,0.00,0.00,0.27,0.83,0.49,0.27,0.02,2.71,124.04,65.51,0.56,0.82,-1.65
-1,1.01,0.80,1.29,1.07,0.03,0.03,167.53,0.46,1.89,4.08,0.30,2.17,1.91,5.38,0.53,0.23,0.29,1.13,0.06,0.25,0.05,0.28,0.12,3 132.89,2.18,1 827.27,1.27,2.71,46.48
+1,1.01,0.80,1.29,1.07,0.03,0.03,167.53,0.46,1.89,4.08,0.30,2.17,1.91,5.38,0.53,0.23,0.29,1.13,0.06,0.25,0.05,0.28,0.12,3132.89,2.18,1827.27,1.27,2.71,46.48
 1,0.01,-1.00,-1.00,0.50,0.48,0.00,-35.63,2.01,-1.97,-0.98,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,-0.01,0.08,0.07,0.08,0.02,4.77,3.25,0.01,0.36,-0.01
-1,0.67,5.22,-1.00,0.98,25.31,24.33,44.31,0.83,-514.87,-622.48,2.70,1.40,1.00,2.28,0.20,0.08,0.15,0.28,0.03,0.05,0.02,0.19,0.11,12.23,9.00,14.00,1.80,2.15,-1 224.16
+1,0.67,5.22,-1.00,0.98,25.31,24.33,44.31,0.83,-514.87,-622.48,2.70,1.40,1.00,2.28,0.20,0.08,0.15,0.28,0.03,0.05,0.02,0.19,0.11,12.23,9.00,14.00,1.80,2.15,-1224.16
 1,0.45,0.84,-1.00,5.46,1.95,0.26,314.20,1.00,-939.89,-938.89,0.18,4.59,0.73,2.00,0.04,0.21,0.04,0.09,0.05,0.10,0.24,0.76,0.95,1.16,0.15,-0.26,0.20,0.33,0.51
 1,0.93,0.83,0.42,1.42,0.53,0.01,30.55,0.41,1.17,2.82,0.33,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.04,0.06,0.03,0.32,0.06,4.00,6.55,3.13,1.42,4.65,6.15
 1,1.03,1.20,1.09,1.37,0.15,0.01,342.67,0.64,2.23,3.51,0.14,1.33,2.93,1.60,0.08,0.04,0.06,0.19,0.02,0.08,0.02,0.31,0.07,24.54,1.05,19.08,1.36,62.18,4.91
 1,0.56,0.22,0.46,1.86,1.03,0.17,60.32,0.47,5.80,12.30,0.07,0.54,27.54,20.11,1.95,0.49,0.84,7.11,0.09,0.74,0.05,0.11,0.02,5.91,6.89,6.71,1.73,7.14,5.57
 1,2.73,0.00,1.00,0.93,0.33,0.03,14.23,0.00,0.00,58.25,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,3.60,158.25,0.19,0.40,0.19,59.20,24.85,55.14,19.01,148.67,-196.76
-1,0.99,-1.00,0.00,0.00,0.01,0.01,0.11,1.18,-1.27,-1.08,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,-0.04,0.04,-0.18,1.00,-0.18,3 398.75,0.00,0.00,0.22,0.43,-0.30
-1,1.00,1.00,-1.00,0.13,0.13,0.00,0.00,0.90,-0.57,-0.63,0.03,0.00,2 164.72,0.00,0.33,6.72,0.60,3.21,0.09,0.48,1.00,1.00,0.49,0.42,0.00,0.00,0.09,0.11,-0.03
+1,0.99,-1.00,0.00,0.00,0.01,0.01,0.11,1.18,-1.27,-1.08,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,-0.04,0.04,-0.18,1.00,-0.18,3398.75,0.00,0.00,0.22,0.43,-0.30
+1,1.00,1.00,-1.00,0.13,0.13,0.00,0.00,0.90,-0.57,-0.63,0.03,0.00,2164.72,0.00,0.33,6.72,0.60,3.21,0.09,0.48,1.00,1.00,0.49,0.42,0.00,0.00,0.09,0.11,-0.03
 1,1.00,0.00,1.16,0.96,0.54,0.29,321.73,0.35,1.31,3.71,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.03,0.08,0.07,0.33,0.18,3.76,1.63,0.99,0.40,0.71,-14.05
 1,1.61,3.45,1.49,0.58,0.39,0.03,17.71,0.59,2.27,3.83,0.15,0.91,0.22,1.58,0.03,0.14,0.02,0.09,0.09,0.40,0.64,0.76,0.61,4.54,97.80,5.50,0.14,0.15,-3.67
 1,1.02,1.29,1.04,0.37,0.32,0.01,144.34,0.20,0.37,1.85,0.20,2.32,0.67,3.46,0.11,0.22,0.02,0.04,0.02,0.04,0.20,1.00,0.33,2.53,0.00,0.00,0.10,0.10,-1.34
 1,0.79,0.47,0.91,2.42,1.53,0.11,180.87,0.38,0.68,1.81,0.04,0.25,0.23,11.33,0.01,0.01,0.00,0.00,0.05,0.09,0.18,0.79,0.04,3.57,1.05,1.36,0.30,0.35,3.57
 1,1.22,2.43,-1.00,7.28,0.22,0.18,90.70,1.39,-2.67,-1.92,0.02,0.35,0.00,0.00,0.00,0.00,0.00,0.00,0.19,2.00,0.20,0.32,0.03,104.92,2.88,9.27,0.97,16.80,1.14
 1,6.95,3.80,-1.00,0.14,0.02,0.00,-42.12,1.76,-2.27,-1.29,0.01,0.03,14.36,1.50,0.02,1.74,0.05,-0.89,0.10,-2.00,3.90,0.35,0.12,3.63,26.87,2.34,0.03,0.03,-0.05
 1,0.99,0.77,0.89,0.57,0.21,0.00,33.73,0.49,1.61,3.32,0.09,0.06,3.35,2.64,0.12,0.15,0.06,0.18,0.20,0.54,0.46,0.24,0.04,7.50,6.48,5.12,0.43,0.56,-2.09
 1,0.99,0.77,0.89,0.57,0.21,0.00,33.73,0.49,1.61,3.32,0.09,0.06,3.35,2.64,0.12,0.15,0.06,0.18,0.20,0.54,0.46,0.24,0.04,7.50,6.48,5.12,0.43,0.56,-2.09
 1,0.98,0.27,-1.00,9.63,1.42,0.83,48.94,1.39,-3.55,-2.55,0.00,0.02,11.89,0.00,0.01,1.57,0.01,-0.23,0.12,-2.00,13.60,0.97,0.13,7.46,0.00,0.64,0.01,0.01,10.85
 1,0.64,0.37,-1.00,1.32,1.22,0.00,121.33,0.28,-9.57,-33.75,0.03,0.16,0.00,0.00,0.00,0.00,0.00,0.00,0.04,-3.53,0.22,0.08,0.05,0.20,3.01,0.26,0.17,2.46,0.77
 1,0.78,0.67,1.32,0.22,0.03,0.00,151.74,0.00,0.00,8.30,1.00,0.00,0.07,0.00,0.00,0.01,0.00,0.03,0.03,0.27,0.05,0.13,0.07,4.74,4.89,0.70,0.53,0.66,-0.84
-1,2.62,1.92,0.91,10.75,8.18,2.50,61.62,1.02,3.94,3.85,0.09,0.37,0.77,119.95,0.07,0.14,0.07,0.27,0.11,0.43,0.22,0.20,0.18,5.65,2 468.61,117.36,0.49,0.55,7.34
+1,2.62,1.92,0.91,10.75,8.18,2.50,61.62,1.02,3.94,3.85,0.09,0.37,0.77,119.95,0.07,0.14,0.07,0.27,0.11,0.43,0.22,0.20,0.18,5.65,2468.61,117.36,0.49,0.55,7.34
 1,3.33,2.62,-1.00,0.33,0.08,0.08,1.33,0.83,-10.05,-12.13,0.19,0.60,4.59,0.00,0.28,0.70,0.21,-14.78,0.01,-0.74,0.04,1.00,0.15,275.23,0.00,0.07,0.30,0.33,-1.91
 1,1.42,5.35,-1.00,1.70,0.31,0.13,171.61,0.72,-12.20,-17.00,0.26,3.19,5.14,19.98,1.05,0.59,0.82,14.39,0.11,1.99,0.08,0.47,0.11,27.70,1.43,3.79,1.40,8.66,3.67
 1,0.74,0.45,0.53,0.50,0.40,0.13,-64.60,0.46,1.94,4.17,0.32,9.43,1.41,83.58,0.23,0.16,0.11,0.31,0.13,0.36,0.19,0.57,0.11,4.86,5.24,1.74,0.69,1.36,-2.21
 1,0.81,0.89,1.26,1.96,0.44,0.09,-40.25,0.65,7.64,11.68,0.29,15.82,3.58,264.15,1.02,1.40,1.07,8.69,0.03,0.23,0.04,0.14,0.39,3.53,424.90,2.53,0.77,13.01,1.01
 1,0.00,3.46,1.16,5.32,0.13,0.02,0.00,0.64,2.47,3.88,0.00,0.00,299.72,0.00,1.00,0.00,1.00,2.65,0.00,0.01,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 1,0.89,1.01,0.78,1.02,0.52,0.06,175.69,0.57,4.54,7.91,0.26,1.76,1.36,5.24,0.35,0.21,0.21,1.38,0.05,0.30,0.05,0.20,0.15,2.36,4.89,6.82,0.99,7.22,59.17
 1,1.16,0.77,1.03,1.25,0.28,0.01,94.60,0.43,2.13,4.98,0.28,2.19,0.29,0.00,0.08,0.01,0.03,0.17,0.01,0.03,0.00,0.09,0.05,13.89,2.96,6.65,2.52,127.09,12.76
@@ -307,56 +307,56 @@
 1,1.34,0.95,1.00,1.36,0.12,0.07,190.28,0.55,1.58,2.86,0.28,2.08,0.82,6.31,0.13,0.07,0.08,0.21,0.00,0.00,0.00,0.37,0.08,69.72,1.74,14.94,1.16,3.88,5.51
 1,1.57,1.25,0.96,1.37,0.77,0.06,304.03,0.63,2.34,3.69,0.10,0.74,0.54,13.03,0.05,0.04,0.04,0.13,0.01,0.04,0.01,0.27,0.07,1.84,2.69,12.19,1.01,308.78,3.67
 1,1.35,1.75,-1.00,0.57,0.40,0.12,-166.17,1.14,-3.66,-3.22,0.11,2.01,0.76,5.35,0.08,0.31,0.12,-1.26,0.22,-2.32,0.57,0.33,0.40,4.93,20.25,1.41,0.39,0.53,-3.41
 1,1.16,3.11,-1.00,2.77,1.54,0.15,311.83,0.89,-7.65,-8.58,0.49,3.92,0.08,0.00,0.04,0.03,0.04,0.31,0.28,2.00,0.20,0.64,0.39,2.83,1.46,5.41,1.42,19.61,1.84
 1,0.18,0.12,-1.00,0.02,0.01,0.00,42.62,0.62,-0.87,-1.39,0.10,0.52,7.76,8.19,0.77,3.05,0.45,-6.48,0.14,-2.00,0.94,0.39,0.39,15.51,19.12,0.19,0.15,0.15,-0.15
 1,1.09,1.25,-1.00,14.54,0.65,0.04,-12.53,1.28,-4.36,-3.40,0.03,0.09,7.82,0.00,0.04,0.58,0.05,-1.01,0.10,-2.00,1.15,0.03,0.07,12.82,132.14,8.34,0.09,0.10,0.58
 1,1.07,1.12,1.07,6.73,5.15,4.77,-52.40,0.80,5.08,6.38,0.18,1.86,0.72,2.60,0.09,0.28,0.07,0.50,0.01,0.06,0.04,0.45,0.39,11.34,40.06,3.90,0.27,0.38,1.02
-1,1.06,0.91,1.12,0.82,0.82,0.65,28.78,0.21,0.28,1.32,0.05,0.31,4.51,2.32,0.22,874.59,0.05,0.06,0.08,0.12,1 562.86,0.54,194.09,0.00,12.68,0.00,0.00,0.00,0.00
+1,1.06,0.91,1.12,0.82,0.82,0.65,28.78,0.21,0.28,1.32,0.05,0.31,4.51,2.32,0.22,874.59,0.05,0.06,0.08,0.12,1562.86,0.54,194.09,0.00,12.68,0.00,0.00,0.00,0.00
 1,1.47,1.16,-1.00,0.28,0.12,0.10,9.99,1.49,-1.61,-1.08,0.08,0.97,0.53,1.65,0.04,0.31,0.07,-0.48,0.31,-2.10,1.34,1.00,0.57,36.54,0.00,-0.01,0.23,0.25,-1.24
 1,1.00,1.00,-1.00,2.78,0.00,0.00,-284.01,0.79,-214.15,-269.65,0.00,0.00,897.87,0.00,1.00,823.11,1.38,-433.76,0.01,-2.07,3.92,1.00,0.92,32.46,0.00,1.24,0.00,0.00,0.00
 1,1.48,1.86,-1.00,0.11,0.04,0.00,67.69,1.02,-5.49,-5.36,0.14,0.35,1.66,2.43,0.06,0.29,0.06,-1.81,0.06,-2.00,0.32,1.00,0.17,5.39,0.00,0.00,0.20,0.22,-0.28
 1,1.11,1.05,1.08,0.80,0.27,0.22,-37.63,0.40,1.00,2.50,0.17,1.08,1.72,3.36,0.14,0.20,0.06,0.15,0.00,0.01,0.01,0.21,0.12,48.68,24.38,6.07,0.30,0.33,-10.08
 1,1.25,3.59,1.07,0.99,0.17,0.10,-5.30,0.66,378.44,569.93,0.09,1.37,5.94,9.15,0.54,0.21,0.47,213.50,0.00,0.21,0.00,0.35,0.03,21.43,15.05,7.84,2.30,45.53,-251.05
 1,1.33,1.32,-1.00,0.34,0.17,0.04,117.29,0.87,-2.80,-3.21,0.17,2.03,0.88,13.50,0.15,0.39,0.13,2.57,0.15,2.88,0.43,0.71,0.44,3.60,23.01,0.31,0.35,0.43,-0.73
 1,0.00,-1.00,-1.00,0.21,0.02,0.01,0.00,1.01,-1.45,-1.44,0.00,0.02,0.00,0.00,0.00,0.00,0.00,0.00,0.02,-2.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 1,1.05,2.84,-1.00,0.72,0.53,0.02,203.24,0.31,-0.81,-2.59,0.30,2.06,2.34,8.30,0.70,0.22,0.28,6.61,0.08,2.00,0.07,0.41,0.09,2.88,4.78,0.84,1.28,4.48,-3.33
 1,1.17,1.12,-1.00,0.49,0.32,0.22,14.10,0.63,-3.80,-6.07,0.27,2.07,0.88,3.97,0.21,0.45,0.14,1.08,0.08,0.66,0.27,0.64,0.51,45.18,13.03,16.60,0.30,0.32,-6.69
 1,1.14,0.99,1.50,0.98,0.17,0.04,-0.92,0.52,2.82,5.41,0.47,3.15,0.82,6.75,0.21,0.05,0.11,0.72,0.12,0.77,0.06,0.13,0.06,36.36,24.14,14.00,2.12,3.13,-392.83
-1,0.62,0.41,0.06,1.00,0.72,0.00,204.94,0.92,284.35,309.65,0.13,1.40,4.39,5.23,0.20,0.12,0.20,6.53,0.05,1.77,0.03,0.07,0.03,1.99,9.67,22.04,1.65,3 776.94,538.26
+1,0.62,0.41,0.06,1.00,0.72,0.00,204.94,0.92,284.35,309.65,0.13,1.40,4.39,5.23,0.20,0.12,0.20,6.53,0.05,1.77,0.03,0.07,0.03,1.99,9.67,22.04,1.65,3776.94,538.26
 1,0.81,0.25,0.78,0.92,0.11,0.03,51.31,0.20,2.57,13.02,0.03,0.10,7.74,0.00,0.09,0.01,0.02,0.21,0.02,0.25,0.02,0.09,0.00,17.48,8.21,26.01,1.51,9.42,-19.65
-1,0.08,0.41,-1.00,0.86,0.83,0.00,-40.72,1.09,-6.93,-6.37,0.09,0.78,8.31,0.00,0.24,0.72,0.25,-4.01,0.07,-1.10,0.20,0.03,0.09,0.37,37.75,7.24,0.35,1 342.95,-2.30
+1,0.08,0.41,-1.00,0.86,0.83,0.00,-40.72,1.09,-6.93,-6.37,0.09,0.78,8.31,0.00,0.24,0.72,0.25,-4.01,0.07,-1.10,0.20,0.03,0.09,0.37,37.75,7.24,0.35,1342.95,-2.30
 1,5.91,3.69,-1.00,0.95,0.50,0.02,94.01,0.45,-35.75,-78.87,0.17,0.95,1.10,2.14,0.19,0.05,0.12,-24.08,0.01,-1.98,0.00,0.13,0.05,5.86,3.96,6.03,2.27,48.62,-33.36
 1,0.96,0.00,-1.00,2.84,2.71,0.01,326.86,0.74,-60.73,-82.27,0.00,1.38,2.32,0.00,0.30,1.64,0.20,9.97,0.06,3.10,0.51,0.79,0.71,0.17,1.12,-0.80,0.12,0.55,0.26
-1,1.19,1.03,1.00,1.00,1.00,1.00,87.80,0.87,5.96,6.85,0.06,0.00,93.07,0.00,0.21,0.73,0.29,1.27,0.00,0.00,0.00,0.21,0.01,46.77,5 963.04,-4.57,0.39,0.40,1.93
+1,1.19,1.03,1.00,1.00,1.00,1.00,87.80,0.87,5.96,6.85,0.06,0.00,93.07,0.00,0.21,0.73,0.29,1.27,0.00,0.00,0.00,0.21,0.01,46.77,5963.04,-4.57,0.39,0.40,1.93
 1,1.08,1.08,-1.00,1.52,1.51,0.00,150.18,1.87,-2.11,-1.13,0.15,1.07,0.66,1.71,0.09,0.53,0.18,1.48,0.14,1.15,0.41,1.00,0.80,2.43,0.00,0.00,0.33,0.39,6.50
 1,0.22,0.20,-1.00,0.26,0.24,0.00,167.14,2.19,-1.69,-0.77,0.01,0.65,1.13,3.56,0.01,0.47,0.02,-0.36,0.13,-2.12,2.80,0.77,0.42,0.21,2.18,0.00,0.05,0.07,-0.07
 1,1.04,0.65,0.80,0.19,0.03,0.00,-42.15,0.34,1.04,3.10,0.07,0.47,0.04,4.31,0.00,0.00,0.00,0.00,0.08,0.22,0.13,0.21,0.04,62.70,9.07,4.14,0.63,0.67,-2.04
-1,1 024.43,5.03,2.02,715.97,142.04,142.04,2.60,0.59,1.55,2.61,0.02,0.00,81.38,0.00,1.29,1 388.79,1.29,2.68,0.01,0.02,9.25,0.00,17.06,140.61,0.00,0.09,0.00,0.00,0.00
-1,192.83,7.73,-1.00,0.79,0.30,0.30,-22.61,1.06,-2.72,-2.58,0.18,0.65,1.31,2.11,0.15,0.11,0.16,-3.17,0.10,-2.00,0.07,0.13,0.08,2 340.21,10.48,6.34,1.54,2.28,-15.66
+1,1024.43,5.03,2.02,715.97,142.04,142.04,2.60,0.59,1.55,2.61,0.02,0.00,81.38,0.00,1.29,1388.79,1.29,2.68,0.01,0.02,9.25,0.00,17.06,140.61,0.00,0.09,0.00,0.00,0.00
+1,192.83,7.73,-1.00,0.79,0.30,0.30,-22.61,1.06,-2.72,-2.58,0.18,0.65,1.31,2.11,0.15,0.11,0.16,-3.17,0.10,-2.00,0.07,0.13,0.08,2340.21,10.48,6.34,1.54,2.28,-15.66
 1,1.34,1.06,1.04,1.14,0.58,0.02,201.71,0.47,2.51,5.36,0.11,0.95,1.86,3.46,0.19,0.09,0.11,0.49,0.01,0.04,0.01,0.16,0.05,2.55,2.55,4.32,1.24,13.82,9.02
 1,2.44,0.40,1.03,1.85,0.07,0.01,92.76,0.26,0.54,2.04,0.14,1.30,0.84,2.43,0.12,0.02,0.04,0.07,0.02,0.03,0.01,0.03,0.02,65.68,4.15,550.93,2.20,39.90,4.52
 1,0.06,1.02,1.83,4.51,2.49,0.11,215.28,0.38,0.84,2.21,0.10,0.82,5.64,0.00,0.56,12.18,0.25,0.61,0.01,0.03,0.67,1.00,2.16,0.07,0.00,-1.70,0.02,0.04,0.05
-1,1.26,0.53,1.48,1.29,1.06,0.27,44.24,0.66,2.88,4.39,0.08,0.94,0.80,0.00,0.06,0.01,0.05,0.21,0.09,0.39,0.03,0.22,0.02,8.17,116.82,102.16,3.19,8 389.37,12.05
+1,1.26,0.53,1.48,1.29,1.06,0.27,44.24,0.66,2.88,4.39,0.08,0.94,0.80,0.00,0.06,0.01,0.05,0.21,0.09,0.39,0.03,0.22,0.02,8.17,116.82,102.16,3.19,8389.37,12.05
 1,1.00,24.49,2.17,0.54,0.23,0.22,-146.90,0.79,9.82,12.36,0.09,46.76,8.45,50.58,0.75,3.08,1.14,10.04,0.14,1.21,0.37,0.61,0.36,77.37,6.95,1.79,0.37,0.61,-0.62
 1,0.65,0.24,0.68,1.05,0.83,0.25,-125.11,0.01,0.09,6.66,3.92,0.75,11.54,14.41,27.44,0.33,0.30,1.92,0.03,0.18,0.03,0.11,0.03,2.25,6.25,1.06,0.93,9.04,24.43
 1,0.71,0.86,-1.00,1.00,0.37,0.06,212.73,0.65,-4.05,-6.20,0.10,3.79,4.30,14.81,0.45,0.80,0.37,-9.18,0.08,-2.00,0.17,0.14,0.19,2.17,1.92,2.50,0.46,1.54,-202.69
 1,0.00,6.86,-1.00,0.00,0.00,0.00,0.00,0.62,-6.15,-9.84,0.00,0.01,52.76,56.85,0.08,0.00,0.05,-1.59,0.06,-2.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 1,2.73,16.67,3.94,0.36,0.08,0.07,-22.27,0.80,17.25,21.52,0.22,2.23,0.31,1.68,0.04,0.02,0.06,1.18,0.06,1.17,0.02,0.43,0.07,876.95,24.40,9.70,2.78,3.19,-7.74
 1,95.49,0.65,2.18,1.29,0.43,0.07,-10.86,0.16,0.85,5.48,0.06,0.96,7.62,0.00,0.33,0.04,0.09,0.39,0.03,0.12,0.01,0.05,0.01,10.86,9.82,4.47,2.32,10.76,6.60
 1,0.18,0.74,0.65,26.08,14.16,0.00,0.00,0.84,5.27,6.27,0.09,9.64,0.21,4.37,0.02,0.13,0.02,0.09,0.08,0.42,0.64,0.19,0.58,0.84,0.71,0.00,0.13,0.20,0.39
 1,1.25,1.25,13.24,0.99,0.77,0.20,85.64,0.74,21.12,28.72,0.04,1.24,0.00,0.00,0.00,0.00,0.00,0.00,0.01,0.30,0.01,0.27,0.05,1.70,1.96,1.16,0.71,20.85,-37.15
-1,2.13,2.39,4.57,1.26,0.00,0.00,-3.00,0.96,683.92,714.56,0.00,0.00,1.22,0.00,0.00,0.74,0.00,2.56,0.00,2.06,0.60,1.00,0.61,5 283.13,0.00,118.91,0.00,0.01,0.02
+1,2.13,2.39,4.57,1.26,0.00,0.00,-3.00,0.96,683.92,714.56,0.00,0.00,1.22,0.00,0.00,0.74,0.00,2.56,0.00,2.06,0.60,1.00,0.61,5283.13,0.00,118.91,0.00,0.01,0.02
 1,-1.00,7.68,-1.00,2.59,0.96,0.02,0.00,1.09,-1.14,-1.04,0.06,1.78,0.13,1.24,0.01,0.00,0.01,-0.39,0.04,-2.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 1,1.00,1.18,-1.00,0.17,0.17,0.00,182.24,0.55,-14.81,-26.97,0.00,0.03,51.91,3.02,0.17,6.79,0.09,-14.99,0.06,-9.75,4.41,0.09,0.13,0.11,2.00,0.00,0.01,0.02,-0.03
 1,0.65,0.99,0.97,1.14,0.62,0.02,202.53,0.51,6.04,11.75,0.16,1.03,2.91,4.38,0.46,0.22,0.24,2.70,0.00,0.01,0.00,0.17,0.08,2.65,2.55,4.65,1.09,40.10,9.30
 1,-1.00,0.67,-1.00,3.58,0.18,0.00,0.00,0.34,-0.58,-1.70,0.03,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.43,-2.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00,0.00
 1,-1.00,3.79,-1.00,36.55,8.63,7.52,0.00,0.88,-1.66,-1.89,0.01,0.36,0.80,0.00,0.01,0.00,0.01,-0.72,0.03,-2.00,0.00,0.00,0.00,0.00,0.00,0.01,0.00,0.00,0.00
 1,1.20,1.09,-1.00,0.63,0.26,0.01,152.52,1.05,-1.84,-1.75,0.10,1.27,3.07,5.29,0.31,0.17,0.37,-1.64,0.21,-0.90,0.10,0.29,0.06,5.74,3.42,20.75,2.17,39.25,-3.43
-1,1.43,4.04,7.82,1.11,0.48,0.02,18.16,0.87,8.88,10.16,0.21,2.40,4.69,15.00,0.98,0.22,1.31,15.41,0.10,1.21,0.02,0.06,0.05,12.28,205 044.29,31.53,5.89,44 308.74,38.99
+1,1.43,4.04,7.82,1.11,0.48,0.02,18.16,0.87,8.88,10.16,0.21,2.40,4.69,15.00,0.98,0.22,1.31,15.41,0.10,1.21,0.02,0.06,0.05,12.28,205044.29,31.53,5.89,44308.74,38.99
 1,0.85,1.49,1.02,6.55,5.41,1.30,106.35,0.62,1.71,2.76,0.06,1.21,0.50,1.81,0.02,0.10,0.02,0.04,0.01,0.02,0.05,0.38,0.19,3.66,3.24,3.44,0.22,0.27,1.45
 1,0.72,0.44,1.12,1.43,0.38,0.08,108.11,0.48,0.95,1.97,0.11,1.21,0.00,1.05,0.00,0.00,0.00,0.00,0.01,0.08,0.02,0.09,0.02,12.41,4.58,376.32,0.45,7.87,10.86
 1,1.00,1.00,1.00,1.35,1.06,0.00,26.97,0.41,1.03,2.51,0.09,2.07,3.79,7.77,0.28,0.32,0.12,0.29,0.03,0.08,0.08,0.12,0.10,2.07,6.23,1.76,0.36,0.47,6.35
 1,0.49,0.16,0.49,0.81,0.73,0.00,112.00,0.24,12.90,54.09,0.03,0.34,3.06,0.00,0.10,0.07,0.02,0.86,0.03,1.04,0.08,0.14,0.02,0.66,3.26,0.48,0.35,0.96,-2.39
 1,0.37,0.55,1.02,0.91,0.63,0.00,321.03,0.00,0.00,1.85,1.00,2.06,0.07,0.00,0.00,0.01,0.00,0.00,0.02,0.03,0.13,0.14,0.13,0.51,1.14,0.36,0.13,0.20,-3.31
 1,0.00,1.00,1.53,3.56,0.01,0.01,0.00,0.45,1.02,2.27,0.11,0.00,2.03,0.00,0.23,0.00,0.14,0.29,0.07,0.14,0.00,0.00,0.00,0.00,0.00,-0.51,0.00,0.00,0.00
 1,0.80,0.75,1.28,1.06,0.26,0.04,8.17,0.19,1.30,6.68,0.57,0.77,0.33,1.67,0.18,0.01,0.04,0.27,0.04,0.27,0.01,0.10,0.01,16.67,6.94,5.51,4.55,57.15,83.86
@@ -365,23 +365,23 @@
 1,0.21,0.39,1.04,1.37,0.56,0.02,-58.70,0.28,0.79,2.85,0.30,0.00,0.48,1.67,0.48,0.38,0.11,0.39,0.02,0.08,0.08,2.68,0.15,0.75,2.07,1.56,0.30,2.87,1.47
 1,0.72,7.09,0.18,0.12,0.02,0.00,126.10,0.34,3.37,10.04,0.67,5.43,0.01,1.33,0.01,0.00,0.00,0.01,0.16,0.56,0.41,0.13,0.50,9.95,4.08,0.77,0.40,0.48,-0.84
 1,1.10,0.71,-1.00,0.32,0.00,0.00,0.00,0.94,-7.84,-8.34,0.03,208.32,0.68,0.00,0.02,53.13,0.02,-0.49,0.03,-0.72,78.76,1.00,78.38,0.37,0.00,0.00,0.00,0.00,0.00
 1,0.67,0.69,1.05,0.15,0.10,0.00,141.95,0.18,0.42,2.35,0.43,1.46,2.97,6.38,0.60,0.36,0.11,0.26,0.02,0.05,0.07,0.29,0.12,6.61,4.21,0.49,0.30,0.34,-0.61
 1,1.17,0.85,1.07,1.55,0.85,0.01,134.97,0.47,1.17,2.47,0.24,1.71,0.66,3.33,0.11,0.04,0.05,0.13,0.03,0.07,0.02,0.10,0.05,3.24,8.54,17.93,1.49,8.05,4.72
 1,0.78,0.60,0.90,0.18,0.09,0.00,212.79,0.55,1.70,3.12,0.09,0.26,0.05,1.03,0.00,0.01,0.00,0.01,0.04,0.11,0.17,0.92,0.06,23.27,1.85,0.19,0.20,0.21,-1.91
 1,1.05,1.05,-1.00,0.06,0.05,0.02,8.89,1.14,-2.12,-1.85,0.10,0.27,1.27,0.00,0.10,0.55,0.11,-0.93,0.27,-2.29,1.36,1.00,0.43,41.06,0.17,0.06,0.20,0.20,-1.29
-1,1.00,0.64,0.92,0.16,0.02,0.00,0.00,0.09,0.27,2.90,0.10,0.62,8.97,8.17,0.88,18 009.24,0.08,0.23,0.02,0.07,5 263.27,1.00,2 006.99,0.00,0.00,0.00,0.00,0.00,0.00
+1,1.00,0.64,0.92,0.16,0.02,0.00,0.00,0.09,0.27,2.90,0.10,0.62,8.97,8.17,0.88,18009.24,0.08,0.23,0.02,0.07,5263.27,1.00,2006.99,0.00,0.00,0.00,0.00,0.00,0.00
 1,0.88,0.99,-1.00,0.63,0.62,0.00,155.66,0.32,-2.98,-9.31,0.19,0.00,0.94,0.00,0.18,0.25,0.06,-1.31,0.05,-1.23,0.24,0.02,0.27,0.56,2.34,0.05,0.23,0.45,-0.77
 1,0.90,1.47,-1.00,0.96,0.36,0.00,102.63,0.81,-8.60,-10.65,0.08,0.84,1.36,1.22,0.02,0.01,0.02,-1.31,0.03,-2.00,0.02,0.20,0.06,4.18,1.52,1.62,1.28,132.25,-26.70
 1,0.91,0.53,1.24,1.18,0.67,0.00,202.21,0.38,6.98,18.20,0.09,0.00,0.36,0.00,0.03,0.04,0.02,0.26,0.01,0.22,0.04,0.11,0.12,0.87,1.81,0.95,0.37,1.31,2.49
 1,1.00,1.00,-1.00,0.61,0.16,0.00,0.00,0.42,-2.75,-6.54,0.08,0.94,5.39,0.00,0.42,212.26,0.23,-7.84,0.06,-2.00,54.13,0.63,39.41,0.01,0.01,0.52,0.00,0.00,0.00
 1,0.73,1.69,0.63,2.46,2.15,0.06,0.00,0.31,0.45,1.45,0.76,0.00,0.02,0.00,0.02,0.04,0.01,0.01,0.23,0.28,1.72,0.88,1.64,0.24,0.08,-0.89,0.14,0.56,0.32
 1,1.00,1.16,1.00,0.80,0.65,0.01,16.29,0.71,4.86,6.82,0.16,2.10,11.68,13.61,0.78,0.29,0.56,3.81,0.05,0.33,0.02,0.11,0.05,4.36,17.54,4.14,1.93,4.27,-13.80
 1,2.06,4.44,-1.00,2.94,1.73,0.16,123.15,1.12,-5.33,-4.77,0.07,0.00,1.19,0.00,0.08,0.14,0.10,3.40,0.06,2.19,0.09,0.20,0.12,5.82,6.04,0.90,0.69,0.89,3.77
-1,1.10,1.02,0.32,1.70,1.05,0.14,308.10,0.89,76.61,85.83,0.12,1.39,3 230.41,2.36,90.81,172.35,78.78,3 350.01,0.02,1.04,0.05,0.56,0.19,2.72,2.10,0.38,0.46,0.64,4.13
+1,1.10,1.02,0.32,1.70,1.05,0.14,308.10,0.89,76.61,85.83,0.12,1.39,3230.41,2.36,90.81,172.35,78.78,3350.01,0.02,1.04,0.05,0.56,0.19,2.72,2.10,0.38,0.46,0.64,4.13
 1,0.83,0.65,0.42,0.25,0.02,0.00,-25.50,0.80,20.81,26.04,0.05,1.26,0.65,4.43,0.03,0.21,0.03,0.41,0.06,0.80,0.41,0.05,0.32,19.78,2.57,1.96,0.14,0.15,-0.39
 1,2.52,1.62,-1.00,0.84,0.56,0.00,235.55,0.56,-35.70,-64.31,0.08,3.78,2.02,0.00,0.12,0.25,0.06,-222.78,0.00,-0.24,0.00,0.19,0.12,0.89,1.55,0.50,0.26,0.47,-3.07
 1,0.45,0.76,-1.00,11.01,6.77,1.13,253.68,0.60,-18.05,-30.13,0.02,69.51,0.43,41.36,0.01,0.47,0.01,-1.23,0.01,-2.58,0.99,0.09,1.09,0.15,1.44,0.72,0.01,0.02,0.06
 1,0.87,0.64,1.04,1.13,0.54,0.23,2.58,0.79,4.75,6.01,0.15,1.08,16.46,2.49,0.18,0.68,0.13,0.86,0.01,0.04,0.03,0.98,0.55,141.70,0.70,0.39,0.19,0.19,204.33
 1,49.57,0.65,-1.00,1.65,0.16,0.09,-219.90,1.37,-2.76,-2.01,0.04,0.00,1.19,0.00,0.05,0.33,0.07,1.37,0.05,1.03,0.25,0.49,0.27,66.38,121.63,1.60,0.22,0.27,3.61
 1,0.00,0.88,-1.00,25.47,0.14,0.14,-10.74,0.75,-11.00,-14.59,0.01,0.00,34.14,0.00,0.38,0.00,0.35,-64.78,0.01,-2.00,0.00,0.00,0.00,0.00,0.00,33.99,0.00,0.00,0.00
 1,0.98,0.88,1.35,2.25,1.27,0.09,86.46,0.60,3.82,6.35,0.21,2.06,0.03,7.41,0.01,0.00,0.00,0.03,0.07,0.47,0.06,0.15,0.11,3.64,5.85,4.79,1.17,2.40,3.77
@@ -394,8 +394,8 @@
 1,0.54,0.20,-1.00,2.05,2.32,0.27,0.00,0.57,-2.65,-4.66,0.18,0.63,0.30,5.55,0.04,0.09,0.04,0.21,0.08,0.45,0.18,0.37,0.37,0.29,0.20,-0.80,0.42,3.10,0.62
 1,1.20,0.00,-1.00,0.00,2.97,0.00,0.00,2.78,-1.56,-0.56,0.00,0.00,1.00,0.00,0.01,0.23,0.03,0.03,0.03,0.03,0.23,0.60,0.23,0.05,0.08,0.03,0.11,0.11,-0.12
 1,0.76,0.60,1.28,0.81,0.10,0.01,73.01,0.37,13.97,37.34,0.13,1.04,0.97,2.05,0.10,0.08,0.04,1.61,0.01,0.24,0.01,0.25,0.08,5.00,0.60,0.51,0.49,2.30,-2.71
 1,1.29,0.52,-1.00,0.15,0.07,0.00,17.84,0.59,-1.09,-1.85,0.09,0.59,0.38,1.46,0.03,0.03,0.02,-0.08,0.04,-0.16,0.06,0.11,0.08,8.93,9.36,5.88,0.62,0.74,-0.77
 1,0.98,1.22,-1.00,0.28,0.02,0.00,-327.24,0.65,-9.10,-14.08,0.13,0.67,0.83,2.06,0.08,0.12,0.05,-7.19,0.01,-2.00,0.03,0.38,0.14,37.58,33.10,1.05,0.43,0.48,-1.60
 1,0.75,3.05,-1.00,0.05,0.00,0.00,0.00,1.17,-0.47,-0.41,0.12,0.42,0.69,1.84,0.08,2.18,0.09,-0.49,0.45,-2.37,10.58,1.00,3.15,0.00,0.00,0.00,0.04,0.05,-0.02
 1,0.55,0.64,0.55,1.09,0.42,0.10,130.92,0.39,1.35,3.46,0.63,1.01,0.40,2.71,0.04,0.01,0.01,0.04,0.00,0.01,0.00,0.10,0.03,5.09,3.91,10.69,1.27,5.48,21.91
-1,0.01,0.95,-1.00,1.61,1.63,0.02,174.49,1.07,-5.89,-5.49,0.24,0.00,1.00,10.95,0.94,161.90,0.94,3.15,0.18,0.60,31.01,117.35,41.71,0.04,2.09,0.00,0.01,0.01,0.09
+1,0.01,0.95,-1.00,1.61,1.63,0.02,174.49,1.07,-5.89,-5.49,0.24,0.00,1.00,10.95,0.94,161.90,0.94,3.15,0.18,0.60,31.01,117.35,41.71,0.04,2.09,0.00,0.01,0.01,0.09
```

### Comparing `AFR-0.2.2/load/finratKZ_dataset.html` & `AFR-0.2.7/AFR/load/finratKZ_dataset.html`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/load/finratKZ_dataset.rst` & `AFR-0.2.7/AFR/load/finratKZ_dataset.rst`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/load/macroKZ.csv` & `AFR-0.2.7/AFR/load/macroKZ.csv`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-﻿date,real_gdp,GDD_Agr_R,GDD_Min_R,GDD_Man_R,GDD_Elc_R,GDD_Con_R,GDD_Trd_R,GDD_Trn_R,GDD_Inf_R,GDD_Est_R,GDD_R,Rincpop_q,Rexppop_q,Rwage_q,imp,exp,usdkzt,eurkzt,rurkzt,poil,GDP_DEF,cpi,realest_resed_prim,realest_resed_sec,realest_comm,index_stock_weighted,ntrade_Agr,ntrade_Min,ntrade_Man,ntrade_Elc,ntrade_Con,ntrade_Trd,ntrade_Trn,ntrade_Inf,fed_fund_rate,govsec_rate_kzt_3m,govsec_rate_kzt_1y,govsec_rate_kzt_7y,govsec_rate_kzt_10y,tonia_rate,rate_kzt_mort_0y_1y,rate_kzt_mort_1y_iy,rate_kzt_corp_0y_1y,rate_usd_corp_0y_1y,rate_kzt_corp_1y_iy,rate_usd_corp_1y_iy,rate_kzt_indv_0y_1y,rate_kzt_indv_1y_iy,realest_resed_prim_rus,realest_resed_sec_rus,cred_portfolio,coef_k1,coef_k3,provisions,percent_margin,com_inc, com_exp ,oper_inc,oth_inc,DR
-Q1-2010,2434.9,137.1,403.2,244.9,43.0,274.2,287.8,210.9,94.0,221.1,2320.8,22.5,38.7,44.5,5677.7,13581.9,147.7,204.9,4.9,76.7,165.1,153.9,101.3,100.4,100.6,106.9,77.5,99.5,88.5,96.4,105.8,94.8,74.5,70.7,0.1,1.5,3.1,7.8,7.7,0.1,10.7,11.3,14.9,11.0,14.5,12.9,30.3,21.5,100.6,101,193.00,0.31,0.03,83.91,0.06,1125517.36,175988.45,3211104.05,411132.70,0.02
-Q2-2010,2506.4,139.7,406.1,273.0,42.8,273.9,309.8,206.1,97.5,197.6,2374.0,24.4,38.7,49.2,7909.4,16312.5,146.8,187.0,4.9,78.7,187.2,156.8,99.8,100.2,100.8,74.6,101.9,100.7,111.5,99.6,99.9,107.6,97.7,103.7,0.2,1.5,2.6,7.3,7.3,0.2,11.2,11.4,14.2,11.0,13.4,12.3,25.5,21.3,99.5,100.3,183.28,0.32,0.06,74.55,0.06,1509069.76,191369.75,3776480.95,369998.20,0.02
-Q3-2010,2512.3,116.7,349.5,242.1,43.3,285.0,319.6,247.9,86.6,204.5,2270.6,25.9,46.4,51.1,9278.9,15415.5,147.4,190.2,4.8,76.4,215.9,157.9,100.2,101.1,100.7,108.9,83.5,86.1,88.7,101.0,104.0,103.2,120.3,88.8,0.2,1.2,2.4,7.8,6.8,0.3,12.8,11.1,13.8,10.6,13.2,12.0,24.7,20.9,100,100.4,243.65,0.43,0.25,86.63,0.06,1811025.26,219077.65,3417365.05,361438.00,0.02
-Q4-2010,2816.4,125.2,456.9,279.4,44.1,287.0,349.4,305.4,143.7,246.5,2687.8,26.3,47.8,52.2,10025.6,16081.7,147.5,200.6,4.8,86.8,272.7,161.2,101.5,101.9,99.9,111.8,107.3,130.7,115.4,101.9,100.7,109.3,123.2,166.0,0.2,0.9,2.4,8.9,7.9,0.3,11.3,10.5,13.5,9.9,11.6,9.5,28.2,20.3,100.2,100.9,232.46,0.33,0.04,80.06,0.06,2059290.86,178291.85,3913204.35,390177.70,0.02
-Q1-2011,2588.7,135.5,410.9,260.1,44.4,274.9,319.9,219.2,108.6,216.5,2464.5,24.9,47.0,48.5,7305.4,16576.7,146.4,199.9,5.0,104.9,202.4,167.0,104.3,103.4,100.1,101.2,108.3,89.9,93.1,100.7,95.8,91.6,71.8,75.6,0.2,0.9,1.7,8.9,8.9,0.2,13.4,11.1,12.9,10.4,11.4,6.3,28.4,22.8,101.5,101.3,234.03,0.32,0.04,78.81,0.06,1784063.16,239975.45,4062113.55,411328.50,0.03
-Q2-2011,2716.2,137.4,408.4,287.4,44.7,267.2,344.4,212.1,106.8,194.8,2586.1,25.6,48.1,50.1,11144.2,25591.2,145.6,209.6,5.2,117.1,220.9,170.0,100.9,101.6,100.0,89.7,101.3,99.4,110.5,100.7,97.2,107.7,96.8,98.3,0.1,0.8,1.8,8.4,8.4,0.2,13.1,11.8,12.6,9.7,11.4,10.0,24.5,22.2,101.6,101.1,239.85,0.34,0.04,78.75,0.06,3208277.16,303592.85,4482621.55,464637.80,0.03
-Q3-2011,2686.6,151.0,332.4,260.3,45.8,291.6,359.6,257.1,101.4,202.7,2417.8,27.5,52.3,53.9,10379.1,22174.4,146.6,207.4,5.1,112.5,276.4,171.9,101.0,101.8,100.4,72.9,109.9,81.4,90.6,102.4,109.1,104.4,121.2,95.0,0.1,1.2,1.8,9.2,9.2,0.5,10.6,11.8,11.9,9.0,11.2,7.8,22.0,22.2,101.7,101,258.85,0.33,0.04,89.65,0.06,5072943.26,291576.45,4935996.45,439672.20,0.03
-Q4-2011,3045.2,214.0,435.2,278.8,48.3,286.1,380.2,313.5,178.9,281.0,2915.7,29.4,54.8,58.0,11521.1,20851.6,147.9,199.6,4.7,109.3,314.5,173.6,101.2,102.1,96.7,98.3,141.7,130.9,107.1,105.4,98.1,105.7,121.9,176.4,0.1,1.0,1.9,4.2,4.9,0.8,11.6,11.3,11.3,8.1,10.4,6.5,21.5,22.7,101.8,102.4,274.81,0.29,0.04,95.32,0.06,7161793.76,1595814.55,4143869.95,471466.60,0.03
-Q1-2012,2763.2,128.2,407.5,282.0,47.5,271.8,362.1,233.6,123.2,219.6,2585.6,27.6,52.9,54.1,9171.5,20759.3,148.1,194.1,4.9,118.6,220.7,175.5,102.5,100.9,102.1,112.7,59.9,93.6,101.1,98.4,95.0,95.2,74.5,68.8,0.1,1.0,2.3,4.4,4.8,0.1,11.5,12.1,11.4,7.3,11.0,9.5,22.1,23.6,103.3,103.2,278.55,0.30,0.04,93.95,0.06,8180743.56,494057.85,4897327.05,467215.10,0.03
-Q2-2012,2886.1,127.2,404.2,297.2,46.9,270.6,393.8,226.5,117.9,212.3,2713.9,28.5,50.7,56.3,10940.6,23380.8,148.2,190.2,4.8,108.9,233.9,178.3,104.1,105.0,103.9,78.1,99.3,99.2,105.4,98.7,99.6,108.8,97.0,95.7,0.2,1.4,1.7,5.0,5.0,0.6,12.7,12.4,11.3,6.8,11.2,10.0,21.2,22.9,103.1,102.8,288.36,0.27,0.05,109.60,0.05,9804025.66,501211.15,5441141.75,473144.10,0.03
-Q3-2012,2770.3,132.0,324.7,242.1,45.8,306.7,408.4,275.6,108.5,217.3,2517.0,29.2,53.2,57.5,12323.1,21347.2,149.7,187.2,4.7,110.0,288.8,180.3,102.9,103.8,100.3,99.2,103.8,80.3,81.5,97.7,113.3,103.7,121.7,92.0,0.1,1.5,2.3,5.0,5.8,1.1,11.5,12.2,10.9,9.0,11.7,8.9,20.6,23.1,102.4,102.8,294.62,0.28,0.04,111.35,0.05,11466380.86,556698.45,5900619.45,490055.50,0.03
-Q4-2012,3140.8,137.2,450.0,293.0,48.9,300.4,437.9,340.9,245.3,311.5,3112.1,30.2,55.5,59.3,14222.5,21007.2,150.4,195.1,4.8,110.5,323.7,183.7,102.2,102.9,98.9,100.3,103.9,138.6,121.0,106.7,98.0,107.2,123.7,226.1,0.2,2.1,2.3,5.8,5.8,1.6,11.4,11.5,10.8,7.9,10.3,9.6,23.8,24.1,101.4,102.8,306.75,0.27,0.04,114.54,0.05,14360588.66,529075.25,8334609.25,550668.80,0.03
-Q1-2013,2881.1,128.5,420.2,284.0,46.5,258.0,408.5,249.7,135.4,224.3,2699.0,28.2,53.5,54.5,9952.6,20726.3,150.7,199.1,5.0,112.9,241.8,187.6,102.4,104.7,101.5,98.3,93.7,93.4,96.9,95.2,85.9,93.3,73.2,55.2,0.1,2.0,2.7,7.1,7.1,0.5,12.7,11.8,10.4,6.9,11.0,10.8,20.4,24.0,101.9,101.7,310.08,0.27,0.04,98.28,0.06,15007259.96,615677.15,6844761.55,762181.20,0.03
-Q2-2013,3051.7,129.8,409.5,300.7,48.2,287.3,439.0,245.3,135.9,219.5,2860.0,29.4,53.7,56.6,12883.6,22137.4,151.1,197.3,4.8,103.0,246.8,189.3,102.3,103.9,100.3,90.8,101.0,97.5,105.9,103.5,111.3,107.5,98.2,100.4,0.1,2.4,2.9,6.1,6.1,0.9,10.9,11.6,10.7,7.3,10.4,9.7,18.1,22.5,101.1,101,322.52,0.25,0.04,124.37,0.06,17722751.86,634535.55,7620005.25,781312.40,0.03
-Q3-2013,2958.4,149.4,343.3,240.0,46.8,323.5,461.2,296.5,122.0,219.3,2680.1,30.0,55.4,57.5,12837.2,20191.8,152.9,202.6,4.7,110.1,313.3,190.4,101.7,103.1,100.4,103.0,115.1,83.8,79.8,97.2,112.6,105.1,120.9,89.8,0.1,2.0,2.7,5.9,5.9,2.8,11.7,11.8,10.4,7.1,11.7,10.5,20.0,21.3,101.2,100.4,333.51,0.25,0.04,110.47,0.06,21135859.36,682799.15,10163721.15,884096.40,0.03
-Q4-2013,3360.0,174.7,466.1,320.0,49.0,318.8,484.1,365.8,276.5,315.2,3316.3,31.2,56.9,60.7,13492.5,22070.5,153.8,209.4,4.7,109.4,364.0,192.3,103.7,102.7,100.7,102.0,117.0,135.8,133.3,104.6,98.5,105.0,123.3,226.6,0.1,2.1,3.0,4.8,4.8,2.6,11.2,11.5,10.4,7.2,10.5,8.2,19.3,21.5,100.5,100.4,351.27,0.24,0.04,145.09,0.06,22030328.76,753596.25,8997647.45,1123733.60,0.03
-Q1-2014,3000.3,132.2,415.0,277.4,47.2,267.4,458.8,264.7,150.2,223.1,2796.1,29.1,53.9,55.1,8524.0,23034.1,170.2,233.3,4.8,107.9,264.4,197.5,107.4,109.4,101.1,114.0,75.7,89.1,86.7,96.3,83.9,94.8,72.4,54.3,0.1,2.3,3.0,6.4,6.4,7.9,11.4,11.4,10.5,7.9,10.5,8.4,14.9,21.5,102.1,101.2,381.67,0.25,0.04,166.11,0.06,19068753.66,815828.75,9393061.15,1238286.50,0.02
-Q2-2014,3170.1,133.0,407.7,297.2,48.8,299.3,466.9,262.6,144.8,224.5,2957.7,30.7,53.2,59.8,11033.3,19681.9,182.7,250.4,5.2,109.8,269.7,202.1,104.1,105.1,100.9,107.3,100.6,98.2,107.1,103.5,111.9,101.8,99.2,96.4,0.1,2.3,3.1,7.1,7.1,0.7,11.4,11.0,10.7,7.2,10.9,9.7,13.6,20.9,102,101.3,382.52,0.25,0.04,157.37,0.06,19721550.86,773559.05,9521521.35,1427547.00,0.02
-Q3-2014,3074.8,147.2,346.2,245.6,47.7,337.2,498.5,316.0,127.6,235.1,2788.9,30.9,55.4,59.9,11417.9,19340.6,182.5,242.2,5.0,102.1,343.4,204.1,99.7,101.5,100.6,107.0,110.7,84.9,82.6,97.8,112.7,106.8,120.3,88.1,0.1,2.8,3.4,7.2,7.2,1.4,11.5,11.4,10.1,6.7,10.7,9.2,17.9,20.1,100.4,100.9,380.32,0.24,0.04,144.57,0.06,22769776.26,757296.65,10027824.95,1592141.10,0.02
-Q4-2014,3522.1,176.1,467.7,339.9,51.2,335.3,509.1,394.3,299.8,336.3,3481.3,32.2,56.8,63.2,11478.5,17016.1,181.4,226.6,3.9,76.0,358.7,206.9,100.3,100.9,100.6,78.7,119.7,135.1,138.4,107.4,99.4,102.1,124.8,235.0,0.1,3.3,3.8,7.8,7.8,17.3,11.2,11.2,12.4,7.6,9.7,8.4,16.6,20.8,101.2,101.7,373.28,0.23,0.06,108.52,0.06,25161537.06,287272.15,11044545.05,1769326.90,0.02
-Q1-2015,3060.2,135.5,418.7,276.8,46.0,271.4,469.0,283.6,157.0,227.8,2868.0,29.5,53.3,56.5,7917.9,11725.0,184.6,208.3,2.9,53.9,270.2,209.8,101.3,100.7,100.8,85.3,76.9,89.5,81.4,89.8,80.9,92.1,71.9,52.4,0.1,8.4,3.9,10.0,10.0,14.7,15.7,9.5,19.5,7.1,11.7,9.1,19.6,21.3,101.8,101,392.59,0.33,0.05,112.18,0.06,25713283.86,591316.55,10891206.15,1714334.60,0.02
-Q2-2015,3214.1,135.8,411.4,299.6,48.2,321.9,482.5,278.7,144.8,227.0,3024.9,31.5,52.1,59.0,9152.0,12210.0,185.9,205.3,3.5,62.1,265.6,210.7,99.4,99.1,100.7,111.2,100.2,98.2,108.2,104.6,118.6,102.9,98.3,92.2,0.1,8.4,3.9,10.3,10.4,7.6,12.1,9.5,15.5,6.8,12.5,9.2,15.7,18.2,99.2,99.3,357.26,0.44,0.32,46.14,0.06,25802870.06,657638.85,13689096.85,1822801.20,0.02
-Q3-2015,3083.7,151.4,319.1,253.0,46.6,347.7,482.7,328.0,129.7,238.9,2795.3,32.1,54.1,58.8,8577.6,11108.9,216.2,240.9,3.4,50.0,344.8,212.1,102.2,102.0,100.3,89.6,111.5,77.6,84.5,96.8,108.0,100.0,117.7,89.6,0.1,4.7,4.7,6.2,6.1,8.1,10.0,9.9,14.7,6.6,11.6,9.5,17.8,18.2,99.1,98.2,410.00,0.43,0.29,50.54,0.06,25055203.36,952520.25,11179606.35,1701102.70,0.02
-Q4-2015,3561.2,184.1,440.4,328.7,50.5,347.8,501.4,413.1,318.3,351.0,3545.9,31.5,52.6,58.8,7551.7,9782.5,300.2,328.7,4.6,43.4,377.6,231.4,108.1,105.6,100.3,106.7,121.6,138.0,129.9,108.3,100.0,103.9,125.9,245.4,0.2,13.2,11.1,7.4,6.8,36.6,17.2,9.6,16.2,7.6,12.6,6.4,15.1,17.9,99.6,98.3,444.39,0.30,0.04,52.98,0.06,26117137.86,1094862.45,11963387.15,1595414.70,0.02
-Q1-2016,3059.0,138.6,411.7,276.8,45.6,286.9,439.1,294.6,150.8,230.7,2860.1,29.7,50.0,55.0,5371.5,8022.7,356.6,392.6,4.8,34.4,304.3,241.4,104.8,104.6,100.7,113.2,75.3,93.5,84.2,90.2,82.5,87.6,71.3,47.4,0.4,14.9,13.4,9.1,8.5,24.9,4.0,9.2,21.6,8.2,12.9,7.7,18.5,19.1,100.3,99.5,446.26,0.33,0.04,50.51,0.06,26723519.46,913089.65,11898493.75,1552554.30,0.02
-Q2-2016,3223.2,138.4,390.4,300.7,47.6,343.8,466.0,290.0,137.9,231.2,3029.4,31.0,48.4,58.4,6364.8,8217.3,335.6,379.0,5.1,46.0,311.7,246.0,97.7,98.5,100.1,101.6,99.8,94.8,108.6,104.5,119.8,106.1,98.4,91.4,0.4,14.5,13.5,9.3,8.4,14.4,15.5,9.4,17.4,8.4,14.2,7.9,20.9,19.2,99.8,99,450.46,0.37,0.03,51.56,0.06,26455285.56,1163709.25,11786904.25,1729624.60,0.02
-Q3-2016,3099.8,164.0,295.7,254.3,47.4,372.3,483.5,337.9,125.5,243.8,2824.9,30.6,50.2,56.7,6841.7,9236.0,341.5,381.1,5.3,45.8,387.1,248.9,99.9,99.4,100.1,120.7,118.5,75.7,84.6,99.6,108.3,103.7,116.5,91.0,0.4,13.1,12.3,10.5,9.3,12.3,18.0,9.8,15.9,7.9,14.8,9.0,22.4,20.4,99.8,99,455.60,0.49,0.33,53.09,0.06,26721196.26,1284186.75,11302902.05,701928.70,0.02
-Q4-2016,3681.3,196.7,452.3,343.5,51.1,377.1,506.5,422.3,339.3,363.0,3668.9,32.5,52.2,61.0,7654.4,10009.8,334.9,361.9,5.3,50.1,424.2,253.7,98.5,99.0,100.2,114.0,120.0,153.0,135.0,107.7,101.3,104.8,125.0,270.3,0.5,11.8,12.0,9.6,10.0,11.5,14.6,9.6,15.3,6.8,14.6,7.7,22.0,19.9,99.7,99.5,410.68,0.40,0.03,47.14,0.06,27878091.56,1826890.45,12130778.55,746191.60,0.02
-Q1-2017,3171.3,142.2,436.5,297.2,47.3,307.4,451.6,305.0,153.5,233.9,2963.7,30.4,51.1,53.9,6274.9,10540.2,322.5,343.3,5.5,54.1,328.9,260.3,99.6,99.6,100.3,114.5,72.3,96.5,86.5,92.6,81.5,89.2,72.2,45.2,0.7,10.6,11.3,9.3,8.8,10.9,9.9,9.7,14.0,6.2,13.9,7.8,22.0,19.4,100.1,99.7,462.06,0.53,0.31,57.04,0.06,28567564.96,1536978.85,15970284.55,680585.40,0.02
-Q2-2017,3380.5,142.6,444.5,319.9,50.7,360.7,475.6,302.6,142.7,237.7,3174.3,31.2,50.4,56.7,7875.8,11946.3,314.7,345.9,5.5,50.2,328.8,264.4,100.3,99.8,99.9,106.8,100.2,101.8,107.7,107.2,117.3,105.3,99.2,93.0,1.0,9.8,9.2,9.2,8.3,10.0,15.9,9.7,13.7,6.1,14.2,7.6,21.6,19.7,100.3,99.5,470.71,0.52,0.30,59.81,0.06,30818177.06,1312502.95,10515776.15,744223.70,0.02
-Q3-2017,3228.9,164.1,342.4,265.0,50.0,370.3,503.6,358.6,130.7,251.3,2940.6,31.3,52.2,55.6,7882.8,11254.3,332.4,390.3,5.6,51.7,421.1,266.3,101.2,99.9,99.9,123.5,115.1,77.0,82.8,98.7,102.7,105.9,118.5,91.6,1.2,9.2,9.0,8.9,9.0,9.4,13.5,9.7,13.4,5.3,13.8,8.0,22.0,19.8,100.1,99.1,421.30,0.50,0.30,73.82,0.06,34108887.56,1440663.95,13902272.45,784476.00,0.03
-Q4-2017,3821.6,209.4,474.6,365.4,54.2,380.8,525.7,443.7,351.1,367.8,3801.0,33.1,53.5,60.2,8539.7,13560.3,334.4,393.7,5.7,61.5,503.4,272.1,99.9,99.3,100.1,105.9,127.6,138.6,137.9,108.3,102.8,104.4,123.7,268.6,1.2,9.3,9.2,8.9,8.8,9.3,14.6,9.3,13.1,5.2,14.4,5.5,21.5,20.6,100.6,100.1,231.49,0.38,0.03,25.49,0.06,38939710.26,1649264.65,15346462.45,940450.50,0.03
-Q1-2018,3307.8,147.0,459.0,314.8,49.2,325.4,478.9,318.8,163.0,239.2,3099.7,31.1,53.4,54.9,7575.4,13669.9,323.2,397.3,5.7,67.0,356.3,277.6,100.6,99.7,100.0,112.2,70.2,96.7,86.2,90.8,85.4,91.1,71.9,46.4,1.4,8.9,8.6,8.9,8.9,8.8,7.9,9.6,12.8,5.4,13.8,5.7,23.4,20.7,101.2,100.8,229.18,0.38,0.03,25.51,0.06,39247807.06,1873724.05,13284024.05,881350.80,0.03
-Q2-2018,3519.5,149.0,470.8,332.8,53.8,367.8,502.5,318.2,151.0,241.2,3298.7,32.4,52.3,57.9,8478.8,14691.7,329.8,393.5,5.3,74.5,371.4,280.9,101.0,100.3,100.0,99.0,101.4,102.6,105.7,109.3,113.0,104.9,99.8,92.6,1.7,8.3,8.4,8.4,8.5,8.3,8.9,9.8,12.0,5.4,12.8,5.1,21.0,21.1,101.9,100.8,237.64,0.42,0.03,25.08,0.06,43997235.26,1982946.35,14813646.65,997580.10,0.04
-Q3-2018,3352.7,161.6,354.0,278.1,50.8,390.4,544.4,373.1,131.3,261.7,3052.5,33.6,53.9,57.3,9083.1,15366.4,356.0,413.8,5.5,75.5,444.7,282.3,100.3,100.4,100.1,91.0,108.5,75.2,83.6,94.5,106.1,108.3,117.3,87.0,1.9,8.4,8.8,9.1,8.4,8.4,14.1,8.7,12.1,5.4,12.8,4.9,20.9,19.8,101.6,100.7,471.22,0.53,0.37,67.48,0.06,48800906.66,2724046.05,15331709.25,1121266.30,0.04
-Q4-2018,3976.5,225.3,491.2,377.2,52.9,400.2,574.3,463.8,364.0,380.8,3952.2,35.0,57.0,61.4,9109.8,16098.3,369.8,422.1,5.6,67.4,554.6,286.5,100.6,100.7,100.1,104.9,139.4,138.8,135.6,104.0,102.5,105.5,124.3,277.2,2.2,8.8,8.7,8.7,8.5,8.3,11.3,8.2,12.4,5.2,11.4,6.1,21.1,19.3,101.4,101.8,491.53,0.39,0.04,63.45,0.06,53885717.16,1115202.55,17667145.65,1197715.20,0.04
-Q1-2019,3430.9,151.3,477.5,319.1,48.6,352.4,510.6,331.1,167.2,243.2,3214.8,33.3,55.9,57.8,7258.6,14364.5,377.7,429.1,5.7,63.3,384.2,291.1,101.0,100.9,100.2,107.0,67.2,97.2,84.6,91.9,88.1,88.9,71.4,45.9,2.4,8.8,8.8,8.8,8.7,8.3,11.0,8.1,12.2,5.6,13.0,5.4,20.9,20.0,102.3,101.1,465.88,0.39,0.05,83.62,0.06,52226897.36,4065848.05,16285468.65,1114377.00,0.05
-Q2-2019,3674.1,153.1,465.8,346.9,56.0,413.5,539.7,336.1,157.3,247.1,3443.2,35.1,53.8,63.1,7258.6,14364.5,380.6,427.5,5.9,68.3,400.8,295.2,101.4,101.3,100.0,93.0,101.2,97.6,108.7,115.2,117.3,105.7,101.5,94.1,2.4,8.8,8.7,8.7,8.6,8.2,12.0,8.1,11.8,5.0,12.0,6.0,19.9,20.4,101.5,100.5,487.39,0.37,0.05,80.59,0.06,61132600.76,4276646.55,18400683.95,1268472.70,0.05
-Q3-2019,3518.9,148.5,371.9,287.9,52.8,457.2,582.6,392.8,136.2,267.0,3209.6,35.4,56.2,67.7,7258.6,14364.5,385.8,429.2,6.0,61.9,465.8,297.3,101.1,102.0,99.9,94.8,97.0,79.8,83.0,94.4,110.6,108.0,116.9,86.5,2.2,9.8,10.0,9.2,9.2,8.5,7.0,8.1,11.8,4.5,12.4,5.2,20.4,21.3,102.1,101.8,528.02,0.33,0.06,83.55,0.06,65828104.76,5641360.45,18106110.55,4145285.10,0.05
-Q4-2019,4170.2,225.7,505.0,417.2,49.4,447.3,604.1,485.2,380.6,385.8,4145.8,36.8,58.5,71.1,7258.6,14364.5,386.9,428.2,6.1,62.7,605.1,302.0,102.6,101.8,100.1,108.7,152.0,135.8,144.9,93.4,97.8,103.7,123.5,279.5,1.6,9.9,9.3,9.6,9.5,8.8,2.8,7.5,11.9,4.6,13.1,4.7,17.4,19.6,101.9,100.4,403.74,0.34,0.06,56.19,0.06,70627071.46,5241812.95,19382747.45,1012652.30,0.05
-Q1-2020,3509.2,153.4,495.9,343.4,47.5,389.3,510.1,323.2,183.0,241.7,3299.5,35.7,57.1,64.8,7258.6,14364.5,389.6,429.9,5.9,50.5,430.1,308.7,101.7,101.9,100.4,94.2,68.0,98.2,82.3,96.3,87.0,84.4,66.6,48.1,1.3,12.2,10.7,10.7,10.6,10.0,15.7,8.4,12.0,4.2,13.7,5.7,21.7,20.8,101.4,100.2,415.71,0.33,0.06,59.38,0.06,67784541.66,5168664.05,19620102.15,890662.30,0.05
-Q2-2020,3446.9,154.3,457.6,347.6,58.5,453.1,419.7,239.7,175.5,222.3,3237.0,35.4,52.8,67.2,8758.3,11688.7,418.1,459.9,5.8,31.4,386.0,315.5,100.5,101.5,96.7,105.4,100.6,92.3,101.2,123.1,116.4,82.3,74.2,95.9,0.1,10.0,10.8,10.6,10.6,8.8,5.0,7.8,11.4,4.2,11.9,6.9,23.8,19.4,102.7,101.4,403.00,0.39,0.05,51.85,0.06,66900692.76,5374901.95,19052286.55,132100.10,0.05
-Q3-2020,3333.6,162.6,317.4,284.5,52.0,494.4,531.9,306.2,132.2,294.0,3041.1,35.3,56.4,67.6,10425.9,9328.2,417.9,488.2,5.7,42.7,522.1,318.3,101.1,103.3,99.6,103.5,105.4,69.4,81.8,88.9,109.1,126.8,127.8,75.3,0.1,9.5,10.2,10.3,10.3,8.6,7.1,7.6,11.7,3.1,13.1,5.1,21.2,20.6,103.7,103.2,588.70,0.56,0.38,73.73,0.06,70349533.76,6146130.65,20662672.25,897458.10,0.05
-Q4-2020,4132.4,240.4,457.4,434.8,46.3,507.1,677.9,312.3,428.7,372.6,4109.4,38.7,59.1,75.8,9765.6,11333.1,426.2,507.8,5.6,44.5,601.2,324.0,101.8,104.5,100.4,110.2,147.8,144.1,152.8,89.0,102.6,127.5,102.0,324.2,0.1,9.5,10.0,9.8,10.0,8.7,1.8,7.5,11.5,4.4,12.1,5.5,18.1,18.2,103.7,104.4,607.39,0.46,0.05,70.42,0.05,75289906.56,5253623.65,22925783.65,1199838.20,0.04
-Q1-2021,3485.0,156.6,457.9,366.5,49.5,437.2,493.3,265.1,199.7,237.1,3283.2,36.5,56.8,70.5,7605.8,11455.4,419.7,506.4,5.6,60.6,463.7,330.8,104.5,109.7,101.2,116.3,64.6,99.3,83.6,106.1,85.6,72.2,84.2,46.2,0.1,9.1,9.1,10.2,10.0,8.7,10.8,8.0,11.7,4.1,13.1,5.4,19.1,20.1,106,103.6,631.71,0.40,0.05,72.03,0.05,67245860.84,4222873.49,20497372.43,1469224.27,0.04
-Q2-2021,3681.9,158.4,460.5,357.4,61.6,498.8,508.3,266.4,215.0,226.9,3448.7,35.9,58.3,79.7,9884.9,15480.3,428.4,515.9,5.8,68.6,442.2,338.5,103.5,105.2,100.1,107.3,101.4,100.6,97.7,124.4,114.1,103.0,100.5,100.0,0.1,8.7,9.2,10.1,10.1,8.4,8.5,8.3,11.6,5.9,13.0,4.2,19.3,19.0,107,104.4,728.89,0.54,0.40,61.24,0.05,72410915.24,4335545.66,20905741.68,1489553.73,0.04
-Q3-2021,3621.8,158.5,333.5,300.0,55.4,520.2,584.7,332.3,167.6,297.0,3289.5,61.0,59.7,70.5,10994.8,16201.8,425.7,502.0,5.8,73.0,573.3,345.6,102.9,103.2,100.1,101.2,100.1,72.4,83.9,90.0,104.3,115.0,124.7,77.9,0.1,9.4,9.8,10.1,10.1,8.8,9.4,8,11.6,3.9,13.0,4.7,18.9,19.2,105.1,103.4,822.04,0.55,0.44,62.84,0.05,77689778.61,4449455.98,21318598.51,1510106.60,0.04
-Q4-2021,4210.4,215.2,493.4,453.5,46.1,513.9,733.7,351.4,448.4,392.1,4343.5,61.0,61.0,78.3,11558.2,17091.6,429.8,491.7,5.9,79.6,646.9,351.8,103.8,103.9,100.8,108.6,135.7,148.0,151.2,83.2,98.8,125.5,105.8,267.6,0.1,9.8,9.9,10.3,10.3,9.6,12.3,8.5,11.5,4.1,14.5,5.2,15.7,19.1,105.7,104.7,918.20,0.39,0.05,63.95,0.05,74562995.83,4563366.30,21731455.33,1530659.47,0.05
-Q1-2022,3573.7,157.4,438.6,385.4,48.5,468.9,526.1,286.1,228.2,231.3,3354.4,41.2,60.5,78.6,9136.6,19059.5,455.1,510.8,5.3,99.0,551.1,362.7,105.7,110.6,100.6,91.04,100.1,98.9,101.3,99.5,101.6,101.5,101.6,102.8,0.1,13.1,13.2,10.9,9.9,11.8,13.9,8.7,13.0,4.5,13.2,4.4,14.9,20.6,108,106.5,904.24,0.60,0.48,69.12,0.06,73590762.04,4894401.58,23450458.36,1661117.26,0.05
-Q2-2022,3771.0,160.2,451.8,375.4,61.5,546.6,530.8,274.4,214.9,190.8,3520.6,39.4,58.4,80.9,11595.6,23307.5,442.5,472.4,6.8,112.7,528.2,385.5,106.1,107.5,100.5,79.95,100.3,99.5,101.2,100.0,102.4,101.0,100.6,100.0,0.8,13.0,13.4,11.3,10.1,13.9,10.3,8.3,15.5,5.3,15.6,5.2,13.2,19.4,106.5,102,1010.02,0.43,0.05,70.34,0.06,77384487.14,5019702.93,23904600.87,1683725.41,0.05
+Date,real_gdp,GDD_Agr_R,GDD_Min_R,GDD_Man_R,GDD_Elc_R,GDD_Con_R,GDD_Trd_R,GDD_Trn_R,GDD_Inf_R,GDD_Est_R,GDD_R,Rincpop_q,Rexppop_q,Rwage_q,imp,exp,usdkzt,eurkzt,rurkzt,poil,GDP_DEF,cpi,realest_resed_prim,realest_resed_sec,realest_comm,index_stock_weighted,ntrade_Agr,ntrade_Min,ntrade_Man,ntrade_Elc,ntrade_Con,ntrade_Trd,ntrade_Trn,ntrade_Inf,fed_fund_rate,govsec_rate_kzt_3m,govsec_rate_kzt_1y,govsec_rate_kzt_7y,govsec_rate_kzt_10y,tonia_rate,rate_kzt_mort_0y_1y,rate_kzt_mort_1y_iy,rate_kzt_corp_0y_1y,rate_usd_corp_0y_1y,rate_kzt_corp_1y_iy,rate_usd_corp_1y_iy,rate_kzt_indv_0y_1y,rate_kzt_indv_1y_iy,realest_resed_prim_rus,realest_resed_sec_rus,cred_portfolio,coef_k1,coef_k3,provisions,percent_margin,com_inc, com_exp ,oper_inc,oth_inc,DR
+2010-03-31,2434.9,137.1,403.2,244.9,43.0,274.2,287.8,210.9,94.0,221.1,2320.8,22.5,38.7,44.5,5677.7,13581.9,147.7,204.9,4.9,76.7,165.1,153.9,101.3,100.4,100.6,106.9,100.9,112.5,107.9,108.2,99.1,104.2,103.5,101.2,0.1,1.5,3.1,7.8,7.7,0.1,10.7,11.3,14.9,11.0,14.5,12.9,30.3,21.5,100.6,101.0,193.0,0.31,0.03,83.91,0.06,1125517.36,175988.45,3211104.05,411132.7,0.02
+2010-06-30,2506.4,139.7,406.1,273.0,42.8,273.9,309.8,206.1,97.5,197.6,2374.0,24.4,38.7,49.2,7909.4,16312.5,146.8,187.0,4.9,78.7,187.2,156.8,99.8,100.2,100.8,74.6,100.4,107.8,111.4,107.0,100.7,105.5,103.6,105.2,0.2,1.5,2.6,7.3,7.3,0.2,11.2,11.4,14.2,11.0,13.4,12.3,25.5,21.3,99.5,100.3,183.28,0.32,0.06,74.55,0.06,1509069.76,191369.75,3776480.95,369998.2,0.02
+2010-09-30,2512.3,116.7,349.5,242.1,43.3,285.0,319.6,247.9,86.6,204.5,2270.6,25.9,46.4,51.1,9278.9,15415.5,147.4,190.2,4.8,76.4,215.9,157.9,100.2,101.1,100.7,108.9,94.3,103.0,110.3,107.5,103.0,107.0,106.8,103.5,0.2,1.2,2.4,7.8,6.8,0.3,12.8,11.1,13.8,10.6,13.2,12.0,24.7,20.9,100.0,100.4,243.65,0.43,0.25,86.63,0.06,1811025.26,219077.65,3417365.05,361438.0,0.02
+2010-12-31,2816.4,125.2,456.9,279.4,44.1,287.0,349.4,305.4,143.7,246.5,2687.8,26.3,47.8,52.2,10025.6,16081.7,147.5,200.6,4.8,86.8,272.7,161.2,101.5,101.9,99.9,111.8,100.0,112.0,110.8,107.1,103.0,116.4,107.4,105.6,0.2,0.9,2.4,8.9,7.9,0.3,11.3,10.5,13.5,9.9,11.6,9.5,28.2,20.3,100.2,100.9,232.46,0.33,0.04,80.06,0.06,2059290.86,178291.85,3913204.35,390177.7,0.02
+2011-03-31,2588.7,135.5,410.9,260.1,44.4,274.9,319.9,219.2,108.6,216.5,2464.5,24.9,47.0,48.5,7305.4,16576.7,146.4,199.9,5.0,104.9,202.4,167.0,104.3,103.4,100.1,101.2,102.6,106.3,105.2,105.0,101.5,104.4,103.9,103.6,0.2,0.9,1.7,8.9,8.9,0.2,13.4,11.1,12.9,10.4,11.4,6.3,28.4,22.8,101.5,101.3,234.03,0.32,0.04,78.81,0.06,1784063.16,239975.45,4062113.55,411328.5,0.03
+2011-06-30,2716.2,137.4,408.4,287.4,44.7,267.2,344.4,212.1,106.8,194.8,2586.1,25.6,48.1,50.1,11144.2,25591.2,145.6,209.6,5.2,117.1,220.9,170.0,100.9,101.6,100.0,89.7,100.2,108.2,106.4,103.8,100.0,104.8,100.4,104.3,0.1,0.8,1.8,8.4,8.4,0.2,13.1,11.8,12.6,9.7,11.4,10.0,24.5,22.2,101.6,101.1,239.85,0.34,0.04,78.75,0.06,3208277.16,303592.85,4482621.55,464637.8,0.03
+2011-09-30,2686.6,151.0,332.4,260.3,45.8,291.6,359.6,257.1,101.4,202.7,2417.8,27.5,52.3,53.9,10379.1,22174.4,146.6,207.4,5.1,112.5,276.4,171.9,101.0,101.8,100.4,72.9,108.9,106.9,111.9,104.5,99.2,113.2,105.5,103.0,0.1,1.2,1.8,9.2,9.2,0.5,10.6,11.8,11.9,9.0,11.2,7.8,22.0,22.2,101.7,101.0,258.85,0.33,0.04,89.65,0.06,5072943.26,291576.45,4935996.45,439672.2,0.03
+2011-12-31,3045.2,214.0,435.2,278.8,48.3,286.1,380.2,313.5,178.9,281.0,2915.7,29.4,54.8,58.0,11521.1,20851.6,147.9,199.6,4.7,109.3,314.5,173.6,101.2,102.1,96.7,98.3,128.0,95.9,101.2,107.5,107.3,108.8,100.5,93.0,0.1,1.0,1.9,4.2,4.9,0.8,11.6,11.3,11.3,8.1,10.4,6.5,21.5,22.7,101.8,102.4,274.81,0.29,0.04,95.32,0.06,7161793.76,1595814.55,4143869.95,471466.6,0.03
+2012-03-31,2763.2,128.2,407.5,282.0,47.5,271.8,362.1,233.6,123.2,219.6,2585.6,27.6,52.9,54.1,9171.5,20759.3,148.1,194.1,4.9,118.6,220.7,175.5,102.5,100.9,102.1,112.7,101.3,100.9,102.6,105.2,100.9,103.0,102.8,100.4,0.1,1.0,2.3,4.4,4.8,0.1,11.5,12.1,11.4,7.3,11.0,9.5,22.1,23.6,103.3,103.2,278.55,0.3,0.04,93.95,0.06,8180743.56,494057.85,4897327.05,467215.1,0.03
+2012-06-30,2886.1,127.2,404.2,297.2,46.9,270.6,393.8,226.5,117.9,212.3,2713.9,28.5,50.7,56.3,10940.6,23380.8,148.2,190.2,4.8,108.9,233.9,178.3,104.1,105.0,103.9,78.1,101.5,99.7,99.7,102.8,104.4,106.3,104.4,99.7,0.2,1.4,1.7,5.0,5.0,0.6,12.7,12.4,11.3,6.8,11.2,10.0,21.2,22.9,103.1,102.8,288.36,0.27,0.05,109.6,0.05,9804025.66,501211.15,5441141.75,473144.1,0.03
+2012-09-30,2770.3,132.0,324.7,242.1,45.8,306.7,408.4,275.6,108.5,217.3,2517.0,29.2,53.2,57.5,12323.1,21347.2,149.7,187.2,4.7,110.0,288.8,180.3,102.9,103.8,100.3,99.2,103.6,102.2,99.0,98.4,104.1,102.9,100.1,104.4,0.1,1.5,2.3,5.0,5.8,1.1,11.5,12.2,10.9,9.0,11.7,8.9,20.6,23.1,102.4,102.8,294.62,0.28,0.04,111.35,0.05,11466380.86,556698.45,5900619.45,490055.5,0.03
+2012-12-31,3140.8,137.2,450.0,293.0,48.9,300.4,437.9,340.9,245.3,311.5,3112.1,30.2,55.5,59.3,14222.5,21007.2,150.4,195.1,4.8,110.5,323.7,183.7,102.2,102.9,98.9,100.3,88.7,102.8,108.3,101.7,96.2,107.5,110.2,111.0,0.2,2.1,2.3,5.8,5.8,1.6,11.4,11.5,10.8,7.9,10.3,9.6,23.8,24.1,101.4,102.8,306.75,0.27,0.04,114.54,0.05,14360588.66,529075.25,8334609.25,550668.8,0.03
+2013-03-31,2881.1,128.5,420.2,284.0,46.5,258.0,408.5,249.7,135.4,224.3,2699.0,28.2,53.5,54.5,9952.6,20726.3,150.7,199.1,5.0,112.9,241.8,187.6,102.4,104.7,101.5,98.3,100.1,103.9,103.7,103.2,100.0,102.6,103.8,100.5,0.1,2.0,2.7,7.1,7.1,0.5,12.7,11.8,10.4,6.9,11.0,10.8,20.4,24.0,101.9,101.7,310.08,0.27,0.04,98.28,0.06,15007259.96,615677.15,6844761.55,762181.2,0.03
+2013-06-30,3051.7,129.8,409.5,300.7,48.2,287.3,439.0,245.3,135.9,219.5,2860.0,29.4,53.7,56.6,12883.6,22137.4,151.1,197.3,4.8,103.0,246.8,189.3,102.3,103.9,100.3,90.8,103.2,99.1,99.3,104.4,103.0,103.8,104.2,102.3,0.1,2.4,2.9,6.1,6.1,0.9,10.9,11.6,10.7,7.3,10.4,9.7,18.1,22.5,101.1,101.0,322.52,0.25,0.04,124.37,0.06,17722751.86,634535.55,7620005.25,781312.4,0.03
+2013-09-30,2958.4,149.4,343.3,240.0,46.8,323.5,461.2,296.5,122.0,219.3,2680.1,30.0,55.4,57.5,12837.2,20191.8,152.9,202.6,4.7,110.1,313.3,190.4,101.7,103.1,100.4,103.0,114.1,101.0,100.3,103.3,101.3,108.5,103.0,103.7,0.1,2.0,2.7,5.9,5.9,2.8,11.7,11.8,10.4,7.1,11.7,10.5,20.0,21.3,101.2,100.4,333.51,0.25,0.04,110.47,0.06,21135859.36,682799.15,10163721.15,884096.4,0.03
+2013-12-31,3360.0,174.7,466.1,320.0,49.0,318.8,484.1,365.8,276.5,315.2,3316.3,31.2,56.9,60.7,13492.5,22070.5,153.8,209.4,4.7,109.4,364.0,192.3,103.7,102.7,100.7,102.0,103.5,99.6,107.9,100.6,107.4,101.4,107.0,109.4,0.1,2.1,3.0,4.8,4.8,2.6,11.2,11.5,10.4,7.2,10.5,8.2,19.3,21.5,100.5,100.4,351.27,0.24,0.04,145.09,0.06,22030328.76,753596.25,8997647.45,1123733.6,0.03
+2014-03-31,3000.3,132.2,415.0,277.4,47.2,267.4,458.8,264.7,150.2,223.1,2796.1,29.1,53.9,55.1,8524.0,23034.1,170.2,233.3,4.8,107.9,264.4,197.5,107.4,109.4,101.1,114.0,101.7,102.6,102.9,103.5,100.9,103.5,103.1,101.6,0.1,2.3,3.0,6.4,6.4,7.9,11.4,11.4,10.5,7.9,10.5,8.4,14.9,21.5,102.1,101.2,381.67,0.25,0.04,166.11,0.06,19068753.66,815828.75,9393061.15,1238286.5,0.02
+2014-06-30,3170.1,133.0,407.7,297.2,48.8,299.3,466.9,262.6,144.8,224.5,2957.7,30.7,53.2,59.8,11033.3,19681.9,182.7,250.4,5.2,109.8,269.7,202.1,104.1,105.1,100.9,107.3,101.8,103.8,102.6,102.1,102.9,105.2,102.7,101.6,0.1,2.3,3.1,7.1,7.1,0.7,11.4,11.0,10.7,7.2,10.9,9.7,13.6,20.9,102.0,101.3,382.52,0.25,0.04,157.37,0.06,19721550.86,773559.05,9521521.35,1427547.0,0.02
+2014-09-30,3074.8,147.2,346.2,245.6,47.7,337.2,498.5,316.0,127.6,235.1,2788.9,30.9,55.4,59.9,11417.9,19340.6,182.5,242.2,5.0,102.1,343.4,204.1,99.7,101.5,100.6,107.0,101.0,103.3,104.1,102.8,101.7,103.1,102.8,101.8,0.1,2.8,3.4,7.2,7.2,1.4,11.5,11.4,10.1,6.7,10.7,9.2,17.9,20.1,100.4,100.9,380.32,0.24,0.04,144.57,0.06,22769776.26,757296.65,10027824.95,1592141.1,0.02
+2014-12-31,3522.1,176.1,467.7,339.9,51.2,335.3,509.1,394.3,299.8,336.3,3481.3,32.2,56.8,63.2,11478.5,17016.1,181.4,226.6,3.9,76.0,358.7,206.9,100.3,100.9,100.6,78.7,101.3,99.2,97.4,101.2,104.1,104.1,105.7,101.1,0.1,3.3,3.8,7.8,7.8,17.3,11.2,11.2,12.4,7.6,9.7,8.4,16.6,20.8,101.2,101.7,373.28,0.23,0.06,108.52,0.06,25161537.06,287272.15,11044545.05,1769326.9,0.02
+2015-03-31,3060.2,135.5,418.7,276.8,46.0,271.4,469.0,283.6,157.0,227.8,2868.0,29.5,53.3,56.5,7917.9,11725.0,184.6,208.3,2.9,53.9,270.2,209.8,101.3,100.7,100.8,85.3,101.0,96.2,102.2,102.3,100.7,103.7,104.4,100.6,0.1,8.4,3.9,10.0,10.0,14.7,15.7,9.5,19.5,7.1,11.7,9.1,19.6,21.3,101.8,101.0,392.59,0.33,0.05,112.18,0.06,25713283.86,591316.55,10891206.15,1714334.6,0.02
+2015-06-30,3214.1,135.8,411.4,299.6,48.2,321.9,482.5,278.7,144.8,227.0,3024.9,31.5,52.1,59.0,9152.0,12210.0,185.9,205.3,3.5,62.1,265.6,210.7,99.4,99.1,100.7,111.2,101.4,98.2,98.4,102.4,102.5,100.3,100.7,100.9,0.1,8.4,3.9,10.3,10.4,7.6,12.1,9.5,15.5,6.8,12.5,9.2,15.7,18.2,99.2,99.3,357.26,0.44,0.32,46.14,0.06,25802870.06,657638.85,13689096.85,1822801.2,0.02
+2015-09-30,3083.7,151.4,319.1,253.0,46.6,347.7,482.7,328.0,129.7,238.9,2795.3,32.1,54.1,58.8,8577.6,11108.9,216.2,240.9,3.4,50.0,344.8,212.1,102.2,102.0,100.3,89.6,107.1,95.6,98.9,101.8,104.5,98.6,100.4,101.2,0.1,4.7,4.7,6.2,6.1,8.1,10.0,9.9,14.7,6.6,11.6,9.5,17.8,18.2,99.1,98.2,410.0,0.43,0.29,50.54,0.06,25055203.36,952520.25,11179606.35,1701102.7,0.02
+2015-12-31,3561.2,184.1,440.4,328.7,50.5,347.8,501.4,413.1,318.3,351.0,3545.9,31.5,52.6,58.8,7551.7,9782.5,300.2,328.7,4.6,43.4,377.6,231.4,108.1,105.6,100.3,106.7,102.2,95.7,103.1,102.0,96.2,107.6,106.0,103.8,0.2,13.2,11.1,7.4,6.8,36.6,17.2,9.6,16.2,7.6,12.6,6.4,15.1,17.9,99.6,98.3,444.39,0.3,0.04,52.98,0.06,26117137.86,1094862.45,11963387.15,1595414.7,0.02
+2016-03-31,3059.0,138.6,411.7,276.8,45.6,286.9,439.1,294.6,150.8,230.7,2860.1,29.7,50.0,55.0,5371.5,8022.7,356.6,392.6,4.8,34.4,304.3,241.4,104.8,104.6,100.7,113.2,100.7,100.3,104.0,102.6,101.1,101.1,102.7,100.2,0.4,14.9,13.4,9.1,8.5,24.9,4.0,9.2,21.6,8.2,12.9,7.7,18.5,19.1,100.3,99.5,446.26,0.33,0.04,50.51,0.06,26723519.46,913089.65,11898493.75,1552554.3,0.02
+2016-06-30,3223.2,138.4,390.4,300.7,47.6,343.8,466.0,290.0,137.9,231.2,3029.4,31.0,48.4,58.4,6364.8,8217.3,335.6,379.0,5.1,46.0,311.7,246.0,97.7,98.5,100.1,101.6,101.6,102.3,106.4,101.1,102.6,102.6,104.5,99.0,0.4,14.5,13.5,9.3,8.4,14.4,15.5,9.4,17.4,8.4,14.2,7.9,20.9,19.2,99.8,99.0,450.46,0.37,0.03,51.56,0.06,26455285.56,1163709.25,11786904.25,1729624.6,0.02
+2016-09-30,3099.8,164.0,295.7,254.3,47.4,372.3,483.5,337.9,125.5,243.8,2824.9,30.6,50.2,56.7,6841.7,9236.0,341.5,381.1,5.3,45.8,387.1,248.9,99.9,99.4,100.1,120.7,104.6,103.2,104.8,103.0,103.9,103.3,101.8,97.8,0.4,13.1,12.3,10.5,9.3,12.3,18.0,9.8,15.9,7.9,14.8,9.0,22.4,20.4,99.8,99.0,455.6,0.49,0.33,53.09,0.06,26721196.26,1284186.75,11302902.05,701928.7,0.02
+2016-12-31,3681.3,196.7,452.3,343.5,51.1,377.1,506.5,422.3,339.3,363.0,3668.9,32.5,52.2,61.0,7654.4,10009.8,334.9,361.9,5.3,50.1,424.2,253.7,98.5,99.0,100.2,114.0,103.8,110.5,109.2,104.7,104.6,105.4,100.9,94.1,0.5,11.8,12.0,9.6,10.0,11.5,14.6,9.6,15.3,6.8,14.6,7.7,22.0,19.9,99.7,99.5,410.68,0.4,0.03,47.14,0.06,27878091.56,1826890.45,12130778.55,746191.6,0.02
+2017-03-31,3171.3,142.2,436.5,297.2,47.3,307.4,451.6,305.0,153.5,233.9,2963.7,30.4,51.1,53.9,6274.9,10540.2,322.5,343.3,5.5,54.1,328.9,260.3,99.6,99.6,100.3,114.5,101.0,104.2,103.6,104.3,101.6,101.9,102.2,100.9,0.7,10.6,11.3,9.3,8.8,10.9,9.9,9.7,14.0,6.2,13.9,7.8,22.0,19.4,100.1,99.7,462.06,0.53,0.31,57.04,0.06,28567564.96,1536978.85,15970284.55,680585.4,0.02
+2017-06-30,3380.5,142.6,444.5,319.9,50.7,360.7,475.6,302.6,142.7,237.7,3174.3,31.2,50.4,56.7,7875.8,11946.3,314.7,345.9,5.5,50.2,328.8,264.4,100.3,99.8,99.9,106.8,100.9,104.3,102.7,100.9,100.6,101.4,101.5,100.9,1.0,9.8,9.2,9.2,8.3,10.0,15.9,9.7,13.7,6.1,14.2,7.6,21.6,19.7,100.3,99.5,470.71,0.52,0.3,59.81,0.06,30818177.06,1312502.95,10515776.15,744223.7,0.02
+2017-09-30,3228.9,164.1,342.4,265.0,50.0,370.3,503.6,358.6,130.7,251.3,2940.6,31.3,52.2,55.6,7882.8,11254.3,332.4,390.3,5.6,51.7,421.1,266.3,101.2,99.9,99.9,123.5,103.2,102.8,103.4,105.3,101.9,101.5,102.6,101.3,1.2,9.2,9.0,8.9,9.0,9.4,13.5,9.7,13.4,5.3,13.8,8.0,22.0,19.8,100.1,99.1,421.3,0.5,0.3,73.82,0.06,34108887.56,1440663.95,13902272.45,784476.0,0.03
+2017-12-31,3821.6,209.4,474.6,365.4,54.2,380.8,525.7,443.7,351.1,367.8,3801.0,33.1,53.5,60.2,8539.7,13560.3,334.4,393.7,5.7,61.5,503.4,272.1,99.9,99.3,100.1,105.9,109.1,109.8,104.8,105.1,103.5,110.3,107.9,107.9,1.2,9.3,9.2,8.9,8.8,9.3,14.6,9.3,13.1,5.2,14.4,5.5,21.5,20.6,100.6,100.1,231.49,0.38,0.03,25.49,0.06,38939710.26,1649264.65,15346462.45,940450.5,0.03
+2018-03-31,3307.8,147.0,459.0,314.8,49.2,325.4,478.9,318.8,163.0,239.2,3099.7,31.1,53.4,54.9,7575.4,13669.9,323.2,397.3,5.7,67.0,356.3,277.6,100.6,99.7,100.0,112.2,101.0,104.7,103.0,102.2,100.9,101.9,101.4,101.3,1.4,8.9,8.6,8.9,8.9,8.8,7.9,9.6,12.8,5.4,13.8,5.7,23.4,20.7,101.2,100.8,229.18,0.38,0.03,25.51,0.06,39247807.06,1873724.05,13284024.05,881350.8,0.03
+2018-06-30,3519.5,149.0,470.8,332.8,53.8,367.8,502.5,318.2,151.0,241.2,3298.7,32.4,52.3,57.9,8478.8,14691.7,329.8,393.5,5.3,74.5,371.4,280.9,101.0,100.3,100.0,99.0,102.4,107.8,104.0,103.8,102.3,102.5,103.4,101.3,1.7,8.3,8.4,8.4,8.5,8.3,8.9,9.8,12.0,5.4,12.8,5.1,21.0,21.1,101.9,100.8,237.64,0.42,0.03,25.08,0.06,43997235.26,1982946.35,14813646.65,997580.1,0.04
+2018-09-30,3352.7,161.6,354.0,278.1,50.8,390.4,544.4,373.1,131.3,261.7,3052.5,33.6,53.9,57.3,9083.1,15366.4,356.0,413.8,5.5,75.5,444.7,282.3,100.3,100.4,100.1,91.0,100.3,105.8,103.5,100.8,102.4,102.4,103.4,100.4,1.9,8.4,8.8,9.1,8.4,8.4,14.1,8.7,12.1,5.4,12.8,4.9,20.9,19.8,101.6,100.7,471.22,0.53,0.37,67.48,0.06,48800906.66,2724046.05,15331709.25,1121266.3,0.04
+2018-12-31,3976.5,225.3,491.2,377.2,52.9,400.2,574.3,463.8,364.0,380.8,3952.2,35.0,57.0,61.4,9109.8,16098.3,369.8,422.1,5.6,67.4,554.6,286.5,100.6,100.7,100.1,104.9,106.7,103.9,104.0,103.0,104.4,106.0,105.0,105.4,2.2,8.8,8.7,8.7,8.5,8.3,11.3,8.2,12.4,5.2,11.4,6.1,21.1,19.3,101.4,101.8,491.53,0.39,0.04,63.45,0.06,53885717.16,1115202.55,17667145.65,1197715.2,0.04
+2019-03-31,3430.9,151.3,477.5,319.1,48.6,352.4,510.6,331.1,167.2,243.2,3214.8,33.3,55.9,57.8,7258.6,14364.5,377.7,429.1,5.7,63.3,384.2,291.1,101.0,100.9,100.2,107.0,100.6,101.0,100.3,99.7,101.8,101.5,100.8,100.5,2.4,8.8,8.8,8.8,8.7,8.3,11.0,8.1,12.2,5.6,13.0,5.4,20.9,20.0,102.3,101.1,465.88,0.39,0.05,83.62,0.06,52226897.36,4065848.05,16285468.65,1114377.0,0.05
+2019-06-30,3674.1,153.1,465.8,346.9,56.0,413.5,539.7,336.1,157.3,247.1,3443.2,35.1,53.9,63.2,7258.6,14364.5,380.6,427.5,5.9,68.3,400.8,295.2,101.4,101.3,100.0,93.0,100.6,99.7,101.1,101.1,103.0,101.7,101.2,100.8,2.4,8.8,8.7,8.7,8.6,8.2,12.0,8.1,11.8,5.0,12.0,6.0,19.9,20.4,101.5,100.5,487.39,0.37,0.05,80.59,0.06,61132600.76,4276646.55,18400683.95,1268472.7,0.05
+2019-09-30,3518.9,148.5,371.9,287.9,52.8,457.2,582.6,392.8,136.2,267.0,3209.6,35.4,56.3,64.3,7258.6,14364.5,385.8,429.2,6.0,61.9,465.8,297.3,101.1,102.0,99.9,94.8,98.1,101.0,100.7,101.0,104.3,101.8,101.3,100.6,2.2,9.8,10.0,9.2,9.2,8.5,7.0,8.1,11.8,4.5,12.4,5.2,20.4,21.3,102.1,101.8,528.02,0.33,0.06,83.55,0.06,65828104.76,5641360.45,18106110.55,4145285.1,0.05
+2019-12-31,4170.2,225.7,505.0,417.2,49.4,447.3,604.1,485.2,380.6,385.8,4145.8,36.8,58.5,67.5,7258.6,14364.5,386.9,428.2,6.1,62.7,605.1,302.0,102.6,101.8,100.1,108.7,100.1,100.8,103.0,98.3,102.9,101.4,101.4,102.0,1.6,9.9,9.3,9.6,9.5,8.8,2.8,7.5,11.9,4.6,13.1,4.7,17.4,19.6,101.9,100.4,403.74,0.34,0.06,56.19,0.06,70627071.46,5241812.95,19382747.45,1012652.3,0.05
+2020-03-31,3509.2,153.4,495.9,343.4,47.5,389.3,510.1,323.2,183.0,241.7,3299.5,36.1,57.1,64.9,7258.6,14364.5,389.6,429.9,5.9,50.5,430.1,308.7,101.7,101.9,100.4,94.2,100.3,101.0,101.8,99.5,102.2,100.0,99.5,101.9,1.3,12.2,10.7,10.7,10.6,10.0,15.7,8.4,12.0,4.2,13.7,5.7,21.7,20.8,101.4,100.2,415.71,0.33,0.06,59.38,0.06,67784541.66,5168664.05,19620102.15,890662.3,0.05
+2020-06-30,3446.9,154.3,457.6,347.6,58.5,453.1,419.7,239.7,175.5,222.3,3237.0,35.8,52.8,67.2,8758.3,11688.7,418.1,459.9,5.8,31.4,386.0,315.5,100.5,101.5,96.7,105.4,100.2,99.6,100.1,101.2,102.3,94.6,93.7,102.1,0.1,10.0,10.8,10.6,10.6,8.8,5.0,7.8,11.4,4.2,11.9,6.9,23.8,19.4,102.7,101.4,403.0,0.39,0.05,51.85,0.06,66900692.76,5374901.95,19052286.55,132100.1,0.05
+2020-09-30,3333.6,162.6,317.4,284.5,52.0,494.4,531.9,306.2,132.2,294.0,3041.1,35.6,56.4,64.2,10425.9,9328.2,417.9,488.2,5.7,42.7,522.1,318.3,101.1,103.3,99.6,103.5,102.1,97.0,99.8,99.6,102.1,97.6,94.0,99.5,0.1,9.5,10.2,10.3,10.3,8.6,7.1,7.6,11.7,3.1,13.1,5.1,21.2,20.6,103.7,103.2,588.7,0.56,0.38,73.73,0.06,70349533.76,6146130.65,20662672.25,897458.1,0.05
+2020-12-31,4132.4,240.4,457.4,434.8,46.3,507.1,677.9,312.3,428.7,372.6,4109.4,39.1,59.1,71.9,9765.6,11333.1,426.2,507.8,5.6,44.5,601.2,324.0,101.8,104.5,100.4,110.2,102.1,97.3,101.3,98.5,103.3,103.6,87.2,105.5,0.1,9.5,10.0,9.8,10.0,8.7,1.8,7.5,11.5,4.4,12.1,5.5,18.1,18.2,103.7,104.4,607.39,0.46,0.05,70.42,0.05,75289906.56,5253623.65,22925783.65,1199838.2,0.04
+2021-03-31,3464.5,156.6,457.9,366.5,49.5,437.2,493.3,265.1,199.7,237.1,3262.8,36.5,56.9,69.8,7605.8,11455.4,419.7,506.4,5.6,60.6,463.7,330.8,104.5,109.7,101.2,116.3,100.4,97.8,101.6,101.0,102.6,99.2,95.1,101.8,0.1,9.1,9.1,10.2,10.0,8.7,10.8,8.0,11.3,4.9,12.7,5.7,19.1,20.1,106.0,103.6,631.71,0.4,0.05,72.03,0.05,67245860.84,4222873.49,20497372.43,1469224.27,0.04
+2021-06-30,3684.5,158.5,460.5,357.4,61.6,498.8,508.3,266.4,215.0,226.9,3451.3,38.0,58.4,74.3,9884.9,15480.3,428.4,515.9,5.8,68.6,442.2,338.5,103.5,105.2,100.1,107.3,100.6,100.2,100.7,101.5,102.4,104.2,102.4,104.2,0.1,8.7,9.2,10.1,10.1,8.5,8.5,8.3,11.3,5.0,12.8,3.9,19.3,19.0,107.0,104.4,728.89,0.54,0.4,61.24,0.05,72410915.24,4335545.66,20905741.68,1489553.73,0.04
+2021-09-30,3556.8,158.6,333.5,300.0,55.4,520.2,584.7,332.3,167.6,297.0,3224.5,37.5,59.7,70.5,10994.8,16201.8,425.7,502.0,5.8,73.0,573.3,345.6,102.9,103.2,100.1,101.4,99.4,101.0,101.1,101.6,101.3,102.4,102.3,103.6,0.1,8.9,9.4,10.1,9.6,8.8,12.1,8.0,11.4,3.8,13.0,4.5,18.9,19.2,105.1,103.4,822.04,0.55,0.44,62.84,0.05,77689778.61,4449455.98,21318598.51,1510106.6,0.04
+2021-12-31,4338.7,216.6,496.9,442.4,48.4,526.7,638.1,425.4,443.0,392.1,4314.7,40.4,62.6,78.3,11133.9,17115.8,429.8,491.7,5.9,79.6,712.7,351.8,103.8,103.9,100.8,108.5,96.7,102.3,100.5,101.0,101.0,98.2,109.6,101.4,0.1,9.0,9.6,10.3,9.8,9.6,12.5,8.5,11.6,4.4,12.8,4.7,15.6,19.1,105.7,104.7,918.2,0.39,0.05,63.95,0.05,74562995.83,4563366.3,21731455.33,1530659.47,0.05
+2022-03-31,3588.5,158.0,440.4,387.0,48.7,470.8,528.2,287.3,229.1,232.3,3368.3,39.1,60.5,78.6,9636.0,19114.6,455.1,510.8,5.3,99.0,548.8,362.7,105.7,110.6,100.6,91.04,100.2,99.0,101.4,99.6,101.7,101.6,101.7,102.9,0.1,13.1,13.2,10.9,9.9,11.9,13.9,8.7,13.0,4.5,13.2,4.4,14.9,20.6,108.0,106.5,904.24,0.6,0.48,69.12,0.06,73590762.04,4894401.58,23450458.36,1661117.26,0.05
+2022-06-30,3733.2,158.7,431.1,372.3,60.9,542.6,526.5,272.4,209.2,217.7,3486.0,39.0,58.4,80.9,12107.7,23244.6,442.1,471.9,6.8,112.7,544.8,385.5,106.1,107.5,100.5,79.95,100.0,98.3,101.0,99.7,102.2,100.8,100.5,99.5,0.8,13.0,13.4,11.3,10.1,13.9,10.3,8.3,15.5,5.3,15.6,5.2,13.2,19.4,106.5,102.0,1010.02,0.43,0.05,70.34,0.06,77384487.14,5019702.93,23904600.87,1683725.41,0.05
+2022-09-30,3663.6,185.2,349.2,302.5,54.7,504.0,585.8,337.9,200.8,312.8,3311.1,37.9,58.8,74.6,13235.4,21820.0,475.4,479.4,8.0,99.2,694.8,401.9,101.8,102.1,100.5,114.7,103.9,100.9,100.2,99.7,99.2,100.0,100.4,103.2,2.2,13.6,13.8,10.2,9.5,13.9,9.9,8.5,16.2,4.1,16.1,4.6,15.4,18.5,104.3,101.4,1111.02,0.47,0.06,77.37,0.06,85122935.85,5521673.23,26295060.95,1852097.95,0.05
+2022-12-31,4537.4,244.7,495.7,441.3,47.5,633.4,675.3,430.5,458.7,393.0,4510.9,35.3,58.7,80.5,14734.5,20659.3,468.0,476.8,7.5,88.4,794.2,420.7,102.0,103.1,100.1,106.1,103.9,99.9,99.9,99.6,105.2,101.6,100.4,101.5,3.7,15.7,14.8,11.0,10.2,15.5,13.7,9.2,18.1,5.3,18.6,6.9,13.6,17.6,100.9,101.6,1222.12,0.52,0.06,85.11,0.07,93635229.43,6073840.55,28924567.05,2037307.75,0.06
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `AFR-0.2.2/load/macroKZ_dataset.html` & `AFR-0.2.7/AFR/load/macroKZ_dataset.html`

 * *Files 0% similar despite different names*

#### Comparing `AFR-0.2.2/load/macroKZ_dataset.html` & `AFR-0.2.7/AFR/load/macroKZ_dataset.html`

```diff
@@ -360,15 +360,15 @@
   <body>
     <div class="document" id="macrokz-dataset">
       <h1 class="title">macroKZ dataset</h1>
       <p>
         The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the
         <a class="reference external" href="https://stat.gov.kz/">Bureau of National Statistics</a>
         .
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 The
         <em>macroKZ</em>
         dataset will be updated periodically as the official statistical information is released.
       </p>
       <p>
         <strong>Dataset contains following data</strong>
         :
```

### Comparing `AFR-0.2.2/load/macroKZ_dataset.rst` & `AFR-0.2.7/AFR/load/macroKZ_dataset.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 macroKZ dataset
 ===============
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the `Bureau of National Statistics <https://stat.gov.kz/>`_.
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
 - **real_gdp** Real GDP
 - **GDD_Agr_R** Real gross value added Agriculture
 - **GDD_Min_R** Real gross value added Mining
```

