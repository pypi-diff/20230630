# Comparing `tmp/dbt_snapshot_analysis-0.2.7.tar.gz` & `tmp/dbt_snapshot_analysis-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_snapshot_analysis-0.2.7.tar", last modified: Wed Jun 28 09:52:33 2023, max compression
+gzip compressed data, was "dbt_snapshot_analysis-0.2.8.tar", last modified: Fri Jun 30 10:42:35 2023, max compression
```

## Comparing `dbt_snapshot_analysis-0.2.7.tar` & `dbt_snapshot_analysis-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-28 09:52:33.380275 dbt_snapshot_analysis-0.2.7/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-28 09:52:33.380035 dbt_snapshot_analysis-0.2.7/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      936 2023-06-26 08:26:25.000000 dbt_snapshot_analysis-0.2.7/README.md
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-28 09:52:33.378561 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/
--rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/__init__.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/data_validation.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)    10834 2023-06-28 09:51:13.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/dbt_snapshot_analysis.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)     2025 2023-06-26 15:24:40.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/snapshot_utils.py
--rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/streamlit_entry_point.py
-drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-28 09:52:33.379639 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/
--rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/PKG-INFO
--rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/entry_points.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/requires.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-28 09:52:33.000000 dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/top_level.txt
--rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-28 09:52:33.380353 dbt_snapshot_analysis-0.2.7/setup.cfg
--rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-28 09:52:30.000000 dbt_snapshot_analysis-0.2.7/setup.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.122973 dbt_snapshot_analysis-0.2.8/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-30 10:42:35.122832 dbt_snapshot_analysis-0.2.8/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      936 2023-06-26 08:26:25.000000 dbt_snapshot_analysis-0.2.8/README.md
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.121715 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        0 2023-06-23 13:17:16.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/__init__.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      873 2023-06-21 15:26:08.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/data_validation.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)    14423 2023-06-30 10:41:14.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/dbt_snapshot_analysis.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     2025 2023-06-26 15:24:40.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/snapshot_utils.py
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      372 2023-06-23 13:21:59.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/streamlit_entry_point.py
+drwxr-xr-x   0 sammyteillet   (501) staff       (20)        0 2023-06-30 10:42:35.122606 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/
+-rw-r--r--   0 sammyteillet   (501) staff       (20)     1355 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      499 2023-06-30 10:42:35.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)        1 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       91 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       24 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/requires.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       22 2023-06-30 10:42:34.000000 dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/top_level.txt
+-rw-r--r--   0 sammyteillet   (501) staff       (20)       38 2023-06-30 10:42:35.123030 dbt_snapshot_analysis-0.2.8/setup.cfg
+-rw-r--r--   0 sammyteillet   (501) staff       (20)      847 2023-06-30 10:41:39.000000 dbt_snapshot_analysis-0.2.8/setup.py
```

### Comparing `dbt_snapshot_analysis-0.2.7/PKG-INFO` & `dbt_snapshot_analysis-0.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_snapshot_analysis
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zjgnurib_/tmpfi9jmrc5_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_zjgnurib_/tmpfi9jmrc5_TarContainer/0/1", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.7 Summary: A
+Metadata-Version: 2.1 Name: dbt_snapshot_analysis Version: 0.2.8 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.7/README.md` & `dbt_snapshot_analysis-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/data_validation.py` & `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/data_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/dbt_snapshot_analysis.py` & `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/dbt_snapshot_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas as pd
 import streamlit as st
 from typing import List
 from datetime import datetime
 import plotly.express as px
 import plotly.graph_objects as go
 import numpy as np
+import base64
 
 
 from snapshot_utils import get_metric_by_month, get_snapshot_as_of_date, determine_type
 
 
 @st.cache_data()
 def compute_all_metric_day_by_day(local_df: pd.DataFrame, date_range: List[str]):
@@ -104,110 +105,111 @@
         ]
     else:
         st.write("Please select a valid metric column and a date column")
     return local_df
 
 
 def run():
-    firstCol1, firstCol2 = st.columns(2)
+    st.sidebar.write("# dbt Snapshot analysis")
+    st.sidebar.write(
+        "*Changes of a metric’s historical value harms data consumers’ trust and is very difficult to solve for data teams.*"
+    )
+    st.sidebar.write(
+        "***Upload a dbt snapshot of a table on which you build a key metric and see how you compare!***"
+    )
+    st.sidebar.write(
+        "⭐️ [Star us on Github](https://github.com/data-drift/data-drift) ⭐️"
+    )
+    st.write("# 👋 Welcome")
+    st.write("### Upload a dbt snapshot to get started")
+    uploaded_file = st.file_uploader("Select a csv file")
     df = pd.DataFrame()
-    with firstCol1:
-        uploaded_file = st.file_uploader("Choose a file")
-
-    with firstCol2:
-        if uploaded_file is not None:
-            df = parse_csv_file(uploaded_file)
-            unique_id_column = st.selectbox("Select unique id column", df.columns)
+    if uploaded_file is None:
+        st.write("### Analyse the stability of your key metrics")
+        st.write(
+            "Changes of a metric’s historical value harms data consumers’ trust and is very difficult to solve for data teams."
+        )
+        st.write(
+            "**Upload a dbt snapshot of a table on which you build a key metric and see how you compare!**"
+        )
+        file_ = open("dbt-snapshot-analysis.gif", "rb")
+        contents = file_.read()
+        data_url = base64.b64encode(contents).decode("utf-8")
+        file_.close()
+        st.markdown(
+            f'<img src="data:image/gif;base64,{data_url}" alt="cat gif">',
+            unsafe_allow_html=True,
+        )
+    else:
+        df = parse_csv_file(uploaded_file)
+        unique_id_column = st.selectbox("Select unique id column", df.columns)
 
     if not df.empty:
-        tab1, tab2, tab3 = st.tabs(["Version", "Lifespan", "Data"])
-        with tab1:
-            st.markdown("## Distribution of versions per ID")
-            st.header("Version distribution")
-            unique_ids = df.groupby(unique_id_column).size()
-            print(f"Number of unique ids: {unique_ids.shape[0]}")
-            versions_per_id = (
-                df.groupby(unique_id_column).size().reset_index(name="version per id")
-            )
-            versions_count = (
-                versions_per_id["version per id"].value_counts().sort_index()
-            )
-
-            st.bar_chart(versions_count)
-
-        with tab2:
-            lifespandf = df.copy()
-            lifespandf["lifespan"] = (
-                lifespandf["dbt_valid_to"] - lifespandf["dbt_valid_from"]
-            )
-            print(lifespandf["lifespan"].describe())
-            lifespandf["lifespan_numeric"] = pd.to_numeric(
-                lifespandf["lifespan"], errors="coerce"
-            )
-            lifespandf["lifespan (days)"] = lifespandf["lifespan"].dt.days
-            print(lifespandf["lifespan (days)"].describe())
-
-            all_versions = lifespandf["lifespan (days)"]
-            dead_versions = lifespandf[lifespandf["is_current_version"] == False][
-                "lifespan (days)"
-            ]
-
-            lifespan_df_with_alive = pd.DataFrame(
-                dict(
-                    series=np.concatenate(
-                        (
-                            ["lifespan all rows (days)"] * len(all_versions),
-                            ["lifespan without active (days)"] * len(dead_versions),
-                        )
-                    ),
-                    data=np.concatenate((all_versions, dead_versions)),
-                )
-            )
+        unique_ids = df.groupby(unique_id_column).size()
+        versions_per_id = (
+            df.groupby(unique_id_column).size().reset_index(name="version per id")
+        )
+        versions_count = versions_per_id["version per id"].value_counts().sort_index()
+        lifespandf = df.copy()
+        lifespandf["lifespan"] = (
+            lifespandf["dbt_valid_to"] - lifespandf["dbt_valid_from"]
+        )
+        print(lifespandf["lifespan"].describe())
+        lifespandf["lifespan_numeric"] = pd.to_numeric(
+            lifespandf["lifespan"], errors="coerce"
+        )
+        lifespandf["lifespan (days)"] = lifespandf["lifespan"].dt.days
+        print(lifespandf["lifespan (days)"].describe())
 
-            fig = px.histogram(
-                lifespan_df_with_alive,
-                x="data",
-                color="series",
-                barmode="overlay",
-                nbins=50,
-            )
-
-            st.plotly_chart(fig, use_container_width=True)
-
-        with tab3:
-            st.header("Dataframe")
-            st.write(df)
+        all_versions = lifespandf["lifespan (days)"]
+        dead_versions = lifespandf[lifespandf["is_current_version"] == False][
+            "lifespan (days)"
+        ]
 
+        lifespan_df_with_alive = pd.DataFrame(
+            dict(
+                series=np.concatenate(
+                    (
+                        ["lifespan all rows (days)"] * len(all_versions),
+                        ["lifespan without active (days)"] * len(dead_versions),
+                    )
+                ),
+                data=np.concatenate((all_versions, dead_versions)),
+            )
+        )
         min_date = df["dbt_valid_from"].min()
         max_date = df["dbt_valid_from"].max()
         date_range = pd.date_range(start=min_date, end=max_date)
         date_range_str = date_range.strftime("%Y-%m-%d").tolist()
 
         metric_distribution_df = df.copy()
+        st.write("### Compute the metric you want to analyse")
 
         col1, col2, col3 = st.columns(3)
 
         with col1:
-            is_metric_or_count = st.radio("Metric", ["Count", "Sum"])
+            is_metric_or_count = st.radio(
+                "Select the aggregation method", ["Count", "Sum"]
+            )
 
         with col2:
             date_column = st.selectbox(
-                "Select metric date column", metric_distribution_df.columns
+                "Select the reference date", metric_distribution_df.columns
             )
             is_date_column_valid = is_date_column(metric_distribution_df, date_column)
             if not is_date_column_valid:
                 st.warning(
                     "Please select a valid date column, it should be supported by pandas.to_datetime."
                 )
 
         with col3:
             is_numeric_column_valid = False
             if is_metric_or_count == "Sum":
                 metric_column = st.selectbox(
-                    "Select metric column to sum", metric_distribution_df.columns
+                    "Select the column to sum", metric_distribution_df.columns
                 )
                 is_numeric_column_valid = is_numeric_column(
                     metric_distribution_df, metric_column
                 )
                 if not is_numeric_column_valid:
                     st.warning(
                         "Please select a valid metric column, it should be a numeric column."
@@ -236,69 +238,122 @@
                 .transform("first")
             )
 
             all_results["relative_value"] = (
                 all_results["metric_value"] / all_results["latest_value"]
             )
 
-            all_monthly_volatility = (
-                all_results[all_results["metric_value"] > 0]
-                .groupby("metric_date")["relative_value"]
-                .std()
-            )
-
-            all_monthly_volatility_from_latest_value = (
-                all_results[all_results["metric_value"] > 0]
-                .groupby("metric_date")["relative_value"]
-                .apply(lambda x: ((x - 1) ** 2).mean() ** 0.5)
-            )
+            volatility_filtered_df = all_results[all_results["metric_value"] > 0]
+            volatility_grouped_df = volatility_filtered_df.groupby("metric_date")[
+                "relative_value"
+            ].apply(lambda x: ((x - 1) ** 2).mean() ** 0.5)
+            all_monthly_volatility_from_latest_value = pd.DataFrame(
+                volatility_grouped_df
+            ).rename(columns={"relative_value": "volatility"})
 
             print("all_monthly_volatility", all_monthly_volatility_from_latest_value)
 
-            grouped_df = all_results.groupby("metric_date")
+            volatility_grouped_df = all_results.groupby("metric_date")
 
             st.set_option("deprecation.showPyplotGlobalUse", False)
             fig = go.Figure()
 
-            for metric_name, group in grouped_df:
+            for metric_name, group in volatility_grouped_df:
                 fig.add_trace(
                     go.Scatter(
                         x=group["computation_day"],
                         y=group["relative_value"],
                         name=metric_name,
                     )
                 )
 
             fig.update_layout(
-                title="Metric Value Over Time",
                 xaxis_title="Computation Day",
-                yaxis_title="Metric Value",
+                yaxis_title="Normalized Value",
                 showlegend=True,
             )
-            st.plotly_chart(fig)
-
-            st.subheader("Monthly volatility")
-
-            st.dataframe(all_monthly_volatility_from_latest_value)
 
-            st.header("Summary")
+            st.divider()
+            st.write("### 💎 Summary")
             summary1, summary2 = st.columns(2)
             with summary1:
-                st.subheader("Mean lifespan of a row")
-                st.write("The average time it takes for an error to be corrected.")
+                st.write("#### Row lifespan")
                 meanLifespan = dead_versions.mean()
-                st.write(f"{meanLifespan:.2f} days")
+                st.metric("Mean row lifespan", f"{meanLifespan:.2f} days")
+                st.info(
+                    "The lifespan is the number of days between two updates of a given row",
+                    icon="💡",
+                )
 
             with summary2:
-                st.subheader("Volatility of the metric")
+                st.write("#### Metric volatility")
+                meanVolatility = all_monthly_volatility_from_latest_value.mean().mean()
+                st.metric(
+                    "Average volatility (between 0 and 1)", f"{meanVolatility:.3f}"
+                )
+                st.info(
+                    "The volatility shows the delta between computed value at time T and latest value",
+                    icon="💡",
+                )
+
+            st.divider()
+            st.write("### 🔎 Deep dive")
+            st.write(
+                "Navigate through the tabs below to get more insights from your dbt snapshot."
+            )
+            volatilityTab, lifespanTab, versionTab, dataTab = st.tabs(
+                ["📊 Volatility", "⏱ Lifespan", "🗂 Version", "💿 Raw data"]
+            )
+            with volatilityTab:
+                st.write("#### Metric volatility")
+                st.write("##### Monthly volatility")
+                st.plotly_chart(
+                    px.line(all_monthly_volatility_from_latest_value)
+                    .update_yaxes(range=[0, 1], title_text="Volatility")
+                    .update_layout(showlegend=False)
+                )
+                volatility_expander = st.expander("💡 Learn more about volatility")
+                volatility_expander.write(
+                    "It shows how much your metric drifts. We compute the root mean square (RMS) of the difference between the computed value at time T and the latest computed value. It's ike a standard deviation but compared to the latest value instead of the mean. The closer to 0, the less your metric has drifted, the better."
+                )
+                st.write("##### Metric cohorts")
+                st.plotly_chart(fig)
+
+                normalized_value_expender = st.expander(
+                    "💡 Learn more about normalized value"
+                )
+                normalized_value_expender.write(
+                    "It shows how long your metric takes to stabilize to its current value. The normalized value is the value at time T divided by the latest known value. The time series of the normalized value converges to 1, the faster it stays there, the better."
+                )
+
+            with lifespanTab:
+                st.write("#### Row lifespan")
+                lifespan_fig = px.histogram(
+                    lifespan_df_with_alive,
+                    color="series",
+                    barmode="overlay",
+                    nbins=50,
+                )
+                st.plotly_chart(lifespan_fig, use_container_width=True)
+                volatility_expander = st.expander("💡 Learn more about lifespan")
+                volatility_expander.write("The lifespan is the number of days between two updates of a given row. For Lifespan without active, we exclude row that have never been updated (still valid).")
+
+            with versionTab:
+                st.write("#### Version distribution")
+                print(f"Number of unique ids: {unique_ids.shape[0]}")
+                st.bar_chart(versions_count)
+                volatility_expander = st.expander("💡 Learn more about version")
+                volatility_expander.write("A version represents a row for a given unique id. When an id has never been updated it's 1, the current version is the only version.")
+
+            with dataTab:
+                st.write("#### Raw data")
                 st.write(
-                    "Between 0 and 1. Represents the difference between the displayed value at time T and the latest value."
+                    "The underlying raw data used to generate metrics and insights."
                 )
-                meanVolatility = all_monthly_volatility_from_latest_value.mean()
-                st.write(f"{meanVolatility:.4f}")
+                st.write(df)
 
 
 def main():
     run()
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis/snapshot_utils.py` & `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_snapshot_analysis-0.2.7/dbt_snapshot_analysis.egg-info/PKG-INFO` & `dbt_snapshot_analysis-0.2.8/dbt_snapshot_analysis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snapshot-analysis
-Version: 0.2.7
+Version: 0.2.8
 Summary: A package for analyzing snapshots
 Home-page: https://github.com/data-drift/dbt-snapshot-analytics
 Author: Sammy Teillet
 Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_zjgnurib_/tmpfi9jmrc5_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

 * *File "/tmp/diffoscope_zjgnurib_/tmpfi9jmrc5_TarContainer/0/10", line 21, column 2: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.7 Summary: A
+Metadata-Version: 2.1 Name: dbt-snapshot-analysis Version: 0.2.8 Summary: A
 package for analyzing snapshots Home-page: https://github.com/data-drift/dbt-
 snapshot-analytics Author: Sammy Teillet Author-email: sammy.teillet@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
                                [DataDrift_logo]
                        ***** A Changelog for Data *****
```

### Comparing `dbt_snapshot_analysis-0.2.7/setup.py` & `dbt_snapshot_analysis-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="dbt_snapshot_analysis",
-    version="0.2.7",
+    version="0.2.8",
     packages=find_packages(),
     py_modules=["dbt_snapshot_analysis"],
     install_requires=["pandas", "plotly", "streamlit"],
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
```

