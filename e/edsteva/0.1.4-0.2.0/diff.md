# Comparing `tmp/edsteva-0.1.4.tar.gz` & `tmp/edsteva-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edsteva-0.1.4.tar", max compression
+gzip compressed data, was "edsteva-0.2.0.tar", max compression
```

## Comparing `edsteva-0.1.4.tar` & `edsteva-0.2.0.tar`

### file list

```diff
@@ -1,58 +1,176 @@
--rw-r--r--   0        0        0     1485 2023-02-02 17:28:49.364642 edsteva-0.1.4/LICENSE
--rw-r--r--   0        0        0     2822 2023-02-02 17:28:49.364642 edsteva-0.1.4/README.md
--rw-r--r--   0        0        0     2987 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/__init__.py
--rw-r--r--   0        0        0      138 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/__init__.py
--rw-r--r--   0        0        0     2351 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/files.py
--rw-r--r--   0        0        0    11759 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/hive.py
--rw-r--r--   0        0        0     6209 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/i2b2_mapping.py
--rw-r--r--   0        0        0     2957 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/postgres.py
--rw-r--r--   0        0        0    11526 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/settings.py
--rw-r--r--   0        0        0       37 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/synthetic/__init__.py
--rw-r--r--   0        0        0     1051 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/synthetic/care_site.py
--rw-r--r--   0        0        0    17699 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/synthetic/synthetic.py
--rw-r--r--   0        0        0      245 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/synthetic/utils.py
--rw-r--r--   0        0        0     2522 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/io/synthetic/visit.py
--rw-r--r--   0        0        0      166 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/metrics/__init__.py
--rw-r--r--   0        0        0     2169 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/metrics/error.py
--rw-r--r--   0        0        0     2558 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/metrics/error_after_t0.py
--rw-r--r--   0        0        0     2718 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/metrics/error_between_t0_t1.py
--rw-r--r--   0        0        0       42 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/__init__.py
--rw-r--r--   0        0        0    11366 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/base.py
--rw-r--r--   0        0        0       83 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/rectangle_function/__init__.py
--rw-r--r--   0        0        0       82 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/rectangle_function/algos/__init__.py
--rw-r--r--   0        0        0     3284 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/rectangle_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     5355 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/rectangle_function/rectangle_function.py
--rw-r--r--   0        0        0       68 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/step_function/__init__.py
--rw-r--r--   0        0        0      193 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/step_function/algos/__init__.py
--rw-r--r--   0        0        0     2625 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/step_function/algos/loss_minimization.py
--rw-r--r--   0        0        0     2528 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/step_function/algos/quantile.py
--rw-r--r--   0        0        0     5038 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/models/step_function/step_function.py
--rw-r--r--   0        0        0      180 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/__init__.py
--rw-r--r--   0        0        0    14339 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/base.py
--rw-r--r--   0        0        0     9841 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/condition.py
--rw-r--r--   0        0        0     8593 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/note.py
--rw-r--r--   0        0        0    33129 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/utils.py
--rw-r--r--   0        0        0     6713 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/probes/visit.py
--rw-r--r--   0        0        0        0 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/utils/__init__.py
--rw-r--r--   0        0        0     3025 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/utils/checks.py
--rw-r--r--   0        0        0     1488 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/utils/framework.py
--rw-r--r--   0        0        0      176 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/utils/loss_functions.py
--rw-r--r--   0        0        0      344 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/utils/typing.py
--rw-r--r--   0        0        0       52 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/__init__.py
--rw-r--r--   0        0        0      227 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/__init__.py
--rw-r--r--   0        0        0    16627 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/estimates_dashboard.py
--rw-r--r--   0        0        0        0 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/predictor_dashboard/__init__.py
--rw-r--r--   0        0        0     8437 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/predictor_dashboard/fitted_probe.py
--rw-r--r--   0        0        0     7309 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/predictor_dashboard/probe.py
--rw-r--r--   0        0        0     5434 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/dashboards/predictor_dashboard/wrapper.py
--rw-r--r--   0        0        0      204 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/__init__.py
--rw-r--r--   0        0        0     5373 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/estimates_densities.py
--rw-r--r--   0        0        0    10727 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/normalized_probe.py
--rw-r--r--   0        0        0        0 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/plot_probe/__init__.py
--rw-r--r--   0        0        0     3502 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/plot_probe/fitted_probe.py
--rw-r--r--   0        0        0     2565 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/plot_probe/probe.py
--rw-r--r--   0        0        0     4628 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/plots/plot_probe/wrapper.py
--rw-r--r--   0        0        0     3943 2023-02-02 17:28:49.392642 edsteva-0.1.4/edsteva/viz/utils.py
--rw-r--r--   0        0        0     2943 2023-02-02 17:28:49.396642 edsteva-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4293 1970-01-01 00:00:00.000000 edsteva-0.1.4/setup.py
--rw-r--r--   0        0        0     4320 1970-01-01 00:00:00.000000 edsteva-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-06-30 07:53:41.112356 edsteva-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2822 2023-06-30 07:53:41.112356 edsteva-0.2.0/README.md
+-rw-r--r--   0        0        0     3063 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/__init__.py
+-rw-r--r--   0        0        0      138 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/__init__.py
+-rw-r--r--   0        0        0     2351 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/files.py
+-rw-r--r--   0        0        0    11759 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/hive.py
+-rw-r--r--   0        0        0     6209 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/i2b2_mapping.py
+-rw-r--r--   0        0        0     2957 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/postgres.py
+-rw-r--r--   0        0        0    11528 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/settings.py
+-rw-r--r--   0        0        0       37 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/__init__.py
+-rw-r--r--   0        0        0     3766 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/biology.py
+-rw-r--r--   0        0        0     1053 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/care_site.py
+-rw-r--r--   0        0        0     3994 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/note.py
+-rw-r--r--   0        0        0    26222 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/synthetic.py
+-rw-r--r--   0        0        0     2814 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/utils.py
+-rw-r--r--   0        0        0     3557 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/io/synthetic/visit.py
+-rw-r--r--   0        0        0      395 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/__init__.py
+-rw-r--r--   0        0        0     2169 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error.py
+-rw-r--r--   0        0        0     2558 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error_after_t0.py
+-rw-r--r--   0        0        0     2718 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/metrics/error_between_t0_t1.py
+-rw-r--r--   0        0        0       42 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/__init__.py
+-rw-r--r--   0        0        0    10953 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/base.py
+-rw-r--r--   0        0        0       83 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/__init__.py
+-rw-r--r--   0        0        0      239 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/algos/__init__.py
+-rw-r--r--   0        0        0     3325 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     5621 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/rectangle_function.py
+-rw-r--r--   0        0        0     1450 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     5197 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1271 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0     1110 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      207 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/rectangle_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0       68 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/__init__.py
+-rw-r--r--   0        0        0     2666 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/loss_minimization.py
+-rw-r--r--   0        0        0     2528 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/algos/quantile.py
+-rw-r--r--   0        0        0     5292 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/step_function.py
+-rw-r--r--   0        0        0     1395 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/__init__.py
+-rw-r--r--   0        0        0     4315 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/defaults.py
+-rw-r--r--   0        0        0     1024 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      863 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/normalized_probe_plot.py
+-rw-r--r--   0        0        0      336 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/probe_dashboard.py
+-rw-r--r--   0        0        0      207 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/models/step_function/viz_configs/probe_plot.py
+-rw-r--r--   0        0        0      257 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/__init__.py
+-rw-r--r--   0        0        0    14033 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/base.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/__init__.py
+-rw-r--r--   0        0        0     9091 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/biology.py
+-rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     5688 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_measurement.py
+-rw-r--r--   0        0        0     6468 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     2595 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/__init__.py
+-rw-r--r--   0        0        0     5642 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/defaults.py
+-rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/n_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/__init__.py
+-rw-r--r--   0        0        0     5941 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/defaults.py
+-rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/estimates_densities_plot.py
+-rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/normalized_probe_plot.py
+-rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_measurement/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5963 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      488 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      693 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      568 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/biology/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/__init__.py
+-rw-r--r--   0        0        0      483 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7947 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_condition.py
+-rw-r--r--   0        0        0     8932 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6392 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/condition.py
+-rw-r--r--   0        0        0     2437 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/__init__.py
+-rw-r--r--   0        0        0     5701 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/n_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/__init__.py
+-rw-r--r--   0        0        0     5933 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_condition/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6549 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/condition/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/note/__init__.py
+-rw-r--r--   0        0        0      457 2023-06-30 07:53:41.124357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     7259 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_note.py
+-rw-r--r--   0        0        0     8556 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     6418 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/note.py
+-rw-r--r--   0        0        0     2278 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/__init__.py
+-rw-r--r--   0        0        0     5218 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/n_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/__init__.py
+-rw-r--r--   0        0        0     5475 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_note/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     6185 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/note/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/__init__.py
+-rw-r--r--   0        0        0    10772 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/filter_df.py
+-rw-r--r--   0        0        0    22364 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/prepare_df.py
+-rw-r--r--   0        0        0     6796 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/__init__.py
+-rw-r--r--   0        0        0     8269 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/per_visit.py
+-rw-r--r--   0        0        0     5326 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/visit.py
+-rw-r--r--   0        0        0     1795 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/__init__.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/__init__.py
+-rw-r--r--   0        0        0     4982 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/n_visit/probe_plot.py
+-rw-r--r--   0        0        0      322 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/__init__.py
+-rw-r--r--   0        0        0     5237 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/defaults.py
+-rw-r--r--   0        0        0      356 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/estimates_densities_plot.py
+-rw-r--r--   0        0        0      561 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_dashboard.py
+-rw-r--r--   0        0        0      308 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/normalized_probe_plot.py
+-rw-r--r--   0        0        0      436 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/probe_dashboard.py
+-rw-r--r--   0        0        0      210 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/probes/visit/viz_configs/per_visit/probe_plot.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/__init__.py
+-rw-r--r--   0        0        0     2498 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/checks.py
+-rw-r--r--   0        0        0     1108 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/file_management.py
+-rw-r--r--   0        0        0     2050 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/framework.py
+-rw-r--r--   0        0        0      176 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/loss_functions.py
+-rw-r--r--   0        0        0      344 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/utils/typing.py
+-rw-r--r--   0        0        0       52 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/normalized_probe/__init__.py
+-rw-r--r--   0        0        0    11510 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/__init__.py
+-rw-r--r--   0        0        0     4251 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/fitted_probe.py
+-rw-r--r--   0        0        0     3496 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/probe.py
+-rw-r--r--   0        0        0     7720 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/dashboards/probe/wrapper.py
+-rw-r--r--   0        0        0      339 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/estimates_densities/__init__.py
+-rw-r--r--   0        0        0     8510 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/estimates_densities/estimates_densities.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/normalized_probe/__init__.py
+-rw-r--r--   0        0        0     7491 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/normalized_probe/normalized_probe.py
+-rw-r--r--   0        0        0        0 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/__init__.py
+-rw-r--r--   0        0        0     2334 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/fitted_probe.py
+-rw-r--r--   0        0        0     1483 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/probe.py
+-rw-r--r--   0        0        0     5473 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/plots/probe/wrapper.py
+-rw-r--r--   0        0        0    16085 2023-06-30 07:53:41.128357 edsteva-0.2.0/edsteva/viz/utils.py
+-rw-r--r--   0        0        0     3307 2023-06-30 07:53:41.132357 edsteva-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5548 1970-01-01 00:00:00.000000 edsteva-0.2.0/setup.py
+-rw-r--r--   0        0        0     4362 1970-01-01 00:00:00.000000 edsteva-0.2.0/PKG-INFO
```

### Comparing `edsteva-0.1.4/LICENSE` & `edsteva-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/README.md` & `edsteva-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ```shell
 pip install edsteva
 ```
 We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
 
 ```
-pip install edsteva==0.1.4
+pip install edsteva==0.2.0
 ```
 ## Example
 
 A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
 ## Contributing
```

#### html2text {}

```diff
@@ -7,14 +7,14 @@
 https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
 at modeling the adoption over time and across space of the Electronic Health
 Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
 //spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
 Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
 install edsteva ``` We recommend pinning the library version in your projects,
 or use a strict package manager like [Poetry](https://python-poetry.org/). ```
-pip install edsteva==0.1.4 ``` ## Example A scientific paper is currently being
+pip install edsteva==0.2.0 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
 pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
 will always be given. ## Acknowledgement We would like to thank [Assistance
 Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
 (https://fondationrechercheaphp.fr/) for funding this project.
```

### Comparing `edsteva-0.1.4/edsteva/__init__.py` & `edsteva-0.2.0/edsteva/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.4"
+__version__ = "0.2.0"
 
 
 import importlib
 import os
 import sys
 import time
 from distutils.version import LooseVersion
@@ -39,20 +39,20 @@
 
 def set_env_variables() -> None:
     # From https://github.com/databricks/koalas/blob/master/databricks/koalas/__init__.py
     if LooseVersion(pyspark.__version__) < LooseVersion("3.0"):
         if LooseVersion(pyarrow.__version__) >= LooseVersion("0.15"):
             os.environ["ARROW_PRE_0_15_IPC_FORMAT"] = "1"
 
-    if LooseVersion(pyarrow.__version__) >= LooseVersion("2.0.0"):
+    if LooseVersion(pyarrow.__version__) >= LooseVersion("2.0.0"):  # pragma: no cover
         os.environ["PYARROW_IGNORE_TIMEZONE"] = "0"
 
 
 def improve_performances(
-    to_add_conf: List[Tuple[str, str]] = [],
+    to_add_conf: List[Tuple[str, str]] = None,
     quiet_spark: bool = True,
 ) -> Tuple[SparkSession, SparkContext, SparkSession.sql]:
     """
     (Re)defines various Spark variable with some configuration changes
     to improve performances by enabling Arrow
     This has to be done
     - Before launching a SparkCOntext
@@ -81,14 +81,17 @@
     conf = sc.getConf()
 
     # Synchronizing TimeZone
     tz = os.environ.get("TZ", "UTC")
     os.environ["TZ"] = tz
     time.tzset()
 
+    if to_add_conf is None:
+        to_add_conf = []
+
     to_add_conf.extend(
         [
             ("spark.app.name", f"{os.environ.get('USER')}_scikit"),
             ("spark.sql.session.timeZone", tz),
             ("spark.sql.execution.arrow.enabled", "true"),
             ("spark.sql.execution.arrow.pyspark.enabled", "true"),
         ]
```

### Comparing `edsteva-0.1.4/edsteva/io/files.py` & `edsteva-0.2.0/edsteva/io/files.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/io/hive.py` & `edsteva-0.2.0/edsteva/io/hive.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/io/i2b2_mapping.py` & `edsteva-0.2.0/edsteva/io/i2b2_mapping.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/io/postgres.py` & `edsteva-0.2.0/edsteva/io/postgres.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/io/settings.py` & `edsteva-0.2.0/edsteva/io/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,10 +373,10 @@
 }
 
 care_site_level_mapping = {
     30: "Hôpital",
     35: "Unité de consultation (UC)",
     45: "Pôle/DMU",
     50: "Unité Fonctionnelle (UF)",
-    70: "Unité d'hébergement (UH)",
+    70: "Unité d’hébergement (UH)",
     100: "Unité de consultation (UC)",
 }
```

### Comparing `edsteva-0.1.4/edsteva/io/synthetic/care_site.py` & `edsteva-0.2.0/edsteva/io/synthetic/care_site.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 import pandas as pd
 
 
-def split_name_id(string):
-    splitted = string.split("-")
-
-    # Name - Type - ID
-    return dict(
-        care_site_short_name=string,
-        care_site_type_source_value=splitted[0],
-        care_site_id=splitted[1],
-    )
-
-
 def generate_care_site_tables(structure, parent=None, final=True):
     cs = []
     fr = []
     for key, value in structure.items():
-        this_cs = split_name_id(key)
+        this_cs = _split_name_id(key)
         cs.append(this_cs)
 
         if parent is not None:
             this_fr = dict(
                 fact_id_1=this_cs["care_site_id"],
                 fact_id_2=parent["care_site_id"],
             )
@@ -36,7 +25,18 @@
     if final:
         cs = pd.DataFrame(cs)
         fr = pd.DataFrame(fr)
         fr["domain_concept_id_1"] = 57
         fr["relationship_concept_id"] = 46233688
 
     return cs, fr
+
+
+def _split_name_id(string):
+    splitted = string.split("-")
+
+    # Name - Type - ID
+    return dict(
+        care_site_short_name=string,
+        care_site_type_source_value=splitted[0],
+        care_site_id=splitted[1],
+    )
```

### Comparing `edsteva-0.1.4/edsteva/metrics/error.py` & `edsteva-0.2.0/edsteva/metrics/error.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/metrics/error_after_t0.py` & `edsteva-0.2.0/edsteva/metrics/error_after_t0.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/metrics/error_between_t0_t1.py` & `edsteva-0.2.0/edsteva/metrics/error_between_t0_t1.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/models/base.py` & `edsteva-0.2.0/edsteva/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from abc import ABCMeta, abstractmethod
 from functools import reduce
-from typing import Callable, List
+from typing import List
 
 import pandas as pd
+from loguru import logger
 
 from edsteva import CACHE_DIR
+from edsteva.metrics import metrics
 from edsteva.probes.base import BaseProbe
-from edsteva.probes.utils import (
-    delete_object,
-    filter_table_by_date,
-    load_object,
-    save_object,
-)
+from edsteva.probes.utils.filter_df import filter_table_by_date
+from edsteva.utils.file_management import delete_object, load_object, save_object
 
 
 class BaseModel(metaclass=ABCMeta):
 
     """Base class for Models
 
     Attributes
@@ -30,37 +28,37 @@
         The list of computed metrics if any
     params: List[str]
         Available with the [``fit()``][edsteva.models.base.BaseModel.fit] method
 
         Ths list of extra keyword parameters used.
     """
 
-    def __init__(self):
-        self.is_valid_model()
-        self.name = type(self).__name__
-
-    def is_valid_model(self) -> None:
-        """Raises an error if the instantiated Model is not valid"""
-        if not hasattr(self, "_coefs"):
-            raise Exception(
-                "Model must have _coefs attribute. Please review the code of your model"
-            )
+    def __init__(
+        self,
+        algo: str,
+        coefs: List[str],
+        default_metrics: List[str],
+    ):
+        self._algo = algo
+        self._coefs = coefs
+        self._default_metrics = default_metrics
+        self._viz_config = {}
 
     def is_computed_estimates(self) -> None:
         """Raises an error if the Probe has not been fitted properly"""
         if hasattr(self, "estimates"):
             if isinstance(self.estimates, pd.DataFrame):
                 if len(self.estimates) == 0:
                     raise Exception(
                         "Estimates are empty, please review the process method or your arguments"
                     )
             else:
                 raise Exception(
                     "The fit process must return a Pandas Dataframe and not {}".format(
-                        type(self.estimates)
+                        type(self.estimates).__name__
                     )
                 )
 
         else:
             raise Exception(
                 "Model has not been fitted, please use the fit method as follow: Model.fit()"
             )
@@ -81,26 +79,27 @@
         **kwargs,
     ):
         """Compute the predicted Probe"""
 
     def fit(
         self,
         probe: BaseProbe,
-        metric_functions: List[Callable] = None,
+        metric_functions: List[str] = None,
         start_date: str = None,
         end_date: str = None,
+        with_cache: bool = True,
         **kwargs,
     ) -> None:
         """Fit the model to the probe instance
 
         Parameters
         ----------
         probe : BaseProbe
             Target variable to be fitted
-        metric_functions : List[Callable], optional
+        metric_functions : List[str], optional
             Metrics to apply on the fitted Probe. By default it will apply the default metric specified in the model.
 
             **EXAMPLE**: `[error, error_after_t0]`
         start_date : str, optional
             **EXAMPLE**: `"2019-05-01"`
         end_date : str, optional
             **EXAMPLE**: `"2021-07-01"`
@@ -122,15 +121,17 @@
         | Pôle/DMU                 | 8312027648   | 'Urg_Hospit' | 2021-03-01 | 0.677 | 0.022 |
         | Pôle/DMU                 | 8312027648   | 'All'        | 2018-08-01 | 0.764 | 0.014 |
         | Hôpital                  | 8312022130   | 'Urg_Hospit' | 2022-02-01 | 0.652 | 0.027 |
         """
         if isinstance(probe, BaseProbe):
             probe.is_computed_probe()
         else:
-            raise TypeError("Unsupported type {} for probe.".format(type(probe)))
+            raise TypeError(
+                "Unsupported type {} for probe.".format(type(probe).__name__)
+            )
 
         predictor = filter_table_by_date(
             table=probe.predictor,
             table_name="predictor",
             start_date=start_date,
             end_date=end_date,
         )
@@ -138,30 +139,47 @@
 
         estimates = self.fit_process(
             predictor=predictor,
             index=index,
             **kwargs,
         )
 
-        metrics = self._compute_metrics(
+        metrics_df = self._compute_metrics(
             predictor=predictor,
             estimates=estimates,
             index=index,
             metric_functions=metric_functions,
         )
 
-        if metrics is not None:
-            self._metrics = list(metrics.columns.difference(index))
-            self.estimates = estimates.merge(metrics, on=index)
+        if metrics_df is not None:
+            self._metrics = list(metrics_df.columns.difference(index))
+            self.estimates = estimates.merge(metrics_df, on=index)
 
         else:
             self.estimates = estimates
 
         self.is_computed_estimates()
         self.params = kwargs
+        if with_cache:
+            self.cache_estimates()
+
+    def reset_estimates(
+        self,
+    ) -> None:
+        """Reset the estimates to its initial state"""
+        self.estimates = self._cache_estimates.copy()
+
+    def cache_estimates(
+        self,
+    ) -> None:
+        """Cache the predictor"""
+        self._cache_estimates = self.estimates.copy()
+        logger.info(
+            "Cache the estimates, you can reset the estimates to this state with the method reset_estimates"
+        )
 
     def predict(
         self,
         probe: BaseProbe,
     ) -> pd.DataFrame:
         """Computes the predicted probe by using the estimates
 
@@ -174,21 +192,21 @@
         --------
         ```python
         from edsteva.models.step_function import StepFunction
 
         step_function_model.predict(visit).head()
         ```
 
-        | care_site_level          | care_site_id | care_site_short_name | stay_type    | date       | n_visit | c     | c_fit |
-        | :----------------------- | :----------- | :------------------- | :----------- | :--------- | :------ | :---- | :---- |
-        | Unité Fonctionnelle (UF) | 8312056386   | Care site 1          | 'Urg_Hospit' | 2019-05-01 | 233.0   | 0.841 | 0.758 |
-        | Unité Fonctionnelle (UF) | 8312056386   | Care site 1          | 'All'        | 2021-04-01 | 393.0   | 0.640 | 0.758 |
-        | Pôle/DMU                 | 8312027648   | Care site 2          | 'Urg_Hospit' | 2011-03-01 | 204.0   | 0.497 | 0     |
-        | Pôle/DMU                 | 8312027648   | Care site 2          | 'All'        | 2018-08-01 | 22.0    | 0.784 | 0.874 |
-        | Hôpital                  | 8312022130   | Care site 3          | 'Urg_Hospit' | 2022-02-01 | 9746.0  | 0.974 | 0.912 |
+        | care_site_level          | care_site_id | stay_type    | date       | n_visit | c     | c_fit |
+        | :----------------------- | :----------- | :----------- | :--------- | :------ | :---- | :---- |
+        | Unité Fonctionnelle (UF) | 8312056386   | 'Urg_Hospit' | 2019-05-01 | 233.0   | 0.841 | 0.758 |
+        | Unité Fonctionnelle (UF) | 8312056386   | 'All'        | 2021-04-01 | 393.0   | 0.640 | 0.758 |
+        | Pôle/DMU                 | 8312027648   | 'Urg_Hospit' | 2011-03-01 | 204.0   | 0.497 | 0     |
+        | Pôle/DMU                 | 8312027648   | 'All'        | 2018-08-01 | 22.0    | 0.784 | 0.874 |
+        | Hôpital                  | 8312022130   | 'Urg_Hospit' | 2022-02-01 | 9746.0  | 0.974 | 0.912 |
 
         """
 
         predictor = probe.predictor
         index = probe._index
 
         prediction = self.predict_process(predictor=predictor, index=index)
@@ -211,17 +229,15 @@
 
         visit = VisitProbe()
         visit.load(path=probe_path)
         ```
 
         """
 
-        if not path:
-            path = CACHE_DIR / "edsteva" / "models" / f"{self.name.lower()}.pickle"
-
+        path = path or self._get_path()
         loaded_model = load_object(path)
         self.__dict__ = loaded_model.__dict__.copy()
         self.path = path
 
     def save(self, path: str = None, name: str = None) -> bool:
         """Saves computed Model instance
 
@@ -244,84 +260,69 @@
         visit.save(path=probe_path)
         ```
 
         """
 
         self.is_computed_estimates()
 
+        if name:
+            self.name = name
         if not path:
-            if name:
-                self.name = name
-            path = CACHE_DIR / "edsteva" / "models" / f"{self.name.lower()}.pickle"
+            path = self._get_path()
 
         self.path = path
         save_object(self, path)
 
     def delete(self, path: str = None) -> bool:
         """Delete the saved Model instance
 
         Parameters
         ----------
         path : str, optional
             **EXAMPLE**: `"my_folder/my_file.html"`
         """
-
         if not path:
-            if hasattr(self, "path"):
-                path = self.path
-            else:
-                path = CACHE_DIR / "edsteva" / "models" / f"{self.name.lower()}.pickle"
+            path = self.path
 
         delete_object(self, path)
 
+    def _get_path(self):
+        base_path = CACHE_DIR / "edsteva" / "models"
+        if hasattr(self, "name"):
+            filename = f"{self.name.lower()}.pickle"
+        else:
+            filename = f"{type(self).__name__.lower()}.pickle"
+        return base_path / filename
+
     def _compute_metrics(
         self,
         predictor: pd.DataFrame,
         estimates: pd.DataFrame,
         index: List[str],
-        metric_functions: List[Callable] = None,
+        metric_functions: List[str] = None,
     ):
-        if metric_functions:
-            if callable(metric_functions):
-                metrics = metric_functions(
-                    predictor=predictor, estimates=estimates, index=index
-                )
-            elif isinstance(metric_functions, list):
-                metrics = []
-                for metric_function in metric_functions:
-                    if callable(metric_function):
-                        metrics.append(
-                            metric_function(
-                                predictor=predictor, estimates=estimates, index=index
-                            )
-                        )
-                    else:
-                        raise TypeError(
-                            "{} is not callable. The metrics input must be a list of callable functions".format(
-                                type(metric_function)
-                            )
-                        )
-                metrics = reduce(
-                    lambda left, right: pd.merge(left, right, on=index), metrics
-                )
+        if metric_functions is None:
+            if hasattr(self, "_default_metrics") and self._default_metrics:
+                metric_functions = self._default_metrics
             else:
-                raise TypeError(
-                    "{} is not callable. The metrics input must be a callable function".format(
-                        type(metrics)
-                    )
+                return None
+        if isinstance(metric_functions, str):
+            metric_functions = [metric_functions]
+        metrics_df = []
+        for metric_function in metric_functions:
+            metrics_df.append(
+                metrics.get(metric_function)(
+                    predictor=predictor, estimates=estimates, index=index
                 )
-
-        elif hasattr(self, "default_metrics"):
-            metrics = self.default_metrics(
-                predictor=predictor, estimates=estimates, index=index
             )
-        else:
-            metrics = None
+        metrics_df = reduce(
+            lambda left, right: pd.merge(left, right, on=index), metrics_df
+        )
 
-        return metrics
+        return metrics_df
 
     def is_predictable_probe(
         self,
         predictor: pd.DataFrame,
         index: List[str],
     ) -> pd.DataFrame:
         """Raises an error if the model has not been fitted on the input predictor.
```

### Comparing `edsteva-0.1.4/edsteva/models/rectangle_function/algos/loss_minimization.py` & `edsteva-0.2.0/edsteva/models/rectangle_function/algos/loss_minimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,26 @@
 
     Parameters
     ----------
     predictor : pd.DataFrame
         $c(t)$ computed in the Probe.
     index : List[str]
         Variable from which data is grouped.
-
         **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
     x_col : str, optional
         Column name for the time variable $t$.
     y_col : str, optional
         Column name  for the completeness variable $c(t)$.
     loss_function : Callable, optional
         The loss function $\mathcal{L}$.
     min_rect_month_width : int, optional
         Min number of months between $t_0$ and $t_1$.
     """
     check_columns(df=predictor, required_columns=index + [x_col, y_col])
+    predictor = predictor.sort_values(x_col)
     cols = index + [x_col, y_col]
     iter = predictor[cols].groupby(index)
     results = []
     for partition, group in iter:
         row = dict(zip(index, partition))
         t_0, c_0, t_1 = _compute_one_double_threshold(
             group,
@@ -79,15 +79,15 @@
     y_col: str,
     loss_func: Callable,
     min_rect_month_width: int,
 ):
     target = group[[x_col, y_col]].values
     best_x0 = best_y0 = best_x1 = None
     best_loss = np.inf
-    for idx in range(1, len(target) - min_rect_month_width):
+    for idx in range(len(target) - min_rect_month_width):
         x0 = target[idx, 0]
         y_before_x0 = target[:idx, 1]
         for jdx in range(idx + min_rect_month_width, len(target)):
             x1 = target[jdx, 0]
             y_between_x0_x1 = target[idx:jdx, 1]
             y_after_x1 = target[jdx:, 1]
             y0 = y_between_x0_x1.mean()
```

### Comparing `edsteva-0.1.4/edsteva/models/rectangle_function/rectangle_function.py` & `edsteva-0.2.0/edsteva/models/rectangle_function/rectangle_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable, List
+from typing import List
 
 import pandas as pd
 
-from edsteva.metrics import error_between_t0_t1
 from edsteva.models import BaseModel
-from edsteva.models.rectangle_function import algos
+from edsteva.models.rectangle_function.algos import algos
+from edsteva.models.rectangle_function.viz_configs import viz_configs
 
 
 class RectangleFunction(BaseModel):
     r"""It models the completeness predictor $c(t)$ as a rectangle function $f_{t_0, c_0, t_1}(t)$ as follow:
 
     $$
     f_{t_0, c_0, t_1}(t) = c_0 \ \mathbb{1}_{t_0 \leq t \leq t_1}(t)
@@ -18,18 +18,26 @@
 
     - the characteristic time $t_0$ estimates the time after which the data is available.
     - the characteristic time $t_1$ estimates the time after which the data is not available anymore.
     - the characteristic value $c_0$ estimates the completeness between $t_0$ and $t_1$.
 
     Attributes
     ----------
+    _algo: List[str]
+        Algorithm used to compute the estimates
+        **VALUE**: ``"loss_minimization"``
     _coefs: List[str]
         Model coefficients
-
         **VALUE**: ``["t_0", "c_0", "t_1"]``
+    _default_metrics: List[str]
+        Metrics to used by default
+        **VALUE**: ``[error_between_t0_t1]``
+    _viz_config: List[str]
+        Dictionary of configuration for visualization purpose.
+        **VALUE**: ``{}``
 
     Example
     ----------
 
     ```python
     from edsteva.models.step_function import StepFunction
 
@@ -43,37 +51,52 @@
     | Unité Fonctionnelle (UF) | 8312056386   | 'Urg'     | 2019-05-01 | 0.397 | 2020-05-01 | 0.040 |
     | Unité Fonctionnelle (UF) | 8312056386   | 'All'     | 2011-04-01 | 0.583 | 2013-04-01 | 0.028 |
     | Pôle/DMU                 | 8312027648   | 'Hospit'  | 2021-03-01 | 0.677 | 2022-03-01 | 0.022 |
     | Pôle/DMU                 | 8312027648   | 'All'     | 2018-08-01 | 0.764 | 2019-08-01 | 0.014 |
     | Hôpital                  | 8312022130   | 'Hospit'  | 2022-02-01 | 0.652 | 2022-08-01 | 0.027 |
     """
 
-    _coefs = ["t_0", "c_0", "t_1"]
+    def __init__(
+        self,
+        algo: str = "loss_minimization",
+    ):
+        """Initialisation of the RectangleFunction Model.
+
+        Parameters
+        ----------
+        algo : Callable, optional
+            Algorithm used for the coefficients estimation ($t_0$, $t_1$ and $c_0$)
+        """
+        coefs = ["t_0", "c_0", "t_1"]
+        default_metrics = ["error_between_t0_t1"]
+        super().__init__(
+            algo=algo,
+            coefs=coefs,
+            default_metrics=default_metrics,
+        )
 
     def fit_process(
         self,
         predictor: pd.DataFrame,
         index: List[str] = None,
-        algo: Callable = algos.loss_minimization,
         **kwargs,
     ):
         """Script to be used by [``fit()``][edsteva.models.base.BaseModel.fit]
 
         Parameters
         ----------
         predictor : pd.DataFrame
             Target variable to be fitted
         index : List[str], optional
             Variable from which data is grouped
-
             **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
-        algo : Callable, optional
-            Algorithm used for the coefficients estimation ($t_0$ and $c_0$)
         """
-        return algo(predictor, index, **kwargs)
+        estimates = algos.get(self._algo)(predictor=predictor, index=index, **kwargs)
+
+        return estimates
 
     def predict_process(
         self,
         predictor: pd.DataFrame,
         index: List[str],
     ):
         """Script to be used by [``predict()``][edsteva.models.base.BaseModel.predict]
@@ -108,33 +131,17 @@
         prediction = self.is_predictable_probe(predictor, index)
 
         rect_mask = (prediction["date"] >= prediction["t_0"]) & (
             prediction["date"] <= prediction["t_1"]
         )
         prediction["c_hat"] = prediction["c_0"].where(rect_mask, 0)
 
-        return prediction.drop(columns=self._coefs + self._metrics)
-
-    def default_metrics(
-        self,
-        predictor: pd.DataFrame,
-        estimates: pd.DataFrame,
-        index: List[str],
-    ):
-        r"""Default metrics used if metric_functions is set to None. Here the default metric is the mean squared error between $t_0$ and $t_1$.
+        return prediction.drop(columns=self._metrics)
 
-        Parameters
-        ----------
-        predictor : pd.DataFrame
-            Target DataFrame describing the completeness predictor $c(t)$
-        estimates : pd.DataFrame
-            Target DataFrame describing the estimates $(\hat{t_0}, \hat{c_0})$
-        index : List[str]
-            Variable from which data is grouped
-
-            **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
-        """
-        return error_between_t0_t1(
-            predictor=predictor,
-            estimates=estimates,
-            index=index,
-        )
+    def get_viz_config(self, viz_type: str, **kwargs):
+        if viz_type in viz_configs.keys():
+            _viz_config = self._viz_config.get(viz_type)
+            if _viz_config is None:
+                _viz_config = "default"
+        else:
+            raise ValueError(f"edsteva has no {viz_type} registry !")
+        return viz_configs[viz_type].get(_viz_config)(self, **kwargs)
```

### Comparing `edsteva-0.1.4/edsteva/models/step_function/algos/loss_minimization.py` & `edsteva-0.2.0/edsteva/models/step_function/algos/loss_minimization.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Column name for the time variable $t$
     y_col : str, optional
         Column name  for the completeness variable $c(t)$
     loss_function : Callable, optional
         The loss function $\mathcal{L}$
     """
     check_columns(df=predictor, required_columns=index + [x_col, y_col])
-
+    predictor = predictor.sort_values(x_col)
     cols = index + [x_col, y_col]
     iter = predictor[cols].groupby(index)
     results = []
     for partition, group in iter:
         row = dict(zip(index, partition))
         t_0, c_0 = _compute_one_threshold(
             group,
@@ -72,15 +72,15 @@
     group: pd.DataFrame,
     x_col: str,
     y_col: str,
     loss_func: Callable,
 ):
     target = group[[x_col, y_col]].values
     best_loss, best_x0, best_y0 = np.inf, None, None
-    for idx in range(1, len(target)):
+    for idx in range(len(target)):
         x0 = target[idx, 0]
         y_before_x0 = target[:idx, 1]
         y_after_x0 = target[idx:, 1]
         y0 = y_after_x0.mean()
         residual = np.hstack([y_before_x0, (y_after_x0 - y0)])
         loss = loss_func(residual).mean()
         if loss < best_loss:
```

### Comparing `edsteva-0.1.4/edsteva/models/step_function/algos/quantile.py` & `edsteva-0.2.0/edsteva/models/step_function/algos/quantile.py`

 * *Files identical despite different names*

### Comparing `edsteva-0.1.4/edsteva/models/step_function/step_function.py` & `edsteva-0.2.0/edsteva/models/step_function/step_function.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Callable, List
+from typing import List
 
 import pandas as pd
 
-from edsteva.metrics import error_after_t0
 from edsteva.models import BaseModel
-from edsteva.models.step_function import algos
+from edsteva.models.step_function.algos import algos
+from edsteva.models.step_function.viz_configs import viz_configs
 
 
 class StepFunction(BaseModel):
     r"""It models the completeness predictor $c(t)$ as a step function $f_{t_0, c_0}(t)$ as follow:
 
     $$
     f_{t_0, c_0}(t) = c_0 \ \mathbb{1}_{t \geq t_0}(t)
@@ -17,18 +17,26 @@
     It computes the following estimates $(t_0, c_0)$:
 
     - the characteristic time $t_0$ estimates the time after which the data is available
     - the characteristic value $c_0$ estimates the stabilized routine completeness
 
     Attributes
     ----------
+    _algo: List[str]
+        Algorithm used to compute the estimates
+        **VALUE**: ``"loss_minimization"``
     _coefs: List[str]
         Model coefficients
-
         **VALUE**: ``["t_0", "c_0"]``
+    _default_metrics: List[str]
+        Metrics to used by default
+        **VALUE**: ``[error_after_t0]``
+    _viz_config: List[str]
+        Dictionary of configuration for visualization purpose.
+        **VALUE**: ``{}``
 
     Example
     ----------
 
     ```python
     from edsteva.models.step_function import StepFunction
 
@@ -42,38 +50,51 @@
     | Unité Fonctionnelle (UF) | 8312056386   | 'Urg_Hospit' | 2019-05-01 | 0.397 |
     | Unité Fonctionnelle (UF) | 8312056386   | 'All'        | 2011-04-01 | 0.583 |
     | Pôle/DMU                 | 8312027648   | 'Urg_Hospit' | 2021-03-01 | 0.677 |
     | Pôle/DMU                 | 8312027648   | 'All'        | 2018-08-01 | 0.764 |
     | Hôpital                  | 8312022130   | 'Urg_Hospit' | 2022-02-01 | 0.652 |
     """
 
-    _coefs = ["t_0", "c_0"]
+    def __init__(
+        self,
+        algo: str = "loss_minimization",
+    ):
+        """Initialisation of the StepFunction Model.
+
+        Parameters
+        ----------
+        algo : Callable, optional
+            Algorithm used for the coefficients estimation ($t_0$ and $c_0$)
+        """
+        coefs = ["t_0", "c_0"]
+        default_metrics = ["error_after_t0"]
+        super().__init__(
+            algo=algo,
+            coefs=coefs,
+            default_metrics=default_metrics,
+        )
 
     def fit_process(
         self,
         predictor: pd.DataFrame,
         index: List[str] = None,
-        algo: Callable = algos.loss_minimization,
-        **kwargs
+        **kwargs,
     ) -> None:
         """Script to be used by [``fit()``][edsteva.models.base.BaseModel.fit]
 
         Parameters
         ----------
         predictor : pd.DataFrame
             Target variable to be fitted
         index : List[str], optional
             Variable from which data is grouped
-
             **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
-        algo : Callable, optional
-            Algorithm used for the coefficients estimation ($t_0$ and $c_0$)
         """
 
-        estimates = algo(predictor=predictor, index=index, **kwargs)
+        estimates = algos.get(self._algo)(predictor=predictor, index=index, **kwargs)
 
         return estimates[index + self._coefs]
 
     def predict_process(
         self,
         predictor: pd.DataFrame,
         index: List[str],
@@ -109,29 +130,17 @@
         """
 
         prediction = self.is_predictable_probe(predictor=predictor, index=index)
 
         prediction["c_hat"] = prediction["c_0"].where(
             prediction["date"] >= prediction["t_0"], 0
         )
-        return prediction.drop(columns=self._coefs + self._metrics)
+        return prediction.drop(columns=self._metrics)
 
-    def default_metrics(
-        self,
-        predictor: pd.DataFrame,
-        estimates: pd.DataFrame,
-        index: List[str],
-    ):
-        r"""Default metrics used if metric_functions is set to None. Here the default metric is the mean squared error computed after $t_0$
-
-        Parameters
-        ----------
-        predictor : pd.DataFrame
-            Target DataFrame describing the completeness predictor $c(t)$
-        estimates : pd.DataFrame
-            Target DataFrame describing the estimates $(\hat{t_0}, \hat{c_0})$
-        index : List[str]
-            Variable from which data is grouped
-
-            **EXAMPLE**: `["care_site_level", "stay_type", "note_type", "care_site_id"]`
-        """
-        return error_after_t0(predictor=predictor, estimates=estimates, index=index)
+    def get_viz_config(self, viz_type: str, **kwargs):
+        if viz_type in viz_configs.keys():
+            _viz_config = self._viz_config.get(viz_type)
+            if _viz_config is None:
+                _viz_config = "default"
+        else:
+            raise ValueError(f"edsteva has no {viz_type} registry !")
+        return viz_configs[viz_type].get(_viz_config)(self, **kwargs)
```

### Comparing `edsteva-0.1.4/edsteva/probes/base.py` & `edsteva-0.2.0/edsteva/probes/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 from abc import ABCMeta, abstractmethod
 from typing import Dict, List, Union
 
 import pandas as pd
 from loguru import logger
 
 from edsteva import CACHE_DIR
-from edsteva.probes.utils import (
-    delete_object,
-    filter_table_by_care_site,
-    get_care_site_relationship,
-    load_object,
-    save_object,
-)
+from edsteva.probes.utils.filter_df import filter_table_by_care_site
+from edsteva.probes.utils.prepare_df import prepare_care_site_relationship
 from edsteva.utils.checks import check_columns, check_tables
-from edsteva.utils.typing import Data
+from edsteva.utils.file_management import delete_object, load_object, save_object
+from edsteva.utils.typing import Data, DataFrame
 
 
 class BaseProbe(metaclass=ABCMeta):
     """Base class for Probes
 
     Attributes
     ----------
@@ -31,58 +27,56 @@
     _cache_predictor: pd.DataFrame
         Available with the [``compute()``][edsteva.probes.base.BaseProbe.compute] method
 
         It is a copy of the predictor DataFrame used to [``reset_predictor()``][edsteva.probes.base.BaseProbe.reset_predictor]
     care_site_relationship: pd.DataFrame
         Available with the [``compute()``][edsteva.probes.base.BaseProbe.compute] method
 
-        It describes the care site structure (cf. [``get_care_site_relationship()``][edsteva.probes.utils.get_care_site_relationship])
+        It describes the care site structure (cf. [``prepare_care_site_relationship()``][edsteva.probes.utils.prepare_df.prepare_care_site_relationship])
     """
 
-    def __init__(self):
-        self.is_valid_probe()
-        self.name = self._get_name()
+    _schema = ["care_site_level", "care_site_id", "date", "c"]
 
-    _schema = ["care_site_id", "care_site_level", "stay_type", "date", "c"]
+    def __init__(
+        self,
+        completeness_predictor: str,
+        index: List[str],
+    ):
+        self._completeness_predictor = completeness_predictor
+        self._cache_index = index.copy()
+        self._viz_config = {}
 
     def validate_input_data(self, data: Data) -> None:
         """Raises an error if the input data is not valid
 
         Parameters
         ----------
         data: Data
             Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]
         """
 
         if not isinstance(data, Data.__args__):
-            raise TypeError("Unsupported type {} for data".format(type(data)))
+            raise TypeError("Unsupported type {} for data".format(type(data).__name__))
 
         check_tables(
             data=data,
             required_tables=[
                 "visit_occurrence",
                 "care_site",
                 "fact_relationship",
             ],
         )
 
-    def is_valid_probe(self) -> None:
-        """Raises an error if the instantiated Probe is not valid"""
-        if not hasattr(self, "_index"):
-            raise Exception(
-                "Probe must have _index attribute. Please review the code of your probe"
-            )
-
     def is_computed_probe(self) -> None:
         """Raises an error if the Probe has not been computed properly"""
         if hasattr(self, "predictor"):
             if not isinstance(self.predictor, pd.DataFrame):
                 raise TypeError(
                     "Predictor must be a Pandas DataFrame and not a {}, please review the process method or your arguments".format(
-                        type(self.predictor)
+                        type(self.predictor).__name__
                     )
                 )
             if self.predictor.empty:
                 raise Exception(
                     "Predictor is empty, please review the process method or your arguments"
                 )
             check_columns(
@@ -101,101 +95,64 @@
                         )
                     )
         else:
             raise Exception(
                 "Predictor has not been computed, please use the compute method as follow: Predictor.compute()"
             )
 
-    def impute_missing_date(
-        self,
-        only_impute_per_care_site: bool = False,
-    ) -> pd.DataFrame:
-        """Impute missing date with 0 on the predictor of a probe.
-
-        Parameters
-        ----------
-        only_impute_per_care_site : bool, optional
-            If True it will only impute missing date between the first and the last observation of each care site.
-            If False it will impute missing data on the entire study period whatever the care site
-        """
-        # Check if probe has been computed.
-        self.is_computed_probe()
-
-        # Set start_date to the beginning of the month.
-        date_index = pd.date_range(
-            start=self.start_date,
-            end=self.end_date,
-            freq="MS",
-            closed="left",
+    def filter_date_per_care_site(self, target_column: str):
+        filtered_predictor = self.predictor.copy()
+        predictor_activity = self.predictor[self.predictor[target_column] > 0].copy()
+        predictor_activity = (
+            predictor_activity.groupby("care_site_id")
+            .agg({"date": ["min", "max"]})
+            .droplevel(axis="columns", level=0)
+            .reset_index()
         )
-        date_index = pd.DataFrame({"date": date_index})
-
-        # Precompute the mapping:
-        # {'Hôpital-1': {'min': Timestamp('2010-06-01'), 'max': Timestamp('2019-11-01')}
-        if only_impute_per_care_site:
-            site_to_min_max_ds = (
-                self.predictor.groupby(["care_site_short_name"])["date"]
-                .agg([min, max])
-                .to_dict("index")
-            )
-
-        partition_cols = self._index + ["care_site_short_name"]
-        groups = []
-        for partition, group in self.predictor.groupby(partition_cols):
-            group = date_index.merge(group, on="date", how="left")
-
-            # Filter on each care site timeframe.
-            if only_impute_per_care_site:
-                care_site_short_name = partition[-1]
-                ds_min = site_to_min_max_ds[care_site_short_name]["min"]
-                ds_max = site_to_min_max_ds[care_site_short_name]["max"]
-                group = group.loc[(group["date"] >= ds_min) & (group["date"] <= ds_max)]
-
-            # Fill specific partition values.
-            for key, val in zip(partition_cols, partition):
-                group[key] = val
-            # Fill remaining NaN from counts values with 0.
-            group.fillna(0, inplace=True)
-            groups.append(group)
-
-        self.predictor = pd.concat(groups)
+        filtered_predictor = filtered_predictor.merge(
+            predictor_activity, on="care_site_id"
+        )
+        filtered_predictor = filtered_predictor[
+            (filtered_predictor["date"] >= filtered_predictor["min"])
+            & (filtered_predictor["date"] <= filtered_predictor["max"])
+        ].drop(columns=["min", "max"])
+        self.predictor = filtered_predictor
 
     @abstractmethod
     def compute_process(
         self,
         data: Data,
         care_site_relationship: pd.DataFrame,
-        start_date: datetime = None,
-        end_date: datetime = None,
-        care_site_levels: List[str] = None,
-        stay_types: Union[str, Dict[str, str]] = None,
-        care_site_ids: List[int] = None,
+        start_date: datetime,
+        end_date: datetime,
+        care_site_levels: List[str],
+        stay_types: Union[str, Dict[str, str]],
+        care_site_ids: List[int],
         **kwargs,
     ) -> pd.DataFrame:
         """Process the data in order to obtain a predictor table"""
 
     def compute(
         self,
         data: Data,
         start_date: datetime = None,
         end_date: datetime = None,
         care_site_levels: List[str] = None,
         stay_types: Union[str, Dict[str, str]] = None,
         care_site_ids: List[int] = None,
-        impute_missing_dates: bool = True,
-        only_impute_per_care_site: bool = False,
+        with_cache: bool = True,
         **kwargs,
     ) -> None:
         """Calls [``compute_process()``][edsteva.probes.base.BaseProbe.compute_process]
 
 
         Here are the following computation steps:
 
         - check if input data is valid with [``validate_input_data()``][edsteva.probes.base.BaseProbe.validate_input_data] method
-        - query care site relationship table with [``get_care_site_relationship()``][edsteva.probes.utils.get_care_site_relationship]
+        - query care site relationship table with [``prepare_care_site_relationship()``][edsteva.probes.utils.prepare_df.prepare_care_site_relationship]
         - compute predictor with [``compute_process()``][edsteva.probes.base.BaseProbe.compute_process] method
         - check if predictor is valid with [``is_computed_probe()``][edsteva.probes.base.BaseProbe.is_computed_probe] method
 
 
 
         Parameters
         ----------
@@ -242,41 +199,33 @@
         | Pôle/DMU                 | 8312027648   | Care site 2          | Urg_and_consult | 2011-03-01 | 204.0   | 0.497 |
         | Pôle/DMU                 | 8312027648   | Care site 2          | 'All'           | 2018-08-01 | 22.0    | 0.274 |
         | Hôpital                  | 8312022130   | Care site 3          | Urg_and_consult | 2022-02-01 | 9746.0  | 0.769 |
 
 
         """
         self.validate_input_data(data=data)
-        care_site_relationship = get_care_site_relationship(data=data)
-
+        self._reset_index()
+        care_site_relationship = prepare_care_site_relationship(data=data)
+        self.start_date = pd.to_datetime(start_date) if start_date else None
+        self.end_date = pd.to_datetime(end_date) if end_date else None
         self.predictor = self.compute_process(
             data=data,
             care_site_relationship=care_site_relationship,
             start_date=start_date,
             end_date=end_date,
             care_site_levels=care_site_levels,
             stay_types=stay_types,
             care_site_ids=care_site_ids,
             **kwargs,
         )
         self.is_computed_probe()
-
-        self.start_date = (
-            pd.to_datetime(start_date) if start_date else self.predictor["date"].min()
-        )
-        self.end_date = (
-            pd.to_datetime(end_date) if end_date else self.predictor["date"].max()
-        )
-
-        if impute_missing_dates:
-            self.impute_missing_date(
-                only_impute_per_care_site=only_impute_per_care_site,
-            )
-        self.cache_predictor()
         self.care_site_relationship = care_site_relationship
+        self.predictor = self.add_names_columns(self.predictor)
+        if with_cache:
+            self.cache_predictor()
 
     def reset_predictor(
         self,
     ) -> None:
         """Reset the predictor to its initial state"""
         self.predictor = self._cache_predictor.copy()
 
@@ -289,33 +238,62 @@
             "Cache the predictor, you can reset the predictor to this state with the method reset_predictor"
         )
 
     def filter_care_site(
         self,
         care_site_ids: Union[int, List[int]] = None,
         care_site_short_names: Union[str, List[str]] = None,
+        care_site_specialties: Union[str, List[str]] = None,
     ) -> None:
         """Filters all the care sites related to the selected care sites.
 
         Parameters
         ----------
         care_site_ids : Union[int, List[int]], optional
             **EXAMPLE**: `[8312056386, 8312027648]`
         care_site_short_names : Union[str, List[str]], optional
             **EXAMPLE**: `["HOSPITAL 1", "HOSPITAL 2"]`
         """
         self.predictor = filter_table_by_care_site(
             table_to_filter=self.predictor,
-            table_name="{} predictor".format(type(self).__name__.lower()),
             care_site_relationship=self.care_site_relationship,
             care_site_ids=care_site_ids,
             care_site_short_names=care_site_short_names,
+            care_site_specialties=care_site_specialties,
         )
         logger.info("Use probe.reset_predictor() to get back the initial predictor")
 
+    def add_names_columns(self, df: DataFrame):
+        if hasattr(self, "care_site_relationship") and "care_site_id" in df.columns:
+            df = df.merge(
+                self.care_site_relationship[
+                    ["care_site_id", "care_site_short_name"]
+                ].drop_duplicates(),
+                on="care_site_id",
+                how="left",
+            )
+        if hasattr(self, "biology_relationship"):
+            concept_codes = [
+                "{}_concept_code".format(terminology)
+                for terminology in self._standard_terminologies
+            ]
+            concept_names = [
+                "{}_concept_name".format(terminology)
+                for terminology in self._standard_terminologies
+            ]
+            if set(concept_codes).issubset(df.columns):
+                df = df.merge(
+                    self.biology_relationship[
+                        concept_codes + concept_names
+                    ].drop_duplicates(),
+                    on=concept_codes,
+                    how="left",
+                )
+        return df.reset_index(drop=True)
+
     def load(self, path=None) -> None:
         """Loads a Probe from local
 
         Parameters
         ----------
         path : str, optional
             **EXAMPLE**: `"my_folder/my_file.html"`
@@ -361,17 +339,17 @@
         visit.save(path=probe_path)
         ```
 
         """
 
         self.is_computed_probe()
 
+        if name:
+            self.name = name
         if not path:
-            if name:
-                self.name = name
             path = self._get_path()
 
         self.path = path
         save_object(self, path)
 
     def delete(self, path: str = None):
         """Delete the saved Probe instance
@@ -379,21 +357,24 @@
         Parameters
         ----------
         path : str, optional
             **EXAMPLE**: `"my_folder/my_file.html"`
         """
 
         if not path:
-            if hasattr(self, "path"):
-                path = self.path
-            else:
-                path = self._get_path()
+            path = self.path
 
         delete_object(self, path)
 
     def _get_path(self):
         base_path = CACHE_DIR / "edsteva" / "probes"
-        filename = f"{self.name.lower()}.pickle"
+        if hasattr(self, "name"):
+            filename = f"{self.name.lower()}.pickle"
+        else:
+            filename = f"{type(self).__name__.lower()}.pickle"
         return base_path / filename
 
-    def _get_name(self):
-        return type(self).__name__
+    def _reset_index(
+        self,
+    ) -> None:
+        """Reset the index to its initial state"""
+        self._index = self._cache_index.copy()
```

### Comparing `edsteva-0.1.4/edsteva/probes/condition.py` & `edsteva-0.2.0/edsteva/probes/condition/completeness_predictors/per_visit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,106 +1,223 @@
 from datetime import datetime
 from typing import Dict, List, Union
 
 import pandas as pd
 from loguru import logger
 
-from edsteva.probes.base import BaseProbe
-from edsteva.probes.utils import (
-    CARE_SITE_LEVEL_NAMES,
-    concatenate_predictor_by_level,
-    convert_table_to_pole,
-    convert_table_to_uf,
-    hospital_only,
+from edsteva.probes.utils.filter_df import convert_uf_to_pole
+from edsteva.probes.utils.prepare_df import (
     prepare_care_site,
     prepare_condition_occurrence,
     prepare_visit_detail,
     prepare_visit_occurrence,
 )
-from edsteva.utils.checks import check_conditon_source_systems, check_tables
+from edsteva.probes.utils.utils import (
+    CARE_SITE_LEVEL_NAMES,
+    concatenate_predictor_by_level,
+    hospital_only,
+    impute_missing_dates,
+)
+from edsteva.utils.checks import check_condition_source_systems, check_tables
 from edsteva.utils.framework import is_koalas, to
-from edsteva.utils.typing import Data
+from edsteva.utils.typing import Data, DataFrame
 
 
-def compute_completeness(condition_predictor):
-    partition_cols = [
-        "care_site_level",
-        "care_site_id",
-        "care_site_short_name",
-        "stay_type",
-        "diag_type",
-        "condition_type",
-        "source_system",
-        "date",
-    ]
+def compute_completeness_predictor_per_visit(
+    self,
+    data: Data,
+    care_site_relationship: pd.DataFrame,
+    start_date: datetime,
+    end_date: datetime,
+    care_site_levels: List[str],
+    stay_types: Union[str, Dict[str, str]],
+    care_site_ids: List[int],
+    extra_data: Data,
+    care_site_short_names: List[str],
+    care_site_specialties: List[str],
+    care_sites_sets: Union[str, Dict[str, str]],
+    specialties_sets: Union[str, Dict[str, str]],
+    diag_types: Union[str, Dict[str, str]],
+    condition_types: Union[str, Dict[str, str]],
+    source_systems: List[str],
+    length_of_stays: List[float],
+    **kwargs
+):
+    r"""Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
+
+    The ``per_visit`` algorithm computes $c_(t)$ the availability of claim data linked to patients' administrative stays:
+
+    $$
+    c(t) = \frac{n_{with\,condition}(t)}{n_{visit}(t)}
+    $$
+
+    Where $n_{visit}(t)$ is the number of administrative stays, $n_{with\,condition}$ the number of stays having at least one claim code (e.g. ICD-10) recorded and $t$ is the month.
+    """
+
+    self._metrics = ["c", "n_visit", "n_visit_with_condition"]
+    check_tables(data=data, required_tables=["condition_occurrence"])
+    check_condition_source_systems(source_systems=source_systems)
+    if "AREM" in source_systems and not hospital_only(
+        care_site_levels=care_site_levels
+    ):  # pragma: no cover
+        logger.info("AREM claim data are only available at hospital level")
+
+    visit_occurrence = prepare_visit_occurrence(
+        data=data,
+        start_date=start_date,
+        end_date=end_date,
+        stay_types=stay_types,
+        length_of_stays=length_of_stays,
+    )
+
+    condition_occurrence = prepare_condition_occurrence(
+        data=data,
+        extra_data=extra_data,
+        visit_occurrence=visit_occurrence,
+        source_systems=source_systems,
+        diag_types=diag_types,
+        condition_types=condition_types,
+    ).drop(columns=["condition_occurrence_id", "date"])
+
+    care_site = prepare_care_site(
+        data=data,
+        care_site_ids=care_site_ids,
+        care_site_short_names=care_site_short_names,
+        care_site_relationship=care_site_relationship,
+        care_site_specialties=care_site_specialties,
+        care_sites_sets=care_sites_sets,
+        specialties_sets=specialties_sets,
+    )
+
+    hospital_visit = get_hospital_visit(
+        condition_occurrence,
+        visit_occurrence,
+        care_site,
+    )
+    hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
+    condition_predictor_by_level = {hospital_name: hospital_visit}
+
+    # UF selection
+    if not hospital_only(care_site_levels=care_site_levels):
+        visit_detail = prepare_visit_detail(data, start_date, end_date)
+
+        uf_visit = get_uf_visit(
+            condition_occurrence=condition_occurrence,
+            visit_occurrence=visit_occurrence,
+            visit_detail=visit_detail,
+            care_site=care_site,
+        )
+        uf_name = CARE_SITE_LEVEL_NAMES["UF"]
+        condition_predictor_by_level[uf_name] = uf_visit
+
+        pole_visit = get_pole_visit(
+            uf_visit=uf_visit,
+            care_site=care_site,
+            care_site_relationship=care_site_relationship,
+        )
+        pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
+        condition_predictor_by_level[pole_name] = pole_visit
+
+    condition_predictor = concatenate_predictor_by_level(
+        predictor_by_level=condition_predictor_by_level,
+        care_site_levels=care_site_levels,
+    )
+
+    return compute_completeness(self, condition_predictor)
+
+
+def compute_completeness(
+    self,
+    condition_predictor: DataFrame,
+):
+    # Visit with diagnosis
+    partition_cols = self._index.copy() + ["date"]
     n_visit_with_condition = (
         condition_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"has_condition": "count"})
         .rename(columns={"has_condition": "n_visit_with_condition"})
     )
-    partition_cols = list(
-        set(partition_cols) - {"diag_type", "condition_type", "source_system"}
+    n_visit_with_condition = to("pandas", n_visit_with_condition)
+    n_visit_with_condition = n_visit_with_condition[
+        n_visit_with_condition.n_visit_with_condition > 0
+    ]
+    n_visit_with_condition = impute_missing_dates(
+        start_date=self.start_date,
+        end_date=self.end_date,
+        predictor=n_visit_with_condition,
+        partition_cols=partition_cols,
     )
 
+    # Visit total
+    condition_columns = ["diag_type", "condition_type", "source_system"]
+    partition_cols = list(set(partition_cols) - set(condition_columns))
     n_visit = (
         condition_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"visit_id": "nunique"})
         .rename(columns={"visit_id": "n_visit"})
     )
+    n_visit = to("pandas", n_visit)
+    n_visit = impute_missing_dates(
+        start_date=self.start_date,
+        end_date=self.end_date,
+        predictor=n_visit,
+        partition_cols=partition_cols,
+    )
 
     condition_predictor = n_visit_with_condition.merge(
         n_visit,
         on=partition_cols,
     )
 
-    condition_predictor = to("pandas", condition_predictor)
-
     condition_predictor["c"] = condition_predictor["n_visit"].where(
         condition_predictor["n_visit"] == 0,
         condition_predictor["n_visit_with_condition"] / condition_predictor["n_visit"],
     )
-    condition_predictor = condition_predictor.drop(columns=["n_visit_with_condition"])
 
     return condition_predictor
 
 
-def get_hospital_visit(condition_occurrence, visit_occurrence, care_site):
+def get_hospital_visit(
+    condition_occurrence: DataFrame,
+    visit_occurrence: DataFrame,
+    care_site: DataFrame,
+):
     condition_hospital = condition_occurrence.drop_duplicates(
         ["visit_occurrence_id", "diag_type", "condition_type", "source_system"]
     )
     condition_hospital["has_condition"] = True
     hospital_visit = visit_occurrence.merge(
         condition_hospital,
         on="visit_occurrence_id",
         how="left",
     )
     hospital_visit = hospital_visit.rename(columns={"visit_occurrence_id": "visit_id"})
     hospital_visit = hospital_visit.merge(care_site, on="care_site_id")
 
     if is_koalas(hospital_visit):
-        hospital_visit.spark.cache()
+        hospital_visit = hospital_visit.spark.cache()
 
     return hospital_visit
 
 
 def get_uf_visit(
-    condition_occurrence,
-    visit_occurrence,
-    visit_detail,
-    care_site,
-    care_site_relationship,
+    condition_occurrence: DataFrame,
+    visit_occurrence: DataFrame,
+    visit_detail: DataFrame,
+    care_site: DataFrame,
 ):  # pragma: no cover
+    visit_detail = visit_detail[visit_detail.visit_detail_type == "RUM"]
     condition_uf = (
         condition_occurrence[
             [
                 "visit_detail_id",
                 "diag_type",
                 "condition_type",
                 "source_system",
@@ -108,188 +225,60 @@
         ]
         .drop_duplicates()
         .rename(columns={"visit_detail_id": "visit_id"})
     )
     condition_uf["has_condition"] = True
 
     visit_detail = visit_detail.merge(
-        visit_occurrence[["visit_occurrence_id", "stay_type"]],
+        visit_occurrence[
+            visit_occurrence.columns.intersection(
+                set(["visit_occurrence_id", "length_of_stay", "stay_type"])
+            )
+        ],
         on="visit_occurrence_id",
     )
-    visit_detail = visit_detail.merge(
+    uf_visit = visit_detail.merge(
         condition_uf,
         on="visit_id",
         how="left",
-    )
-    visit_detail = visit_detail.drop(columns=["visit_occurrence_id"])
+    ).drop(columns=["visit_occurrence_id"])
 
-    uf_visit = convert_table_to_uf(
-        table=visit_detail,
-        table_name="visit_detail",
-        care_site_relationship=care_site_relationship,
-    )
     uf_visit = uf_visit.merge(care_site, on="care_site_id")
 
     uf_name = CARE_SITE_LEVEL_NAMES["UF"]
     uf_visit = uf_visit[uf_visit["care_site_level"] == uf_name]
 
     if is_koalas(uf_visit):
-        uf_visit.spark.cache()
+        uf_visit = uf_visit.spark.cache()
 
     return uf_visit
 
 
-def get_pole_visit(uf_visit, care_site, care_site_relationship):  # pragma: no cover
-    pole_visit = convert_table_to_pole(
-        table=uf_visit.drop(columns=["care_site_short_name", "care_site_level"]),
+def get_pole_visit(
+    uf_visit: DataFrame,
+    care_site: DataFrame,
+    care_site_relationship: DataFrame,
+):  # pragma: no cover
+    care_site_cols = list(
+        set(
+            [
+                "care_site_short_name",
+                "care_site_level",
+                "care_site_specialty",
+                "specialties_set",
+                "care_sites_set",
+            ]
+        ).intersection(uf_visit.columns)
+    )
+    pole_visit = convert_uf_to_pole(
+        table=uf_visit.drop(columns=care_site_cols),
         table_name="uf_visit",
         care_site_relationship=care_site_relationship,
     )
 
     pole_visit = pole_visit.merge(care_site, on="care_site_id")
-
     pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
     pole_visit = pole_visit[pole_visit["care_site_level"] == pole_name]
-
     if is_koalas(pole_visit):
-        pole_visit.spark.cache()
+        pole_visit = pole_visit.spark.cache()
 
     return pole_visit
-
-
-class ConditionProbe(BaseProbe):
-    r"""
-    The [``ConditionProbe``][edsteva.probes.condition.ConditionProbe] computes $c_{condition}(t)$ the availability of claim data in patients' administrative stay:
-
-    $$
-    c_{condition}(t) = \frac{n_{with\,condition}(t)}{n_{visit}(t)}
-    $$
-
-    Where $n_{visit}(t)$ is the number of administrative stays, $n_{with\,condition}$ the number of stays having at least one claim code (e.g. ICD-10) recorded and $t$ is the month.
-
-    Attributes
-    ----------
-    _index: List[str]
-        Variable from which data is grouped
-
-        **VALUE**: ``["care_site_level", "stay_type", "diag_type", "condition_type", "source_system", "care_site_id"]``
-    """
-
-    _index = [
-        "care_site_level",
-        "stay_type",
-        "diag_type",
-        "condition_type",
-        "source_system",
-        "care_site_id",
-    ]
-
-    def compute_process(
-        self,
-        data: Data,
-        care_site_relationship: pd.DataFrame,
-        extra_data: Data = None,
-        start_date: datetime = None,
-        end_date: datetime = None,
-        care_site_levels: List[str] = None,
-        stay_types: Union[str, Dict[str, str]] = None,
-        diag_types: Union[str, Dict[str, str]] = None,
-        condition_types: Union[str, Dict[str, str]] = {
-            "All": ".*",
-            "Cancer": "C",
-        },
-        source_systems: List[str] = ["ORBIS"],
-        care_site_ids: List[int] = None,
-        care_site_short_names: List[str] = None,
-    ):
-        """Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
-
-        Parameters
-        ----------
-        data : Data
-            Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]
-        care_site_relationship : pd.DataFrame
-            DataFrame computed in the [``compute()``][edsteva.probes.base.BaseProbe.compute] that gives the hierarchy of the care site structure.
-        start_date : datetime, optional
-            **EXAMPLE**: `"2019-05-01"`
-        end_date : datetime, optional
-            **EXAMPLE**: `"2021-07-01"`
-        care_site_levels : List[str], optional
-            **EXAMPLE**: `["Hospital", "Pole", "UF"]`
-        stay_types : Union[str, Dict[str, str]], optional
-            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "Urg_and_consult": "urgences|consultation"}` or `"hospitalisés"`
-        diag_types : Union[str, Dict[str, str]], optional
-            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "DP\DR": "DP|DR"}` or `"DP"`
-        condition_types : Union[str, Dict[str, str]], optional
-            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "Pulmonary_embolism": "I26"}`
-        source_systems : List[str], optional
-            **EXAMPLE**: `["AREM", "ORBIS"]`
-        care_site_ids : List[int], optional
-            **EXAMPLE**: `[8312056386, 8312027648]`
-        care_site_short_names : List[str], optional
-            **EXAMPLE**: `["HOSPITAL 1", "HOSPITAL 2"]`
-        """
-
-        check_tables(data=data, required_tables=["condition_occurrence"])
-        check_conditon_source_systems(source_systems=source_systems)
-        if "AREM" in source_systems and not hospital_only(
-            care_site_levels=care_site_levels
-        ):
-            logger.info("AREM claim data are only available at hospital level")
-
-        visit_occurrence = prepare_visit_occurrence(
-            data=data,
-            start_date=start_date,
-            end_date=end_date,
-            stay_types=stay_types,
-        )
-
-        condition_occurrence = prepare_condition_occurrence(
-            data=data,
-            extra_data=extra_data,
-            visit_occurrence=visit_occurrence,
-            source_systems=source_systems,
-            diag_types=diag_types,
-            condition_types=condition_types,
-        )
-
-        care_site = prepare_care_site(
-            data=data,
-            care_site_ids=care_site_ids,
-            care_site_short_names=care_site_short_names,
-            care_site_relationship=care_site_relationship,
-        )
-
-        hospital_visit = get_hospital_visit(
-            condition_occurrence,
-            visit_occurrence,
-            care_site,
-        )
-        hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
-        condition_predictor_by_level = {hospital_name: hospital_visit}
-
-        # UF selection
-        if not hospital_only(care_site_levels=care_site_levels):
-            visit_detail = prepare_visit_detail(
-                data, start_date, end_date, visit_detail_type="RUM"
-            )
-
-            uf_visit = get_uf_visit(
-                condition_occurrence,
-                visit_occurrence,
-                visit_detail,
-                care_site,
-                care_site_relationship,
-            )
-            uf_name = CARE_SITE_LEVEL_NAMES["UF"]
-            condition_predictor_by_level[uf_name] = uf_visit
-
-            pole_visit = get_pole_visit(uf_visit, care_site, care_site_relationship)
-            pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
-            condition_predictor_by_level[pole_name] = pole_visit
-
-        condition_predictor = concatenate_predictor_by_level(
-            predictor_by_level=condition_predictor_by_level,
-            care_site_levels=care_site_levels,
-        )
-
-        return compute_completeness(condition_predictor)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edsteva-0.1.4/edsteva/probes/note.py` & `edsteva-0.2.0/edsteva/probes/note/completeness_predictors/per_visit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,259 +1,267 @@
 from datetime import datetime
 from typing import Dict, List, Union
 
 import pandas as pd
+from loguru import logger
 
-from edsteva.probes.base import BaseProbe
-from edsteva.probes.utils import (
-    CARE_SITE_LEVEL_NAMES,
-    add_note_care_site,
-    concatenate_predictor_by_level,
-    convert_table_to_pole,
-    convert_table_to_uf,
-    hospital_only,
+from edsteva.probes.utils.filter_df import convert_uf_to_pole
+from edsteva.probes.utils.prepare_df import (
     prepare_care_site,
     prepare_note,
+    prepare_note_care_site,
     prepare_visit_detail,
     prepare_visit_occurrence,
 )
+from edsteva.probes.utils.utils import (
+    CARE_SITE_LEVEL_NAMES,
+    concatenate_predictor_by_level,
+    hospital_only,
+    impute_missing_dates,
+)
 from edsteva.utils.checks import check_tables
 from edsteva.utils.framework import is_koalas, to
-from edsteva.utils.typing import Data
+from edsteva.utils.typing import Data, DataFrame
+
+
+def compute_completeness_predictor_per_visit(
+    self,
+    data: Data,
+    care_site_relationship: pd.DataFrame,
+    start_date: datetime,
+    end_date: datetime,
+    care_site_levels: List[str],
+    stay_types: Union[str, Dict[str, str]],
+    care_site_ids: List[int],
+    care_site_short_names: List[str],
+    care_site_specialties: List[str],
+    care_sites_sets: Union[str, Dict[str, str]],
+    specialties_sets: Union[str, Dict[str, str]],
+    extra_data: Data,
+    length_of_stays: List[float],
+    note_types: Union[str, Dict[str, str]],
+    **kwargs
+):
+    r"""Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
+
+    The ``per_visit`` algorithm computes $c_(t)$ the availability of clinical documents linked to patients' administrative stays:
+
+    $$
+    c(t) = \frac{n_{with\,doc}(t)}{n_{visit}(t)}
+    $$
+
+    Where $n_{visit}(t)$ is the number of administrative stays, $n_{with\,doc}$ the number of visits having at least one document and $t$ is the month.
+    """
+
+    self._metrics = ["c", "n_visit", "n_visit_with_note"]
+    check_tables(data=data, required_tables=["note"])
+
+    visit_occurrence = prepare_visit_occurrence(
+        data=data,
+        start_date=start_date,
+        end_date=end_date,
+        stay_types=stay_types,
+        length_of_stays=length_of_stays,
+    )
+
+    care_site = prepare_care_site(
+        data=data,
+        care_site_ids=care_site_ids,
+        care_site_short_names=care_site_short_names,
+        care_site_relationship=care_site_relationship,
+        care_site_specialties=care_site_specialties,
+        care_sites_sets=care_sites_sets,
+        specialties_sets=specialties_sets,
+    )
+
+    note = prepare_note(data, note_types)
 
+    hospital_visit = get_hospital_visit(note, visit_occurrence, care_site)
+    hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
+    note_predictor_by_level = {hospital_name: hospital_visit}
+
+    # UF selection
+    if not hospital_only(care_site_levels=care_site_levels):
+        if extra_data:  # pragma: no cover
+            visit_detail = prepare_visit_detail(data, start_date, end_date)
+
+            uf_visit, uc_visit, uh_visit = get_visit_detail(
+                extra_data=extra_data,
+                note=note,
+                visit_occurrence=visit_occurrence,
+                visit_detail=visit_detail,
+                care_site=care_site,
+            )
+            uf_name = CARE_SITE_LEVEL_NAMES["UF"]
+            note_predictor_by_level[uf_name] = uf_visit
+            uc_name = CARE_SITE_LEVEL_NAMES["UC"]
+            note_predictor_by_level[uc_name] = uc_visit
+            uh_name = CARE_SITE_LEVEL_NAMES["UH"]
+            note_predictor_by_level[uh_name] = uh_visit
+
+            pole_visit = get_pole_visit(uf_visit, care_site, care_site_relationship)
+            pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
+            note_predictor_by_level[pole_name] = pole_visit
+        else:
+            logger.info("Note data are only available at hospital level")
+            care_site_levels = ["Hospital"]
+
+    # Concatenate all predictors
+    note_predictor = concatenate_predictor_by_level(
+        predictor_by_level=note_predictor_by_level,
+        care_site_levels=care_site_levels,
+    )
+
+    if is_koalas(note_predictor):
+        note_predictor.spark.cache()
+
+    return compute_completeness(self, note_predictor)
 
-def compute_completeness(note_predictor):
-    partition_cols = [
-        "care_site_level",
-        "care_site_id",
-        "care_site_short_name",
-        "stay_type",
-        "note_type",
-        "date",
-    ]
+
+def compute_completeness(
+    self,
+    note_predictor: DataFrame,
+):
+    # Visit with note
+    partition_cols = self._index.copy() + ["date"]
     n_visit_with_note = (
         note_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"has_note": "count"})
         .rename(columns={"has_note": "n_visit_with_note"})
     )
+    n_visit_with_note = to("pandas", n_visit_with_note)
+    n_visit_with_note = n_visit_with_note[n_visit_with_note.n_visit_with_note > 0]
+    n_visit_with_note = impute_missing_dates(
+        start_date=self.start_date,
+        end_date=self.end_date,
+        predictor=n_visit_with_note,
+        partition_cols=partition_cols,
+    )
 
-    partition_cols = list(set(partition_cols) - {"note_type"})
+    # Visit total
+    note_columns = ["note_type"]
+    partition_cols = list(set(partition_cols) - set(note_columns))
     n_visit = (
         note_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"visit_id": "nunique"})
         .rename(columns={"visit_id": "n_visit"})
     )
-
+    n_visit = to("pandas", n_visit)
+    n_visit = impute_missing_dates(
+        start_date=self.start_date,
+        end_date=self.end_date,
+        predictor=n_visit,
+        partition_cols=partition_cols,
+    )
     note_predictor = n_visit_with_note.merge(
         n_visit,
         on=partition_cols,
     )
 
-    note_predictor = to("pandas", note_predictor)
-
+    # Compute completeness
     note_predictor["c"] = note_predictor["n_visit"].where(
         note_predictor["n_visit"] == 0,
         note_predictor["n_visit_with_note"] / note_predictor["n_visit"],
     )
-    note_predictor = note_predictor.drop(columns=["n_visit_with_note"])
 
     return note_predictor
 
 
-def get_hospital_visit(note, visit_occurrence, care_site):
+def get_hospital_visit(
+    note: DataFrame,
+    visit_occurrence: DataFrame,
+    care_site: DataFrame,
+):
     note_hospital = note[["visit_occurrence_id", "note_type"]].drop_duplicates()
     note_hospital["has_note"] = True
     hospital_visit = visit_occurrence.merge(
         note_hospital, on="visit_occurrence_id", how="left"
     )
     hospital_visit = hospital_visit.rename(columns={"visit_occurrence_id": "visit_id"})
     hospital_visit = hospital_visit.merge(care_site, on="care_site_id")
     if is_koalas(hospital_visit):
-        hospital_visit.spark.cache()
+        hospital_visit = hospital_visit.spark.cache()
 
     return hospital_visit
 
 
-def get_uf_visit(
-    extra_data,
-    note,
-    visit_occurrence,
-    visit_detail,
-    care_site,
-    care_site_relationship,
+def get_visit_detail(
+    extra_data: Data,
+    note: DataFrame,
+    visit_occurrence: DataFrame,
+    visit_detail: DataFrame,
+    care_site: DataFrame,
 ):  # pragma: no cover
-    note = add_note_care_site(extra_data=extra_data, note=note)
-    note_uf = note[
-        ["visit_occurrence_id", "note_type", "care_site_id"]
-    ].drop_duplicates()
-    note_uf["has_note"] = True
-
     visit_detail = visit_detail.merge(
-        visit_occurrence[["visit_occurrence_id", "stay_type"]],
+        visit_occurrence[
+            visit_occurrence.columns.intersection(
+                set(["visit_occurrence_id", "length_of_stay", "stay_type"])
+            )
+        ],
         on="visit_occurrence_id",
     )
-    visit_detail = visit_detail.merge(
-        note_uf,
+
+    note_detail = prepare_note_care_site(extra_data=extra_data, note=note)
+    note_detail = note_detail[
+        ["visit_occurrence_id", "note_type", "care_site_id"]
+    ].drop_duplicates()
+    note_detail["has_note"] = True
+    note_detail = visit_detail.merge(
+        note_detail,
         on=["visit_occurrence_id", "care_site_id"],
         how="left",
-    )
-    visit_detail = visit_detail.drop(columns="visit_occurrence_id")
+    ).drop(columns="visit_occurrence_id")
 
-    uf_visit = convert_table_to_uf(
-        table=visit_detail,
-        table_name="visit_detail",
-        care_site_relationship=care_site_relationship,
-    )
-    uf_visit = uf_visit.merge(care_site, on="care_site_id")
+    note_detail = note_detail.merge(care_site, on="care_site_id")
 
     uf_name = CARE_SITE_LEVEL_NAMES["UF"]
-    uf_visit = uf_visit[uf_visit["care_site_level"] == uf_name]
-
-    if is_koalas(uf_visit):
-        uf_visit.spark.cache()
-
-    return uf_visit
-
-
-def get_pole_visit(uf_visit, care_site, care_site_relationship):  # pragma: no cover
-    pole_visit = convert_table_to_pole(
-        table=uf_visit.drop(columns=["care_site_short_name", "care_site_level"]),
+    uf_visit = note_detail[note_detail["care_site_level"] == uf_name]
+    uc_name = CARE_SITE_LEVEL_NAMES["UC"]
+    uc_visit = note_detail[note_detail["care_site_level"] == uc_name]
+    uh_name = CARE_SITE_LEVEL_NAMES["UH"]
+    uh_visit = note_detail[note_detail["care_site_level"] == uh_name]
+
+    if is_koalas(note_detail):
+        uf_visit = uf_visit.spark.cache()
+        uc_visit = uc_visit.spark.cache()
+        uh_visit = uh_visit.spark.cache()
+
+    return uf_visit, uc_visit, uh_visit
+
+
+def get_pole_visit(
+    uf_visit: DataFrame,
+    care_site: DataFrame,
+    care_site_relationship: DataFrame,
+):  # pragma: no cover
+    care_site_cols = list(
+        set(
+            [
+                "care_site_short_name",
+                "care_site_level",
+                "care_site_specialty",
+                "specialties_set",
+                "care_sites_set",
+            ]
+        ).intersection(uf_visit.columns)
+    )
+    pole_visit = convert_uf_to_pole(
+        table=uf_visit.drop(columns=care_site_cols),
         table_name="uf_visit",
         care_site_relationship=care_site_relationship,
     )
 
     pole_visit = pole_visit.merge(care_site, on="care_site_id")
-
     pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
     pole_visit = pole_visit[pole_visit["care_site_level"] == pole_name]
-
     if is_koalas(pole_visit):
-        pole_visit.spark.cache()
+        pole_visit = pole_visit.spark.cache()
 
     return pole_visit
-
-
-class NoteProbe(BaseProbe):
-    r"""
-    The ``NoteProbe`` computes $c(t)$ the availability of clinical documents linked to patients' administrative visit:
-
-    $$
-    c(t) = \frac{n_{with\,doc}(t)}{n_{visit}(t)}
-    $$
-
-    Where $n_{visit}(t)$ is the number of visits, $n_{with\,doc}$ the number of visits having at least one document and $t$ is the month.
-
-    Attributes
-    ----------
-    _index: List[str]
-        Variable from which data is grouped
-
-        **VALUE**: ``["care_site_level", "stay_type", "note_type", "care_site_id"]``
-    """
-
-    _index = ["care_site_level", "stay_type", "note_type", "care_site_id"]
-
-    def compute_process(
-        self,
-        data: Data,
-        care_site_relationship: pd.DataFrame,
-        extra_data: Data = None,
-        start_date: datetime = None,
-        end_date: datetime = None,
-        care_site_levels: List[str] = None,
-        care_site_short_names: List[str] = None,
-        stay_types: Union[str, Dict[str, str]] = None,
-        note_types: Union[str, Dict[str, str]] = {
-            "All": ".*",
-            "Urgence": "urge",
-            "Ordonnance": "ordo",
-            "CRH": "crh",
-        },
-        care_site_ids: List[int] = None,
-    ):
-        """Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
-
-        Parameters
-        ----------
-        data : Data
-            Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]
-        care_site_relationship : pd.DataFrame
-            DataFrame computed in the [``compute()``][edsteva.probes.base.BaseProbe.compute] that gives the hierarchy of the care site structure.
-        extra_data : Data, optional
-            Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]. This is not OMOP-standardized data but data needed to associate note with UF and Pole. If not provided, it will only compute the predictor for hospitals.
-        start_date : datetime, optional
-            **EXAMPLE**: `"2019-05-01"`
-        end_date : datetime, optional
-            **EXAMPLE**: `"2021-07-01"`
-        care_site_levels : List[str], optional
-            **EXAMPLE**: `["Hospital", "Pole", "UF"]`
-        care_site_short_names : List[str], optional
-            **EXAMPLE**: `["HOSPITAL 1", "HOSPITAL 2"]`
-        stay_types : Union[str, Dict[str, str]], optional
-            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "Urg_and_consult": "urgences|consultation"}` or `"hospitalisés`
-        note_types : Union[str, Dict[str, str]], optional
-        care_site_ids : List[int], optional
-            **EXAMPLE**: `[8312056386, 8312027648]`
-        """
-        check_tables(data=data, required_tables=["note"])
-
-        visit_occurrence = prepare_visit_occurrence(
-            data,
-            start_date,
-            end_date,
-            stay_types,
-        )
-
-        care_site = prepare_care_site(
-            data,
-            care_site_ids,
-            care_site_short_names,
-            care_site_relationship,
-        )
-
-        note = prepare_note(data, note_types)
-
-        hospital_visit = get_hospital_visit(note, visit_occurrence, care_site)
-        hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
-        note_predictor_by_level = {hospital_name: hospital_visit}
-
-        # UF selection
-        if not hospital_only(care_site_levels=care_site_levels) and extra_data:
-            visit_detail = prepare_visit_detail(data, start_date, end_date)
-
-            uf_visit = get_uf_visit(
-                extra_data,
-                note,
-                visit_occurrence,
-                visit_detail,
-                care_site,
-                care_site_relationship,
-            )
-            uf_name = CARE_SITE_LEVEL_NAMES["UF"]
-            note_predictor_by_level[uf_name] = uf_visit
-
-            pole_visit = get_pole_visit(uf_visit, care_site, care_site_relationship)
-            pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
-            note_predictor_by_level[pole_name] = pole_visit
-
-        # Concatenate all predictors
-        note_predictor = concatenate_predictor_by_level(
-            predictor_by_level=note_predictor_by_level,
-            care_site_levels=care_site_levels,
-        )
-
-        note_predictor = note_predictor.drop_duplicates(
-            ["visit_id", "care_site_id", "stay_type", "note_type", "date"]
-        )
-
-        if is_koalas(note_predictor):
-            note_predictor.spark.cache()
-
-        return compute_completeness(note_predictor)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edsteva-0.1.4/edsteva/probes/visit.py` & `edsteva-0.2.0/edsteva/probes/visit/completeness_predictors/per_visit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,277 @@
 from datetime import datetime
 from typing import Dict, List, Union
 
 import pandas as pd
 
-from edsteva.probes.base import BaseProbe
-from edsteva.probes.utils import (
-    CARE_SITE_LEVEL_NAMES,
-    concatenate_predictor_by_level,
-    convert_table_to_pole,
-    convert_table_to_uf,
-    hospital_only,
+from edsteva.probes.utils.filter_df import convert_uf_to_pole
+from edsteva.probes.utils.prepare_df import (
     prepare_care_site,
     prepare_visit_detail,
     prepare_visit_occurrence,
 )
+from edsteva.probes.utils.utils import (
+    CARE_SITE_LEVEL_NAMES,
+    VISIT_DETAIL_TYPE,
+    concatenate_predictor_by_level,
+    hospital_only,
+    impute_missing_dates,
+)
 from edsteva.utils.framework import is_koalas, to
-from edsteva.utils.typing import Data
+from edsteva.utils.typing import Data, DataFrame
 
 
-def compute_completeness(visit_predictor):
-    partition_cols = [
-        "care_site_level",
-        "care_site_id",
-        "care_site_short_name",
-        "stay_type",
-        "date",
-    ]
+def compute_completeness_predictor_per_visit(
+    self,
+    data: Data,
+    care_site_relationship: pd.DataFrame,
+    start_date: datetime,
+    end_date: datetime,
+    care_site_levels: List[str],
+    stay_types: Union[str, Dict[str, str]],
+    care_site_ids: List[int],
+    care_site_short_names: List[str],
+    care_site_specialties: List[str],
+    care_sites_sets: Union[str, Dict[str, str]],
+    specialties_sets: Union[str, Dict[str, str]],
+    length_of_stays: List[float],
+    **kwargs
+):
+    r"""Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
+
+    The ``per_visit`` algorithm computes $c_(t)$ the availability of administrative data related to visits for each care site according to time:
+
+    $$
+    c(t) = \frac{n_{visit}(t)}{n_{max}}
+    $$
+
+    Where $n_{visit}(t)$ is the number of administrative stays, $t$ is the month and $n_{max} = \max_{t}(n_{visit}(t))$.
+    """
+    self._metrics = ["c", "n_visit"]
+    visit_occurrence = prepare_visit_occurrence(
+        data=data,
+        start_date=start_date,
+        end_date=end_date,
+        stay_types=stay_types,
+        length_of_stays=length_of_stays,
+    )
+
+    care_site = prepare_care_site(
+        data=data,
+        care_site_ids=care_site_ids,
+        care_site_short_names=care_site_short_names,
+        care_site_specialties=care_site_specialties,
+        care_site_relationship=care_site_relationship,
+        specialties_sets=specialties_sets,
+        care_sites_sets=care_sites_sets,
+    )
+
+    hospital_visit = get_hospital_visit(
+        visit_occurrence,
+        care_site,
+    )
+    hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
+    visit_predictor_by_level = {hospital_name: hospital_visit}
+
+    if not hospital_only(care_site_levels=care_site_levels):
+        visit_detail = prepare_visit_detail(data, start_date, end_date)
+
+        uf_name = CARE_SITE_LEVEL_NAMES["UF"]
+        uf_visit = get_uf_visit(
+            visit_occurrence,
+            visit_detail,
+            care_site,
+        )
+        visit_predictor_by_level[uf_name] = uf_visit
+
+        uc_name = CARE_SITE_LEVEL_NAMES["UC"]
+        uc_visit = get_uc_visit(
+            visit_occurrence,
+            visit_detail,
+            care_site,
+        )
+        visit_predictor_by_level[uc_name] = uc_visit
+
+        uh_name = CARE_SITE_LEVEL_NAMES["UH"]
+        uh_visit = get_uh_visit(
+            visit_occurrence,
+            visit_detail,
+            care_site,
+        )
+        visit_predictor_by_level[uh_name] = uh_visit
+
+        pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
+        pole_visit = get_pole_visit(
+            uf_visit,
+            care_site,
+            care_site_relationship,
+        )
+        visit_predictor_by_level[pole_name] = pole_visit
+
+    visit_predictor = concatenate_predictor_by_level(
+        predictor_by_level=visit_predictor_by_level,
+        care_site_levels=care_site_levels,
+    )
+
+    return compute_completeness(self, visit_predictor)
+
+
+def compute_completeness(
+    self,
+    visit_predictor: DataFrame,
+):
+    partition_cols = self._index.copy() + ["date"]
+
     n_visit = (
         visit_predictor.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
         )
         .agg({"visit_id": "nunique"})
         .rename(columns={"visit_id": "n_visit"})
     )
-
     n_visit = to("pandas", n_visit)
+    n_visit = impute_missing_dates(
+        start_date=self.start_date,
+        end_date=self.end_date,
+        predictor=n_visit,
+        partition_cols=partition_cols,
+    )
 
     partition_cols = list(set(partition_cols) - {"date"})
-    q_99_visit = (
+    max_n_visit = (
         n_visit.groupby(
             partition_cols,
             as_index=False,
             dropna=False,
-        )[["n_visit"]]
-        .quantile(q=0.99)
-        .rename(columns={"n_visit": "q_99_visit"})
+        )
+        .agg({"n_visit": "max"})
+        .rename(columns={"n_visit": "max_n_visit"})
     )
 
     visit_predictor = n_visit.merge(
-        q_99_visit,
+        max_n_visit,
         on=partition_cols,
     )
 
-    visit_predictor["c"] = visit_predictor["q_99_visit"].where(
-        visit_predictor["q_99_visit"] == 0,
-        visit_predictor["n_visit"] / visit_predictor["q_99_visit"],
+    visit_predictor["c"] = visit_predictor["max_n_visit"].where(
+        visit_predictor["max_n_visit"] == 0,
+        visit_predictor["n_visit"] / visit_predictor["max_n_visit"],
     )
-    visit_predictor = visit_predictor.drop(columns="q_99_visit")
+    visit_predictor = visit_predictor.drop(columns="max_n_visit")
 
     return visit_predictor
 
 
-def get_hospital_visit(visit_occurrence, care_site):
+def get_hospital_visit(
+    visit_occurrence: DataFrame,
+    care_site: DataFrame,
+):
     hospital_visit = visit_occurrence.rename(
         columns={"visit_occurrence_id": "visit_id"}
     )
-    hospital_visit = hospital_visit.merge(care_site, on="care_site_id")
 
+    hospital_visit = hospital_visit.merge(care_site, on="care_site_id")
+    hospital_visit = hospital_visit[
+        hospital_visit["care_site_level"] == CARE_SITE_LEVEL_NAMES["Hospital"]
+    ]
     if is_koalas(hospital_visit):
-        hospital_visit.spark.cache()
+        hospital_visit = hospital_visit.spark.cache()
 
     return hospital_visit
 
 
-def get_uf_visit(visit_occurrence, visit_detail, care_site, care_site_relationship):
-    visit_detail = visit_detail.merge(
-        visit_occurrence[["visit_occurrence_id", "stay_type"]],
+def get_uf_visit(
+    visit_occurrence: DataFrame,
+    visit_detail: DataFrame,
+    care_site: DataFrame,
+):
+    uf_visit = visit_detail[visit_detail.visit_detail_type == VISIT_DETAIL_TYPE["UF"]]
+    uf_visit = uf_visit.merge(
+        visit_occurrence[
+            visit_occurrence.columns.intersection(
+                set(["visit_occurrence_id", "length_of_stay", "stay_type"])
+            )
+        ],
         on="visit_occurrence_id",
     ).drop(columns="visit_occurrence_id")
-
-    uf_visit = convert_table_to_uf(
-        table=visit_detail,
-        table_name="visit_detail",
-        care_site_relationship=care_site_relationship,
-    )
     uf_visit = uf_visit.merge(care_site, on="care_site_id")
     uf_visit = uf_visit[uf_visit["care_site_level"] == CARE_SITE_LEVEL_NAMES["UF"]]
     if is_koalas(uf_visit):
-        uf_visit.spark.cache()
+        uf_visit = uf_visit.spark.cache()
 
     return uf_visit
 
 
-def get_pole_visit(uf_visit, care_site, care_site_relationship):
-    pole_visit = convert_table_to_pole(
-        table=uf_visit.drop(columns=["care_site_short_name", "care_site_level"]),
+def get_uc_visit(
+    visit_occurrence: DataFrame,
+    visit_detail: DataFrame,
+    care_site: DataFrame,
+):
+    uc_visit = visit_detail[visit_detail.visit_detail_type == VISIT_DETAIL_TYPE["UC"]]
+    uc_visit = uc_visit.merge(
+        visit_occurrence[
+            visit_occurrence.columns.intersection(
+                set(["visit_occurrence_id", "length_of_stay", "stay_type"])
+            )
+        ],
+        on="visit_occurrence_id",
+    ).drop(columns="visit_occurrence_id")
+    uc_visit = uc_visit.merge(care_site, on="care_site_id")
+    uc_visit = uc_visit[uc_visit["care_site_level"] == CARE_SITE_LEVEL_NAMES["UC"]]
+    if is_koalas(uc_visit):
+        uc_visit = uc_visit.spark.cache()
+
+    return uc_visit
+
+
+def get_uh_visit(
+    visit_occurrence: DataFrame,
+    visit_detail: DataFrame,
+    care_site: DataFrame,
+):
+    uh_visit = visit_detail[visit_detail.visit_detail_type == VISIT_DETAIL_TYPE["UH"]]
+    uh_visit = uh_visit.merge(
+        visit_occurrence[
+            visit_occurrence.columns.intersection(
+                set(["visit_occurrence_id", "length_of_stay", "stay_type"])
+            )
+        ],
+        on="visit_occurrence_id",
+    ).drop(columns="visit_occurrence_id")
+    uh_visit = uh_visit.merge(care_site, on="care_site_id")
+    uh_visit = uh_visit[uh_visit["care_site_level"] == CARE_SITE_LEVEL_NAMES["UH"]]
+    if is_koalas(uh_visit):
+        uh_visit = uh_visit.spark.cache()
+
+    return uh_visit
+
+
+def get_pole_visit(
+    uf_visit: DataFrame,
+    care_site: DataFrame,
+    care_site_relationship: DataFrame,
+):
+    care_site_cols = list(
+        set(
+            [
+                "care_site_short_name",
+                "care_site_level",
+                "care_site_specialty",
+                "specialties_set",
+                "care_sites_set",
+            ]
+        ).intersection(uf_visit.columns)
+    )
+    pole_visit = convert_uf_to_pole(
+        table=uf_visit.drop(columns=care_site_cols),
         table_name="uf_visit",
         care_site_relationship=care_site_relationship,
     )
-
     pole_visit = pole_visit.merge(care_site, on="care_site_id")
-    pole_visit = pole_visit[
-        pole_visit["care_site_level"] == CARE_SITE_LEVEL_NAMES["Pole"]
-    ]
+    pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
+    pole_visit = pole_visit[pole_visit["care_site_level"] == pole_name]
     if is_koalas(pole_visit):
-        pole_visit.spark.cache()
+        pole_visit = pole_visit.spark.cache()
 
     return pole_visit
-
-
-class VisitProbe(BaseProbe):
-    r"""
-    The ``VisitProbe`` computes $c_(t)$ the availability of administrative data related to visits for each care site according to time:
-
-    $$
-    c(t) = \frac{n_{visit}(t)}{n_{99}}
-    $$
-
-    Where $n_{visit}(t)$ is the number of visits, $n_{99}$ is the $99^{th}$ percentile of visits and $t$ is the month.
-
-    Attributes
-    ----------
-    _index: List[str]
-        Variable from which data is grouped
-
-        **VALUE**: ``["care_site_level", "stay_type", "care_site_id"]``
-    """
-
-    _index = ["care_site_level", "stay_type", "care_site_id"]
-
-    def compute_process(
-        self,
-        data: Data,
-        care_site_relationship: pd.DataFrame,
-        start_date: datetime = None,
-        end_date: datetime = None,
-        care_site_levels: List[str] = None,
-        stay_types: Union[str, Dict[str, str]] = None,
-        care_site_ids: List[int] = None,
-        care_site_short_names: List[str] = None,
-    ):
-        """Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
-
-        Parameters
-        ----------
-        data : Data
-            Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]
-        care_site_relationship : pd.DataFrame
-            DataFrame computed in the [``compute()``][edsteva.probes.base.BaseProbe.compute] that gives the hierarchy of the care site structure.
-        start_date : datetime, optional
-            **EXAMPLE**: `"2019-05-01"`
-        end_date : datetime, optional
-            **EXAMPLE**: `"2021-07-01"`
-        care_site_levels : List[str], optional
-            **EXAMPLE**: `["Hospital", "Pole", "UF"]`
-        stay_types : Union[str, Dict[str, str]], optional
-            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "Urg_and_consult": "urgences|consultation"}` or `"hospitalisés`
-        care_site_ids : List[int], optional
-            **EXAMPLE**: `[8312056386, 8312027648]`
-        care_site_short_names : List[str], optional
-            **EXAMPLE**: `["HOSPITAL 1", "HOSPITAL 2"]`
-        """
-
-        visit_occurrence = prepare_visit_occurrence(
-            data,
-            start_date,
-            end_date,
-            stay_types,
-        )
-
-        care_site = prepare_care_site(
-            data,
-            care_site_ids,
-            care_site_short_names,
-            care_site_relationship,
-        )
-
-        hospital_visit = get_hospital_visit(
-            visit_occurrence,
-            care_site,
-        )
-        hospital_name = CARE_SITE_LEVEL_NAMES["Hospital"]
-        visit_predictor_by_level = {hospital_name: hospital_visit}
-
-        if not hospital_only(care_site_levels=care_site_levels):
-            visit_detail = prepare_visit_detail(data, start_date, end_date)
-
-            uf_name = CARE_SITE_LEVEL_NAMES["UF"]
-            uf_visit = get_uf_visit(
-                visit_occurrence,
-                visit_detail,
-                care_site,
-                care_site_relationship,
-            )
-            visit_predictor_by_level[uf_name] = uf_visit
-
-            pole_name = CARE_SITE_LEVEL_NAMES["Pole"]
-            pole_visit = get_pole_visit(
-                uf_visit,
-                care_site,
-                care_site_relationship,
-            )
-            visit_predictor_by_level[pole_name] = pole_visit
-
-        visit_predictor = concatenate_predictor_by_level(
-            predictor_by_level=visit_predictor_by_level,
-            care_site_levels=care_site_levels,
-        )
-
-        return compute_completeness(visit_predictor)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edsteva-0.1.4/edsteva/utils/checks.py` & `edsteva-0.2.0/edsteva/utils/checks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-from typing import List, Union
+from typing import List
 
 from edsteva.utils.typing import Data, DataFrame
 
 
 class MissingColumnError(Exception):
     """Exception raised when a concept is missing"""
 
     def __init__(
         self,
-        required_columns: Union[List, dict],
+        required_columns: List,
         df_name: str = "",
     ):
-        if isinstance(required_columns, dict):
-            to_display_per_column = [
-                f"- {column} ({msg})" if msg is not None else f"{column}"
-                for column, msg in required_columns.items()
-            ]
-        else:
-            to_display_per_column = [f"- {column}" for column in required_columns]
+        to_display_per_column = [f"- {column}" for column in required_columns]
         str_to_display = "\n".join(to_display_per_column)
 
         if df_name:
             df_name = f" {df_name} "
         message = (
             f"The{df_name}DataFrame is missing some columns, "
             "namely:\n"
@@ -32,23 +26,17 @@
 
 
 class MissingTableError(Exception):
     """Exception raised when a table is missing in the Data"""
 
     def __init__(
         self,
-        required_tables: Union[List, dict],
+        required_tables: List,
     ):
-        if isinstance(required_tables, dict):
-            to_display_per_concept = [
-                f"- {concept} ({msg})" if msg is not None else f"{concept}"
-                for concept, msg in required_tables.items()
-            ]
-        else:
-            to_display_per_concept = [f"- {concept}" for concept in required_tables]
+        to_display_per_concept = [f"- {concept}" for concept in required_tables]
         str_to_display = "\n".join(to_display_per_concept)
 
         message = f"Data is missing some tables, namely:\n {str_to_display}"
 
         super().__init__(message)
 
 
@@ -67,15 +55,15 @@
             raise MissingTableError(missing_tables)
     else:
         raise AttributeError(
             "data should be a Data type please refer to this [page](https://aphp.github.io/edsteva/latest/components/loading_data/)"
         )
 
 
-def check_conditon_source_systems(
+def check_condition_source_systems(
     source_systems: List[str], valid_source_systems: List[str] = ["AREM", "ORBIS"]
 ):
     if source_systems and isinstance(source_systems, list):
         valid = False
         for valid_source_system in valid_source_systems:
             if valid_source_system in source_systems:
                 valid = True
@@ -83,10 +71,10 @@
         if not valid:
             raise AttributeError(
                 "Source systems only accept {}".format(valid_source_systems)
             )
     else:
         raise AttributeError(
             "Source systems must be a non empty list and not {}".format(
-                type(source_systems)
+                type(source_systems).__name__
             )
         )
```

### Comparing `edsteva-0.1.4/edsteva/viz/dashboards/estimates_dashboard.py` & `edsteva-0.2.0/edsteva/viz/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,466 +1,484 @@
-import uuid
+import os
+from datetime import datetime
 from functools import reduce
+from math import ceil, floor, log10
+from pathlib import Path
+from typing import Dict, List, Union
 
 import altair as alt
-from IPython.display import HTML, display
+import pandas as pd
+from loguru import logger
 
-from edsteva.models.base import BaseModel
-from edsteva.probes.base import BaseProbe
-from edsteva.probes.utils import CARE_SITE_LEVEL_NAMES
-from edsteva.viz.utils import filter_predictor, round_it, save_html, scale_it
+from edsteva.probes.utils.filter_df import filter_table_by_date
+from edsteva.probes.utils.utils import CARE_SITE_LEVEL_NAMES
 
 
-def estimates_dashboard(
-    probe: BaseProbe,
-    fitted_model: BaseModel,
-    care_site_level: str = CARE_SITE_LEVEL_NAMES["Hospital"],
-    save_path: str = None,
-    labelFontSize: float = 12,
-    titleFontSize: float = 13,
+def generate_main_chart(
+    base: alt.Chart,
+    main_chart_config: Dict[str, str],
+    index_selection: alt.SelectionParameter = None,
+    index_fields: List[str] = None,
+    x_axis_title: str = None,
+    y_axis_title: str = None,
 ):
-    r"""Displays an interactive chart with:
+    if x_axis_title:
+        main_chart_config["encode"]["x"]["title"] = x_axis_title
+    if y_axis_title:
+        main_chart_config["encode"]["y"]["title"] = y_axis_title
+    if index_fields:
+        base = base.transform_fold(index_fields, as_=["index", "value"])
+        if "aggregates" in main_chart_config.keys():
+            for aggregate in main_chart_config["aggregates"]:
+                base = base.transform_joinaggregate(**aggregate)
+        if "calculates" in main_chart_config.keys():
+            for calculate in main_chart_config["calculates"]:
+                base = base.transform_calculate(**calculate)
+        if "filters" in main_chart_config.keys():
+            for filter in main_chart_config["filters"]:
+                base = base.transform_filter(**filter)
+        main_chart = base.encode(**main_chart_config["encode"])
+        if index_selection:
+            main_chart = main_chart.transform_filter(index_selection)
+    else:
+        main_chart = base.encode(
+            x=main_chart_config["encode"]["x"],
+            y=main_chart_config["encode"]["y"],
+        )
+
+    return main_chart.properties(**main_chart_config["properties"])
+
+
+def generate_model_line(
+    main_chart: alt.Chart,
+    model_line_config: Dict[str, str],
+):
+    model_line = main_chart.mark_line(**model_line_config["mark_line"])
+    if "aggregates" in model_line_config.keys():
+        for aggregate in model_line_config["aggregates"]:
+            model_line = model_line.transform_joinaggregate(**aggregate)
+    if "calculates" in model_line_config.keys():
+        for calculate in model_line_config["calculates"]:
+            model_line = model_line.transform_calculate(**calculate)
+    if "filters" in model_line_config.keys():
+        for filter in model_line_config["filters"]:
+            model_line = model_line.transform_filter(**filter)
+    model_line = model_line.encode(**model_line_config["encode"])
+    model_line = add_selection_on_legend(model_line)
+    return model_line
+
+
+def generate_error_line(
+    main_chart: alt.Chart,
+    error_line_config: Dict[str, str],
+):
+    error_line = main_chart.mark_errorband(
+        **error_line_config["mark_errorband"]
+    ).encode(**error_line_config["encode"])
+    error_line = add_selection_on_legend(
+        error_line, opacity_true=0.3, opacity_false=0.05
+    )
+    return error_line
 
-    - On the top, the aggregated normalized completeness predictor $\frac{c(\Delta t)}{c_0}$ over normalized time $\Delta t = t - t_0$. It represents the overall deviation from the Model.
-    - On the bottom, interactive filters including all the columns in the [Probe][probe] (such as time, care site, number of visits...etc.) and all the estimates (coefficients and metrics) in the [Model][model].
 
-    Is is possible to save the chart in HTML with the "save_path" optional input.
+def generate_probe_line(
+    main_chart: alt.Chart,
+    probe_line_config: Dict[str, str],
+):
+    probe_line = main_chart.mark_line().encode(**probe_line_config["encode"])
+    probe_line = add_selection_on_legend(probe_line)
+    return probe_line
 
-    Parameters
-    ----------
-    probe : BaseProbe
-        Class describing the completeness predictor $c(t)$
-    fitted_model : BaseModel
-        Model fitted to the probe
-    care_site_level : str, optional
-        **EXAMPLE**: `"Hospital"`, `"Hôpital"` or `"UF"`
-    save_path : str, optional
-        Folder path where to save the chart in HTML format.
 
-        **EXAMPLE**: `"my_folder/my_file.html"`
-    labelFontSize: float, optional
-        The font size of the labels (axis and legend).
-    titleFontSize: float, optional
-        The font size of the titles.
-    """
-    alt.data_transformers.disable_max_rows()
+def generate_time_line(
+    base: alt.Chart,
+    time_line_config: Dict[str, str],
+):
+    time_selection = alt.selection_interval(encodings=["x"])
+    time_line = (
+        base.mark_line().encode(**time_line_config["encode"]).add_params(time_selection)
+    ).properties(**time_line_config["properties"])
+    return time_line, time_selection
 
-    predictor = probe.predictor.copy()
-    estimates = fitted_model.estimates.copy()
-    predictor = predictor.merge(estimates, on=probe._index)
-
-    def month_diff(x, y):
-        end = x.dt.to_period("M").view(dtype="int64")
-        start = y.dt.to_period("M").view(dtype="int64")
-        return end - start
-
-    predictor["date"] = predictor["date"].astype("datetime64[ns]")
-    predictor["t_0"] = predictor["t_0"].astype("datetime64[ns]")
-    predictor["normalized_date"] = month_diff(predictor["date"], predictor["t_0"])
-    predictor["t_0"] = predictor["t_0"].astype(str)
-    predictor["normalized_date"] = predictor["normalized_date"].astype(int)
 
-    predictor["normalized_c"] = predictor["c"].mask(
-        (predictor["normalized_date"] >= 0) & (predictor["c_0"] == 0), 1
-    )
-    predictor["normalized_c"] = predictor["normalized_c"].mask(
-        (predictor["normalized_date"] >= 0) & (predictor["c_0"] > 0),
-        predictor["c"] / predictor["c_0"],
-    )
+def generate_horizontal_bar_charts(
+    base: alt.Chart,
+    horizontal_bar_charts_config: Dict[str, str],
+    predictor: pd.DataFrame,
+):
+    horizontal_bar_charts = {}
+    y_variables_selections = {}
+    for y_variable in horizontal_bar_charts_config["y"]:
+        if y_variable["field"] not in predictor.columns:
+            continue
+        y_variable_bar_charts = []
+        y_variable_selection = alt.selection_point(fields=[y_variable["field"]])
+        y_variables_selections[y_variable["field"]] = y_variable_selection
+        y_variable_base_chart = (
+            base.mark_bar()
+            .encode(
+                y=alt.Y(**y_variable),
+            )
+            .add_params(y_variable_selection)
+        )
+        for x_variable in horizontal_bar_charts_config["x"]:
+            y_index_variable_color = alt.condition(
+                y_variables_selections[y_variable["field"]],
+                alt.Color(
+                    "{}:N".format(y_variable["field"]),
+                    legend=None,
+                    sort=x_variable["sort"],
+                ),
+                alt.value("lightgray"),
+            )
+            y_variable_bar_chart = y_variable_base_chart.encode(
+                x=x_variable["x"],
+                color=y_index_variable_color,
+                tooltip=x_variable["tooltip"],
+            )
 
-    predictor["legend_error_band"] = "Standard deviation"
-    predictor["legend_model"] = type(fitted_model).__name__
+            y_variable_bar_charts.append(y_variable_bar_chart)
+        horizontal_bar_charts[y_variable["field"]] = y_variable_bar_charts
+    return horizontal_bar_charts, y_variables_selections
 
-    predictor["model"] = predictor["c_0"].where(predictor["normalized_date"] < 0, 1)
-    predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
 
-    predictor = filter_predictor(
-        predictor=predictor,
-        care_site_level=care_site_level,
-    )
+def generate_vertical_bar_charts(
+    base: alt.Chart,
+    vertical_bar_charts_config: Dict[str, str],
+    predictor: pd.DataFrame,
+):
+    vertical_bar_charts = {}
+    x_variables_selections = {}
+    for x_variable in vertical_bar_charts_config["x"]:
+        if x_variable["field"] not in predictor.columns:
+            continue
+        x_variable_bar_charts = []
+        x_variable_selection = alt.selection_point(fields=[x_variable["field"]])
+        x_variables_selections[x_variable["field"]] = x_variable_selection
+        x_variable_base_chart = (
+            base.mark_bar()
+            .encode(
+                x=alt.X(**x_variable),
+            )
+            .add_params(x_variable_selection)
+        )
 
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        predictor = predictor[predictor.date < predictor.t_1]
-
-    index = list(set(probe._index).difference(["care_site_level", "care_site_id"]))
-    time = "date"
-    _predictor = "c"
-
-    c_0_min_slider = alt.binding_range(
-        min=0,
-        max=round_it(predictor.c_0.max(), 2),
-        step=scale_it(predictor.c_0.max()) / 100,
-        name="c₀ min: ",
-    )
-    c_0_min_selection = alt.selection_single(
-        name="c_0_min",
-        fields=["c_0_min"],
-        bind=c_0_min_slider,
-        init={"c_0_min": 0},
-    )
-    t_0_slider = alt.binding(
-        input="t_0",
-        name="t₀ max: ",
-    )
-    t_0_selection = alt.selection_single(
-        name="t_0",
-        fields=["t_0"],
-        bind=t_0_slider,
-        init={"t_0": predictor.t_0.astype(str).max()},
-    )
-    if fitted_model.name == "RectangleFunction":
-        t_1_slider = alt.binding(
-            input="t_1",
-            name="t₁ min: ",
-        )
-        t_1_selection = alt.selection_single(
-            name="t_1",
-            fields=["t_1"],
-            bind=t_1_slider,
-            init={"t_1": predictor.t_1.astype(str).min()},
-        )
-
-    error_max_slider = alt.binding_range(
-        min=0,
-        max=round_it(predictor.error.max(), 2),
-        step=scale_it(predictor.error.max()) / 100,
-        name="error max: ",
-    )
-    error_max_selection = alt.selection_single(
-        name="error_max",
-        fields=["error_max"],
-        bind=error_max_slider,
-        init={"error_max": round_it(predictor.error.max(), 2)},
-    )
+        for y_variable in vertical_bar_charts_config["y"]:
+            x_index_variable_color = alt.condition(
+                x_variables_selections[x_variable["field"]],
+                alt.Color(
+                    "{}:N".format(x_variable["field"]),
+                    legend=None,
+                    sort=y_variable["sort"],
+                ),
+                alt.value("lightgray"),
+            )
+            x_variable_bar_chart = x_variable_base_chart.encode(
+                y=y_variable["y"],
+                color=x_index_variable_color,
+                tooltip=y_variable["tooltip"],
+            )
 
-    care_site_selection = alt.selection_multi(fields=["care_site_short_name"])
-    care_site_color = alt.condition(
-        care_site_selection,
-        alt.Color(
-            "care_site_short_name:N",
-            legend=None,
-            sort={"field": "c_0", "op": "min", "order": "descending"},
-        ),
-        alt.value("lightgray"),
-    )
+            x_variable_bar_charts.append(x_variable_bar_chart)
+        vertical_bar_charts[x_variable["field"]] = x_variable_bar_charts
+    return vertical_bar_charts, x_variables_selections
 
-    base_chart = alt.Chart(predictor).transform_joinaggregate(
-        mean_c_0="mean(c_0)",
-        mean_error="mean(error)",
-        groupby=["care_site_short_name"] + index,
-    )
 
-    time_selection = alt.selection_interval(encodings=["x"])
-    time_line = (
-        base_chart.mark_line()
-        .encode(
-            x=alt.X(
-                "normalized_date:Q",
-                title="Δt = (t - t₀) months",
-                scale=alt.Scale(nice=False),
-            ),
-            y=alt.Y(
-                "mean(c):Q",
-                title="c(Δt)",
-            ),
-        )
-        .add_selection(time_selection)
-    ).properties(width=800, height=50)
+def add_interactive_selection(
+    base: alt.Chart,
+    selections: Dict[str, alt.SelectionParameter],
+    selection_charts: Dict[str, List[alt.Chart]] = None,
+):
+    if selection_charts is None:
+        selection_charts = {}
+    for selection_variable, selection in selections.items():
+        base = base.transform_filter(selection)
+        for chart_variable in selection_charts.keys():
+            if chart_variable != selection_variable:
+                for i in range(len(selection_charts[chart_variable])):
+                    selection_charts[chart_variable][i] = selection_charts[
+                        chart_variable
+                    ][i].transform_filter(selection)
+    return base
+
+
+def add_selection_on_legend(
+    chart: alt.Chart, opacity_true: float = 1, opacity_false: float = 0.2
+):
+    legend_selection = alt.selection_point(fields=["value"], bind="legend")
+    chart = chart.encode(
+        opacity=alt.condition(
+            legend_selection, alt.value(opacity_true), alt.value(opacity_false)
+        )
+    ).add_params(legend_selection)
+    return chart
 
-    predictor_hist = (
-        base_chart.mark_bar()
-        .encode(
-            y=alt.Y(
-                "care_site_short_name:N",
-                title="Care site short name",
-                sort="-x",
-            ),
-            color=care_site_color,
-        )
-        .add_selection(care_site_selection)
-        .transform_filter(alt.datum.mean_c_0 >= c_0_min_selection.c_0_min)
-        .transform_filter(alt.datum.mean_error <= error_max_selection.error_max)
-        .transform_filter(alt.datum.t_0 <= t_0_selection.t_0)
-    ).properties(width=300)
-
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        predictor_hist = predictor_hist.transform_filter(
-            alt.datum.t_1 >= t_1_selection.t_1
-        )
-
-    c_0_hist = predictor_hist.encode(
-        x=alt.X(
-            "min(mean_c_0):Q",
-            title="Min(c₀)",
-        ),
-        tooltip=alt.Tooltip("min(mean_c_0):Q", format=".2"),
-    )
-    error_hist = predictor_hist.encode(
-        x=alt.X(
-            "max(mean_error):Q",
-            title="Max(error)",
-        ),
-        tooltip=alt.Tooltip("max(mean_error):Q", format=".2"),
-    )
 
-    index_variables_hists = []
-    index_variables_selections = []
-    for index_variable in index:
-        index_variable_selection = alt.selection_multi(fields=[index_variable])
-        index_variables_selections.append(index_variable_selection)
-
-        index_variable_color = alt.condition(
-            index_variable_selection,
-            alt.Color(
-                "{}:N".format(index_variable),
-                legend=None,
-                sort={"field": "c_0", "op": "min", "order": "descending"},
+def add_estimates_filters(
+    base: alt.Chart,
+    estimates_filters: Dict[str, alt.SelectionParameter],
+    selection_charts: Dict[str, List[alt.Chart]] = None,
+):
+    if selection_charts is None:
+        selection_charts = {}
+    for estimate_filter in estimates_filters:
+        base = base.transform_filter(estimate_filter)
+        for chart_variable in selection_charts.keys():
+            for i in range(len(selection_charts[chart_variable])):
+                selection_charts[chart_variable][i] = selection_charts[chart_variable][
+                    i
+                ].transform_filter(estimate_filter)
+
+    return base
+
+
+def create_groupby_selection(
+    indexes: List[Dict[str, str]],
+    predictor: pd.DataFrame,
+):
+    index_fields = [
+        index["field"] for index in indexes if index["field"] in predictor.columns
+    ]
+    if len(index_fields) >= 2:
+        index_labels = [
+            index["title"] for index in indexes if index["field"] in predictor.columns
+        ]
+        index_selection = alt.selection_point(
+            fields=["index"],
+            bind=alt.binding_radio(
+                name="Group by: ", options=index_fields, labels=index_labels
             ),
-            alt.value("lightgray"),
+            value=index_fields[0],
         )
-        index_variable_hist = (
-            base_chart.mark_bar()
-            .encode(
-                y=alt.Y(
-                    "mean(c):Q",
-                    title="c",
-                ),
-                x=alt.X(
-                    "{}:N".format(index_variable),
-                    title=index_variable,
-                    sort="-y",
-                ),
-                tooltip=alt.Tooltip("mean(c):Q", format=".2"),
-                color=index_variable_color,
-            )
-            .add_selection(index_variable_selection)
-            .transform_filter(care_site_selection)
-            .transform_filter(alt.datum.mean_c_0 >= c_0_min_selection.c_0_min)
-            .transform_filter(alt.datum.t_0 <= t_0_selection.t_0)
-            .transform_filter(alt.datum.mean_error <= error_max_selection.error_max)
-        ).properties(title="Average completeness per {}".format(index_variable))
-
-        # RectangleModel
-        if fitted_model.name == "RectangleFunction":
-            index_variable_hist = index_variable_hist.transform_filter(
-                alt.datum.t_1 >= t_1_selection.t_1
-            )
+    else:
+        index_selection = None
+    return index_selection, index_fields
 
-        index_variables_hists.append(index_variable_hist)
 
-    extra_predictors = predictor.columns.difference(
-        index
-        + [time]
-        + [_predictor]
-        + [
-            "care_site_short_name",
-            "care_site_id",
-            "model",
-            "legend_error_band",
-            "legend_model",
-            "normalized_date",
-            "normalized_c",
-            "c_0",
-            "t_0",
-            "t_1",
-            "error",
-        ]
+def configure_style(
+    chart: alt.Chart,
+    chart_style: Dict[str, float],
+):
+    return chart.configure_axis(
+        labelFontSize=chart_style["labelFontSize"],
+        titleFontSize=chart_style["titleFontSize"],
+        labelLimit=500,
+    ).configure_legend(
+        labelFontSize=chart_style["labelFontSize"],
+        titleFontSize=chart_style["titleFontSize"],
+        labelLimit=500,
     )
-    extra_predictors_hists = []
 
-    for extra_predictor in extra_predictors:
-        extra_predictor_hist = predictor_hist.encode(
-            x=alt.X(
-                "sum({}):Q".format(extra_predictor),
-                title="{}".format(extra_predictor),
-                axis=alt.Axis(format="s"),
-            ),
-            tooltip=alt.Tooltip("sum({}):Q".format(extra_predictor), format=","),
-        ).properties(title="Total {} per care site".format(extra_predictor))
-        extra_predictors_hists.append(extra_predictor_hist)
-
-    index.append("care_site_short_name")
-    index_selection = alt.selection_single(
-        fields=["index"],
-        bind=alt.binding_radio(name="Group by: ", options=index),
-        init={"index": "stay_type"},
-    )
 
-    probe_line = (
-        base_chart.transform_fold(index, as_=["index", "value"])
-        .encode(
-            x=alt.X(
-                "normalized_date:Q",
-                title="Δt = (t - t₀) months",
-                scale=alt.Scale(nice=False),
-            ),
-            color=alt.Color(
-                "value:N",
-                sort={"field": "c_0", "op": "min", "order": "descending"},
-                title=None,
+def concatenate_charts(
+    main_chart: alt.Chart,
+    horizontal_bar_charts: Dict[str, List[alt.Chart]],
+    vertical_bar_charts: Dict[str, List[alt.Chart]],
+    time_line: alt.Chart = None,
+    spacing: float = 10,
+):
+    # Horizontal histograms
+    bar_charts_rows = []
+    for bar_charts_row in horizontal_bar_charts.values():
+        bar_charts_row = reduce(
+            lambda bar_chart_1, bar_chart_2: (bar_chart_1 | bar_chart_2).resolve_scale(
+                color="independent"
             ),
+            bar_charts_row,
         )
-        .transform_filter(alt.datum.mean_c_0 >= c_0_min_selection.c_0_min)
-        .transform_filter(alt.datum.mean_error <= error_max_selection.error_max)
-        .transform_filter(alt.datum.t_0 <= t_0_selection.t_0)
-        .transform_filter(care_site_selection)
-        .transform_filter(index_selection)
-    ).properties(width=900, height=300)
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        probe_line = probe_line.transform_filter(alt.datum.t_1 >= t_1_selection.t_1)
-
-    mean_line = probe_line.mark_line().encode(
-        y=alt.Y(
-            "mean(normalized_c):Q",
-        )
-    )
-    error_line = probe_line.mark_errorband(extent="stdev").encode(
-        y=alt.Y(
-            "normalized_c:Q",
-            title="c(Δt) / c₀",
-        ),
-        stroke=alt.Stroke(
-            "legend_error_band",
-            title="Error band",
-            legend=alt.Legend(symbolType="square", orient="top"),
-        ),
-    )
-    model_line = (
-        alt.Chart(predictor)
-        .mark_line(color="black", interpolate="step-after", strokeDash=[5, 5])
-        .encode(
-            x=alt.X(
-                "normalized_date:Q",
-                scale=alt.Scale(nice=False),
+        bar_charts_rows.append(bar_charts_row)
+    if bar_charts_rows:
+        horizontal_bar_charts = reduce(
+            lambda bar_chart_1, bar_chart_2: (bar_chart_1 & bar_chart_2).resolve_scale(
+                color="independent"
             ),
-            y="model:Q",
-            strokeWidth=alt.StrokeWidth(
-                "legend_model",
-                title="Model line",
-                legend=alt.Legend(orient="top", symbolDash=[2, 2]),
+            bar_charts_rows,
+        )
+
+    # Vertical histograms
+    bar_charts_columns = []
+    for bar_charts_column in vertical_bar_charts.values():
+        bar_charts_column = reduce(
+            lambda bar_chart_1, bar_chart_2: (bar_chart_1 | bar_chart_2).resolve_scale(
+                color="independent"
             ),
+            bar_charts_column,
         )
-    )
+        bar_charts_columns.append(bar_charts_column)
+    if bar_charts_columns:
+        if bar_charts_rows:
+            vertical_bar_charts = reduce(
+                lambda bar_chart_1, bar_chart_2: (
+                    bar_chart_1 & bar_chart_2
+                ).resolve_scale(color="independent"),
+                bar_charts_columns,
+            )
+        else:
+            vertical_bar_charts = reduce(
+                lambda bar_chart_1, bar_chart_2: (
+                    bar_chart_1 | bar_chart_2
+                ).resolve_scale(color="independent"),
+                bar_charts_columns,
+            )
 
-    top_chart = mean_line + error_line + model_line
+    if bar_charts_rows:
+        if bar_charts_columns:
+            bottom_chart = vertical_bar_charts | horizontal_bar_charts
+        else:
+            bottom_chart = horizontal_bar_charts
+    elif bar_charts_columns:
+        bottom_chart = vertical_bar_charts
+    else:
+        bottom_chart = None
+
+    if time_line:
+        top_chart = alt.vconcat(main_chart, time_line, spacing=100).resolve_scale(
+            color="independent"
+        )
+    else:
+        top_chart = main_chart
+
+    if bottom_chart:
+        concat_chart = alt.vconcat(
+            top_chart,
+            bottom_chart,
+            spacing=spacing,
+        )
+    else:
+        concat_chart = top_chart
+    return concat_chart
+
+
+def month_diff(x, y):
+    end = x.dt.to_period("M").view(dtype="int64")
+    start = y.dt.to_period("M").view(dtype="int64")
+    return end - start
 
-    top_chart = top_chart.add_selection(index_selection).transform_filter(
-        time_selection
-    )
 
-    for index_variable_selection in index_variables_selections:
-        top_chart = top_chart.transform_filter(index_variable_selection)
-        c_0_hist = c_0_hist.transform_filter(index_variable_selection)
-        error_hist = error_hist.transform_filter(index_variable_selection)
-        for idx in range(len(extra_predictors_hists)):
-            extra_predictors_hists[idx] = extra_predictors_hists[idx].transform_filter(
-                index_variable_selection
-            )
-        for idx in range(len(index_variables_hists)):
-            if idx != index_variables_selections.index(index_variable_selection):
-                index_variables_hists[idx] = index_variables_hists[
-                    idx
-                ].transform_filter(index_variable_selection)
-
-    index_variables_hists = reduce(
-        lambda index_variable_hist_1, index_variable_hist_2: index_variable_hist_1
-        & index_variable_hist_2,
-        index_variables_hists,
-    )
-    extra_predictors_hists = reduce(
-        lambda extra_predictor_hist_1, extra_predictor_hist_2: extra_predictor_hist_1
-        & extra_predictor_hist_2,
-        extra_predictors_hists,
-    )
+def save_html(obj: alt.Chart, filename: str):
+    """Save chart in the specified file
 
-    chart = (
-        (
-            (
-                alt.vconcat(
-                    alt.vconcat(top_chart, time_line, spacing=130),
-                    (
-                        index_variables_hists
-                        | c_0_hist
-                        | error_hist & extra_predictors_hists
-                    ),
-                    spacing=10,
-                )
-            )
-            .resolve_scale(color="independent")
-            .add_selection(error_max_selection)
-            .add_selection(c_0_min_selection)
-            .add_selection(t_0_selection)
-        )
-        .configure_axis(labelFontSize=labelFontSize, titleFontSize=titleFontSize)
-        .configure_legend(labelFontSize=labelFontSize)
-    )
-    if fitted_model.name == "RectangleFunction":
-        chart = chart.add_selection(t_1_selection)
+    Parameters
+    ----------
+    obj : alt.Chart
+        Altair chart to be saved
+    filename : str
+        Folder path where to save the chart in HTML format.
 
-    vis_threshold = "id" + uuid.uuid4().hex
-    new_sliders_threshold_id = "id" + uuid.uuid4().hex
-    old_sliders_threshold_id = "id" + uuid.uuid4().hex
-    new_index_threshold_id = "id" + uuid.uuid4().hex
-    old_index_threshold_id = "id" + uuid.uuid4().hex
-    html_chart = f"""
-        <!DOCTYPE html>
-        <html>
-        <head>
-          <script src="https://cdn.jsdelivr.net/npm/vega@{alt.VEGA_VERSION}"></script>
-          <script src="https://cdn.jsdelivr.net/npm/vega-lite@{alt.VEGALITE_VERSION}"></script>
-          <script src="https://cdn.jsdelivr.net/npm/vega-embed@{alt.VEGAEMBED_VERSION}"></script>
-        </head>
-        <body>
-
-        <div class="container">
-          <div class="row">
-            <div>
-            <div id={vis_threshold}></div>
-            </div>
-            <div style="position:absolute;left:920px;top:520px;width: -webkit-fill-available;">
-            <div id={new_sliders_threshold_id}>
-              <div id={old_sliders_threshold_id}></div>
-            </div>
-            </div>
-            <div style="position:absolute;left:45px;top:390px;width: -webkit-fill-available;">
-            <div id={new_index_threshold_id}>
-              <div id={old_index_threshold_id}></div>
-            </div>
-            <hr/>
-            <h1 style="text-align:center"> Interactive filters </h1>
-            </div>
-          </div>
-        </div>
-
-        <script type="text/javascript">
-        vegaEmbed('#{vis_threshold}', {chart.to_json(indent=None)}).then(function(result) {{
-            const sliders = document.getElementsByClassName('vega-bindings');
-            const newestimate = document.getElementById('{new_sliders_threshold_id}');
-            const oldestimate = document.getElementById('{old_sliders_threshold_id}');
-            const newparent = document.getElementById('{new_index_threshold_id}');
-            const oldchild = document.getElementById('{old_index_threshold_id}');
-            for (var i = 0; i < sliders.length; i++) {{
-                if (sliders[i].parentElement.parentElement.id == '{vis_threshold}') {{
-                    var estimate_slider = sliders[i]
-                    var index_slider = estimate_slider.querySelectorAll(".vega-bind")
-                    }}
-                }}
-            newestimate.replaceChild(estimate_slider, oldestimate);
-            for (var i = 0; i < index_slider.length; i++) {{
-                if (index_slider[i].firstChild.innerHTML == "Group by: ") {{
-                    var index_color = index_slider[i]}}
-                }}
-            newparent.replaceChild(index_color, oldchild);
-            }}).catch(console.error);
-        </script>
-        </body>
-        </html>
-        """
-    display(HTML(html_chart))
-    if save_path:
-        save_html(
-            obj=html_chart,
-            filename=save_path,
-        )
+        **EXAMPLE**: `"my_folder/my_file.html"`
+    """
+    if not isinstance(filename, Path):
+        filename = Path(filename)
+    os.makedirs(filename.parent, exist_ok=True)
+    if hasattr(obj, "save"):
+        obj.save(filename)
+    else:
+        with open(filename, "w") as f:
+            f.write(obj)
+    logger.info("The chart has been saved in {}", filename)
+
+
+def round_up(x: float, sig: int):
+    if x == 0:
+        return 0
+    else:
+        decimals = sig - floor(log10(abs(x))) - 1
+        return ceil(x * 10**decimals) / 10**decimals
+
+
+def scale_it(x: float):
+    if x == 0:
+        return 1
+    else:
+        return 10 ** ceil(log10(x))
+
+
+def filter_predictor(
+    predictor: pd.DataFrame,
+    care_site_level: str = None,
+    stay_type: List[str] = None,
+    care_site_id: List[int] = None,
+    care_site_short_name: List[int] = None,
+    start_date: Union[datetime, str] = None,
+    end_date: Union[datetime, str] = None,
+    **kwargs
+):
+    # Time
+    predictor = filter_table_by_date(
+        table=predictor,
+        table_name="predictor",
+        start_date=start_date,
+        end_date=end_date,
+    )
+
+    # Care site level
+    if care_site_level:
+        if not isinstance(care_site_level, list):
+            care_site_level = [care_site_level]
+        care_site_levels = []
+        for care_site_lvl in care_site_level:
+            if care_site_lvl in CARE_SITE_LEVEL_NAMES.keys():
+                care_site_lvl = CARE_SITE_LEVEL_NAMES[care_site_lvl]
+            if care_site_lvl not in predictor.care_site_level.unique():
+                raise AttributeError(
+                    "The selected care site level {} is not part of the computed care site levels {}".format(
+                        care_site_level, list(predictor.care_site_level.unique())
+                    )
+                )
+            care_site_levels.append(care_site_lvl)
+        predictor = predictor[predictor.care_site_level.isin(care_site_levels)]
+        logger.debug(
+            "Predictor has been filtered on the selected care site level : {}",
+            care_site_levels,
+        )
+
+    # Stay type
+    if stay_type:
+        if not isinstance(stay_type, list):
+            stay_type = [stay_type]
+        predictor = predictor[predictor.stay_type.isin(stay_type)]
+        logger.debug(
+            "Predictor has been filtered on the selected stay type : {}",
+            stay_type,
+        )
+
+    # Care site id
+    if care_site_id:
+        if not isinstance(care_site_id, list):
+            care_site_id = [care_site_id]
+        predictor = predictor[predictor.care_site_id.isin(care_site_id)]
+        logger.debug(
+            "Predictor has been filtered on the selected care site id : {}",
+            care_site_id,
+        )
+
+    # Care site short name
+    if care_site_short_name:
+        if not isinstance(care_site_short_name, list):
+            care_site_short_name = [care_site_short_name]
+        predictor = predictor[predictor.care_site_short_name.isin(care_site_short_name)]
+        logger.debug(
+            "Predictor has been filtered on the selected care site short name : {}",
+            care_site_short_name,
+        )
+
+    # Others
+    for key, value in kwargs.items():
+        if not isinstance(value, list):
+            value = [value]
+        predictor = predictor[predictor[key].isin(value)]
+        logger.debug(
+            "Predictor has been filtered on the selected {} : {}",
+            key,
+            value,
+        )
+
+    # Care site specialty
+    if (
+        "care_site_specialty" in predictor.columns
+        and predictor[~(predictor.care_site_specialty == "Non Renseigné")].empty
+    ):
+        predictor = predictor.drop(columns="care_site_specialty")
+
+    if predictor.empty:
+        raise TypeError("Empty predictor: no data to plot.")
+    return predictor
```

### Comparing `edsteva-0.1.4/edsteva/viz/dashboards/predictor_dashboard/probe.py` & `edsteva-0.2.0/edsteva/probes/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,218 +1,211 @@
-from functools import reduce
-from typing import List
+from datetime import datetime
+from typing import Dict, List
 
-import altair as alt
 import pandas as pd
+from loguru import logger
 
+from edsteva.utils.framework import get_framework
+from edsteva.utils.typing import DataFrame
 
-def probe_dashboard(
-    predictor: pd.DataFrame,
-    index: List[str],
-    x_axis_title: str = "Time (Month Year)",
-    y_axis_title: str = "Completeness predictor c(t)",
-    x_grid: bool = True,
-    y_grid: bool = True,
-    show_n_visit: bool = False,
-    labelAngle: float = -90,
+CARE_SITE_LEVEL_NAMES = {
+    "Hospital": "Hôpital",
+    "Pole": "Pôle/DMU",
+    "UF": "Unité Fonctionnelle (UF)",
+    "UC": "Unité de consultation (UC)",
+    "UH": "Unité d’hébergement (UH)",
+}
+
+VISIT_DETAIL_TYPE = {
+    "UF": "PASS UF",
+    "UC": "PASS UC",
+    "UH": "PASS UH",
+}
+
+
+def impute_missing_dates(
+    start_date: datetime,
+    end_date: datetime,
+    predictor: DataFrame,
+    partition_cols: List[str],
 ):
-    """Script to be used by [``predictor_dashboard()``][edsteva.viz.dashboards.predictor_dashboard.wrapper]
-
-    Parameters
-    ----------
-    predictor : pd.DataFrame
-        $c(t)$ computed in the Probe
-    index : List[str]
-        Variable from which data is grouped
-    x_axis_title: str, optional,
-        Label name for the x axis.
-    x_grid: bool, optional,
-        If False, remove the grid for the x axis.
-    y_axis_title: str, optional,
-        Label name for the y axis.
-    y_grid: bool, optional,
-        If False, remove the grid for the y axis.
-    show_n_visit: bool, optional
-        show the number of visit instead of the completeness predictor $c(t)$
-    labelAngle: float, optional
-        The rotation angle of the label on the x_axis.
-    """
-
-    time = "date"
-    _predictor = "c"
-
-    alt.data_transformers.disable_max_rows()
-
-    time_selection = alt.selection_interval(encodings=["x"])
-    time_line = (
-        alt.Chart(predictor)
-        .mark_line()
-        .encode(
-            x=alt.X(
-                f'yearmonth({"date"}):T',
-                title=x_axis_title,
-                axis=alt.Axis(tickCount="month", labelAngle=labelAngle),
-            ),
-            y=alt.Y(
-                "mean(c):Q",
-                title="c(t)",
-            ),
-        )
-        .add_selection(time_selection)
-    ).properties(width=900, height=50)
-
-    care_site_selection = alt.selection_multi(fields=["care_site_short_name"])
-    care_site_color = alt.condition(
-        care_site_selection,
-        alt.Color(
-            "care_site_short_name:N",
-            legend=None,
-            sort={"field": "c", "op": "mean", "order": "descending"},
-        ),
-        alt.value("lightgray"),
+    # Generate all available dates
+    if not start_date:
+        start_date = predictor["date"].min()
+    if not end_date:
+        end_date = predictor["date"].max()
+    date_index = pd.date_range(
+        start=start_date,
+        end=end_date,
+        freq="MS",
+        closed="left",
     )
-    predictor_hist = (
-        alt.Chart(predictor)
-        .mark_bar()
-        .encode(
-            y=alt.Y(
-                "care_site_short_name:N",
-                title="Care site short name",
-                sort="-x",
-            ),
-            color=care_site_color,
-        )
-        .transform_filter(time_selection)
-        .add_selection(care_site_selection)
-    ).properties(width=300)
-
-    care_site_hist = predictor_hist.encode(
-        x=alt.X(
-            "mean(c):Q",
-            title="c",
-        ),
-        tooltip=alt.Tooltip("mean(c):Q", format=".2"),
-    ).properties(title="Average completeness per care site")
-
-    index_variables_hists = []
-    index_variables_selections = []
-    for index_variable in index:
-        index_variable_selection = alt.selection_multi(fields=[index_variable])
-        index_variables_selections.append(index_variable_selection)
-
-        index_variable_color = alt.condition(
-            index_variable_selection,
-            alt.Color(
-                "{}:N".format(index_variable),
-                legend=None,
-                sort={"field": "c", "op": "mean", "order": "descending"},
-            ),
-            alt.value("lightgray"),
-        )
-        index_variable_hist = (
-            alt.Chart(predictor)
-            .mark_bar()
-            .encode(
-                y=alt.Y(
-                    "mean(c):Q",
-                    title="c",
-                ),
-                x=alt.X(
-                    "{}:N".format(index_variable),
-                    title=index_variable,
-                    sort="-y",
-                ),
-                tooltip=alt.Tooltip("mean(c):Q", format=".2"),
-                color=index_variable_color,
-            )
-            .add_selection(index_variable_selection)
-            .transform_filter(time_selection)
-            .transform_filter(care_site_selection)
-        ).properties(title="Average completeness per {}".format(index_variable))
-        index_variables_hists.append(index_variable_hist)
-
-    extra_predictors = predictor.columns.difference(
-        index
-        + [time]
-        + [_predictor]
-        + ["care_site_short_name", "care_site_id", "c_hat"]
+    date_index = pd.DataFrame({"date": date_index})
+
+    # Generate all available partitions
+    all_partitions = (
+        predictor[list(set(partition_cols) - {"date"})]
+        .drop_duplicates()
+        .merge(date_index, how="cross")
     )
-    extra_predictors_hists = []
+    filled_predictor = all_partitions.merge(
+        predictor,
+        on=partition_cols,
+        how="left",
+    ).fillna({col: 0 for col in set(predictor.columns) - set(partition_cols)})
+    return filled_predictor
 
-    for extra_predictor in extra_predictors:
-        extra_predictor_hist = predictor_hist.encode(
-            x=alt.X(
-                "sum({}):Q".format(extra_predictor),
-                title="{}".format(extra_predictor),
-                axis=alt.Axis(format="s"),
-            ),
-            tooltip=alt.Tooltip("sum({}):Q".format(extra_predictor), format=","),
-        ).properties(title="Total {} per care site".format(extra_predictor))
-
-        extra_predictors_hists.append(extra_predictor_hist)
-
-    index.append("care_site_short_name")
-    index_selection = alt.selection_single(
-        fields=["index"],
-        bind=alt.binding_radio(name="Group by: ", options=index),
-        init={"index": "stay_type"},
+
+def hospital_only(care_site_levels: List[str]):
+    if not isinstance(care_site_levels, list):
+        care_site_levels = [care_site_levels]
+    return len(care_site_levels) == 1 and (
+        care_site_levels[0] == "Hospital"
+        or care_site_levels[0] == CARE_SITE_LEVEL_NAMES["Hospital"]
     )
-    probe_line = (
-        alt.Chart(predictor)
-        .transform_fold(index, as_=["index", "value"])
-        .mark_line()
-        .encode(
-            x=alt.X(
-                f'yearmonth({"date"}):T',
-                title=x_axis_title,
-                axis=alt.Axis(tickCount="month", labelAngle=-90, grid=x_grid),
-            ),
-            y=alt.Y(
-                "sum(n_visit):Q" if show_n_visit else "mean(c):Q",
-                title=y_axis_title,
-                axis=alt.Axis(grid=y_grid),
-            ),
-            color=alt.Color(
-                "value:N",
-                sort={"field": "c", "op": "mean", "order": "descending"},
-                title=None,
-            ),
-        )
-        .add_selection(index_selection)
-        .transform_filter(index_selection)
-        .transform_filter(care_site_selection)
-        .transform_filter(time_selection)
-    ).properties(width=900, height=300)
-
-    for index_variable_selection in index_variables_selections:
-        probe_line = probe_line.transform_filter(index_variable_selection)
-        care_site_hist = care_site_hist.transform_filter(index_variable_selection)
-        for idx in range(len(extra_predictors_hists)):
-            extra_predictors_hists[idx] = extra_predictors_hists[idx].transform_filter(
-                index_variable_selection
+
+
+def concatenate_predictor_by_level(
+    predictor_by_level: Dict[str, DataFrame],
+    care_site_levels: List[str] = None,
+) -> DataFrame:
+    predictors_to_concat = []
+    if care_site_levels:
+        if not isinstance(care_site_levels, list):
+            care_site_levels = [care_site_levels]
+        unknown_levels, unavailable_levels, selected_levels = [], [], []
+        for level in care_site_levels:
+            if level in predictor_by_level.keys():
+                predictors_to_concat.append(predictor_by_level[level])
+                selected_levels.append(level)
+            elif level in CARE_SITE_LEVEL_NAMES.keys():
+                raw_level = CARE_SITE_LEVEL_NAMES[level]
+                if raw_level in predictor_by_level.keys():
+                    predictors_to_concat.append(predictor_by_level[raw_level])
+                    selected_levels.append(level)
+                else:
+                    unavailable_levels.append(level)
+            else:
+                unknown_levels.append(level)
+
+        logger.debug(
+            "The following levels {} have been selected",
+            selected_levels,
+        )
+        if unknown_levels:
+            logger.warning(
+                "Unrecognized levels {}.the only supported levels are: {}",
+                unknown_levels,
+                list(CARE_SITE_LEVEL_NAMES.values())
+                + list(CARE_SITE_LEVEL_NAMES.keys()),
             )
-        for idx in range(len(index_variables_hists)):
-            if idx != index_variables_selections.index(index_variable_selection):
-                index_variables_hists[idx] = index_variables_hists[
-                    idx
-                ].transform_filter(index_variable_selection)
-
-    index_variables_hists = reduce(
-        lambda index_variable_hist_1, index_variable_hist_2: index_variable_hist_1
-        & index_variable_hist_2,
-        index_variables_hists,
-    )
-    extra_predictors_hists = reduce(
-        lambda extra_predictor_hist_1, extra_predictor_hist_2: extra_predictor_hist_1
-        & extra_predictor_hist_2,
-        extra_predictors_hists,
-    )
+        if unavailable_levels:
+            logger.warning(
+                "The following levels: {} are not available for this probe.",
+                unavailable_levels,
+            )
+    else:
+        predictors_to_concat = list(predictor_by_level.values())
+        logger.debug(
+            "The following levels {} have been selected",
+            list(predictor_by_level.keys()),
+        )
 
-    chart = (
-        alt.vconcat(
-            alt.vconcat(probe_line, time_line, spacing=130),
-            (index_variables_hists | care_site_hist | extra_predictors_hists),
-            spacing=10,
+    if not predictors_to_concat:
+        raise AttributeError(
+            "care site levels must include at least one of the following levels: {}".format(
+                list(CARE_SITE_LEVEL_NAMES.values())
+                + list(CARE_SITE_LEVEL_NAMES.keys())
+            )
+        )
+
+    return get_framework(predictors_to_concat[0]).concat(predictors_to_concat)
+
+
+def get_child_and_parent_cs(
+    care_site_sample: DataFrame, care_site_relationship: DataFrame
+):
+    extended_care_site_id_to_filter = []
+
+    # Parent care site to get
+    parent_rel = care_site_relationship[
+        ~care_site_relationship.parent_care_site_id.isna()
+    ][
+        [
+            "care_site_id",
+            "parent_care_site_id",
+            "parent_care_site_level",
+            "parent_care_site_specialty",
+        ]
+    ]
+    parent_care_site_filter = care_site_sample.copy()
+    while set(parent_care_site_filter.care_site_level.unique()).intersection(
+        CARE_SITE_LEVEL_NAMES.values()
+    ):
+        extended_care_site_id_to_filter.append(
+            parent_care_site_filter[
+                ["care_site_id", "care_site_level", "care_site_specialty"]
+            ]
+        )
+        parent_care_site_filter = parent_care_site_filter.merge(
+            parent_rel,
+            on="care_site_id",
+        )[
+            [
+                "parent_care_site_id",
+                "parent_care_site_level",
+                "parent_care_site_specialty",
+            ]
+        ].rename(
+            columns={
+                "parent_care_site_id": "care_site_id",
+                "parent_care_site_level": "care_site_level",
+                "parent_care_site_specialty": "care_site_specialty",
+            }
+        )
+
+    # Child care site to get
+    child_rel = care_site_relationship[~care_site_relationship.care_site_id.isna()][
+        [
+            "care_site_id",
+            "care_site_level",
+            "care_site_specialty",
+            "parent_care_site_id",
+        ]
+    ].rename(
+        columns={
+            "care_site_id": "child_care_site_id",
+            "care_site_level": "child_care_site_level",
+            "care_site_specialty": "child_care_site_specialty",
+            "parent_care_site_id": "care_site_id",
+        }
+    )
+    child_care_site_filter = care_site_sample.copy()
+    while set(child_care_site_filter.care_site_level.unique()).intersection(
+        CARE_SITE_LEVEL_NAMES.values()
+    ):
+        extended_care_site_id_to_filter.append(
+            child_care_site_filter[
+                ["care_site_id", "care_site_level", "care_site_specialty"]
+            ]
+        )
+        child_care_site_filter = child_care_site_filter.merge(
+            child_rel,
+            on="care_site_id",
+        )[
+            [
+                "child_care_site_id",
+                "child_care_site_level",
+                "child_care_site_specialty",
+            ]
+        ].rename(
+            columns={
+                "child_care_site_id": "care_site_id",
+                "child_care_site_level": "care_site_level",
+                "child_care_site_specialty": "care_site_specialty",
+            }
         )
-    ).resolve_scale(color="independent")
 
-    return chart
+    extended_care_site_id_to_filter = pd.concat(
+        extended_care_site_id_to_filter
+    ).drop_duplicates()
+    return extended_care_site_id_to_filter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `edsteva-0.1.4/edsteva/viz/plots/normalized_probe.py` & `edsteva-0.2.0/edsteva/probes/biology/biology.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,315 +1,194 @@
 from datetime import datetime
-from typing import List, Union
+from typing import Dict, List, Tuple, Union
 
-import altair as alt
 import pandas as pd
 
-from edsteva.models.base import BaseModel
 from edsteva.probes.base import BaseProbe
-from edsteva.viz.utils import filter_predictor, round_it, save_html, scale_it
+from edsteva.probes.biology.completeness_predictors import completeness_predictors
+from edsteva.probes.biology.viz_configs import viz_configs
+from edsteva.utils.typing import Data
 
 
-def plot_normalized_probe(
-    probe: BaseProbe,
-    fitted_model: BaseModel,
-    t_0_max: datetime = None,
-    t_1_min: datetime = None,
-    error_max: float = None,
-    c_0_min: float = None,
-    care_site_level: str = None,
-    stay_type: List[str] = None,
-    care_site_id: List[int] = None,
-    start_date: Union[datetime, str] = None,
-    end_date: Union[datetime, str] = None,
-    care_site_short_name: List[int] = None,
-    t_min: int = None,
-    t_max: int = None,
-    save_path: str = None,
-    x_axis_title: str = "Δt = (t - t₀) months",
-    y_axis_title: str = "c(Δt) / c₀",
-    show_per_care_site: bool = False,
-    labelFontSize: float = 12,
-    titleFontSize: float = 13,
-    **kwargs,
-):
-    r"""Displays a chart with the aggregated normalized completeness predictor $\frac{c(\Delta t)}{c_0}$ over normalized time $\Delta t = t - t_0$. It represents the overall deviation from the Model.
+class BiologyProbe(BaseProbe):
+    r"""
+    The ``BiologyProbe`` computes $c_(t)$ the availability of laboratory data related to biological measurements for each biological code and each care site according to time:
 
-    Is is possible to save the chart in HTML with the "save_path" optional input.
+    $$
+    c(t) = \frac{n_{biology}(t)}{n_{99}}
+    $$
+
+    Where $n_{biology}(t)$ is the number of biological measurements, $n_{99}$ is the $99^{th}$ percentile and $t$ is the month.
 
     Parameters
     ----------
-    probe : BaseProbe
-        Class describing the completeness predictor $c(t)$
-    fitted_model : BaseModel
-        Model fitted to the probe
-    t_0_max : datetime, optional
-        Initial value for the $t_0$ threshold. If None, it will be set as the maximum possible $t_0$ value.
-
-        **EXAMPLE**: `"2022-01"`, `datetime(2020, 2, 1)`
-    error_max : float, optional
-        Initial value for the $error$ threshold. If None, it will be set as the maximum possible error value.
-
-        **EXAMPLE**: `0.02`, `0.25`
-    c_0_min : float, optional
-        Initial value for the $c_0$ threshold. If None, it will be set as 0.
-
-        **EXAMPLE**: `0.1`, `0.8`
-    stay_type : List[str], optional
-        **EXAMPLE**: `"All"` or `["All", "Urg"]`
-    care_site_id : List[int], optional
-        **EXAMPLE**: `[8312056386, 8312027648]`
-    care_site_level : str, optional
-        **EXAMPLE**: `"Hospital"`, `"Hôpital"` or `"UF"`
-    stay_type : List[str], optional
-        **EXAMPLE**: `"All"` or `["All", "Urg"]`
-    care_site_id : List[int], optional
-        **EXAMPLE**: `[8312056386, 8312027648]`
-    start_date : datetime, optional
-        **EXAMPLE**: `"2019-05-01"`
-    end_date : datetime, optional
-        **EXAMPLE**: `"2021-07-01"`
-    care_site_short_name : List[int], optional
-        **EXAMPLE**: `"HOSPITAL XXXX"`
-    save_path : str, optional
-        Folder path where to save the chart in HTML format.
-
-        **EXAMPLE**: `"my_folder/my_file.html"`
-    x_axis_title: str, optional,
-        Label name for the x axis
-    y_axis_title: str, optional,
-        Label name for the y axis
-    show_per_care_site: bool, optional
-        If True, the average completeness predictor $c(t)$ is computed for each care site independently. If False, it is computed over all care sites.
-    labelFontSize: float, optional
-        The font size of the labels (axis and legend).
-    titleFontSize: float, optional
-        The font size of the titles.
+    completeness_predictor: str
+        Algorithm used to compute the completeness predictor
+        **EXAMPLE**: ``"per_visit_default"``
+    standard_terminologies: List[str]
+        List of standards terminologies to consider
+        **EXAMPLE**: ``["LOINC", "ANABIO"]``
+
+    Attributes
+    ----------
+    _completeness_predictor: str
+        Algorithm used to compute the completeness predictor
+        **VALUE**: ``"per_visit_default"``
+    _standard_terminologies: List[str]
+        List of standards terminologies to consider
+        **VALUE**: ``["LOINC", "ANABIO"]``
+    _index: List[str]
+        Variable from which data is grouped
+        **VALUE**: ``["care_site_level", "concepts_set", "stay_type", "length_of_stay", "care_site_id", "care_site_specialty", "specialties_set", "<std_terminology>_concept_code"]``
+    _viz_config: List[str]
+        Dictionary of configuration for visualization purpose.
+        **VALUE**: ``{}``
     """
 
-    predictor = probe.predictor.copy()
-    estimates = fitted_model.estimates.copy()
-    predictor = predictor.merge(estimates, on=probe._index)
-
-    def month_diff(x, y):
-        end = x.dt.to_period("M").view(dtype="int64")
-        start = y.dt.to_period("M").view(dtype="int64")
-        return end - start
-
-    predictor["date"] = predictor["date"].astype("datetime64[ns]")
-    predictor["t_0"] = predictor["t_0"].astype("datetime64[ns]")
-    predictor["normalized_date"] = month_diff(predictor["date"], predictor["t_0"])
-    predictor["t_0"] = predictor["t_0"].astype(str)
-    predictor["normalized_date"] = predictor["normalized_date"].astype(int)
-    if t_min:
-        predictor = predictor[predictor.normalized_date >= t_min]
-    if t_max:
-        predictor = predictor[predictor.normalized_date <= t_max]
-    predictor["normalized_c"] = predictor["c"].mask(
-        (predictor["normalized_date"] >= 0) & (predictor["c_0"] == 0), 1
-    )
-    predictor["normalized_c"] = predictor["normalized_c"].mask(
-        (predictor["normalized_date"] >= 0) & (predictor["c_0"] > 0),
-        predictor["c"] / predictor["c_0"],
-    )
-
-    predictor["legend_error_band"] = "Standard deviation"
-    predictor["legend_model"] = type(fitted_model).__name__
-
-    predictor["model"] = predictor["c_0"].where(predictor["normalized_date"] < 0, 1)
-    predictor["model"] = predictor["model"].where(predictor["normalized_date"] >= 0, 0)
-
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        predictor = predictor[predictor.date < predictor.t_1]
-
-    index = list(set(probe._index).difference(["care_site_level", "care_site_id"]))
-    if show_per_care_site:
-        index = index + ["care_site_short_name"]
-
-    predictor = filter_predictor(
-        predictor=predictor,
-        care_site_level=care_site_level,
-        stay_type=stay_type,
-        care_site_id=care_site_id,
-        care_site_short_name=care_site_short_name,
-        start_date=start_date,
-        end_date=end_date,
+    def __init__(
+        self,
+        completeness_predictor: str = "per_measurement_default",
+        standard_terminologies: List[str] = ["ANABIO", "LOINC"],
+    ):
+        self._standard_terminologies = standard_terminologies
+        self._index = [
+            "care_site_level",
+            "concepts_set",
+            "stay_type",
+            "length_of_stay",
+            "care_site_id",
+            "care_site_specialty",
+            "care_sites_set",
+            "specialties_set",
+        ] + [
+            "{}_concept_code".format(terminology)
+            for terminology in standard_terminologies
+        ]
+        super().__init__(
+            completeness_predictor=completeness_predictor,
+            index=self._index,
+        )
+
+    def compute_process(
+        self,
+        data: Data,
+        care_site_relationship: pd.DataFrame,
+        start_date: datetime,
+        end_date: datetime,
+        care_site_levels: List[str],
+        stay_types: Union[str, Dict[str, str]],
+        care_site_ids: List[int],
+        care_site_short_names: List[str] = None,
+        care_site_specialties: List[str] = None,
+        concept_codes: List[str] = None,
+        care_sites_sets: Union[str, Dict[str, str]] = None,
+        specialties_sets: Union[str, Dict[str, str]] = None,
+        concepts_sets: Union[str, Dict[str, str]] = {
+            "Leucocytes": "A0174|K3232|H6740|E4358|C9784|C8824|E6953",
+            "Plaquettes": "E4812|C0326|A1636|A0230|H6751|A1598|G7728|G7727|G7833|A2538|A2539|J4463",
+            "Créatinine": "E3180|G1974|J1002|A7813|A0094|G1975|J1172|G7834|F9409|F9410|C0697|H4038|F2621",
+            "Potassium": "A1656|C8757|C8758|A2380|E2073|L5014|F2618|E2337|J1178|A3819|J1181",
+            "Sodium": "A1772|C8759|C8760|A0262|J1177|F8162|L5013|F2617|K9086|J1180",
+            "Chlorure": "B5597|F2359|A0079|J1179|F2619|J1182|F2358|A0079|J1179|F2619|J1182",
+            "Glucose": "A1245|E7961|C8796|H7753|A8029|H7749|A0141|H7323|J7401|F2622|B9553|C7236|E7312|G9557|A7338|H7324|C0565|E9889|A8424|F6235|F5659|F2406",
+            "Bicarbonate": "A0422|H9622|C6408|F4161",
+        },
+        length_of_stays: List[float] = [1],
+        source_terminologies: Dict[str, str] = {
+            "ANALYSES_LABORATOIRE": r"Analyses Laboratoire",
+            "GLIMS_ANABIO": r"GLIMS.{0,20}Anabio",
+            "GLIMS_LOINC": r"GLIMS.{0,20}LOINC",
+            "ANABIO_ITM": r"ITM - ANABIO",
+            "LOINC_ITM": r"ITM - LOINC",
+        },
+        mapping: List[Tuple[str, str, str]] = [
+            ("ANALYSES_LABORATOIRE", "GLIMS_ANABIO", "Maps to"),
+            ("ANALYSES_LABORATOIRE", "GLIMS_LOINC", "Maps to"),
+            ("GLIMS_ANABIO", "ANABIO_ITM", "Mapped from"),
+            ("ANABIO_ITM", "LOINC_ITM", "Maps to"),
+        ],
         **kwargs,
-    )
-    index = [variable for variable in index if len(predictor[variable].unique()) >= 2]
-
-    if c_0_min:
-        c_0_min = round_it(float(c_0_min), 2)
-        if c_0_min > round_it(predictor.c_0.max(), 2):
-            c_0_min = round_it(predictor.c_0.max(), 2)
-        elif c_0_min < round_it(predictor.c_0.min(), 2):
-            c_0_min = round_it(predictor.c_0.min(), 2)
-    else:
-        c_0_min = round_it(predictor.c_0.min(), 2)
-
-    if error_max:
-        error_max = round_it(float(error_max), 2)
-        if error_max > predictor.error.max():
-            error_max = round_it(predictor.error.max(), 2)
-        elif error_max < round_it(predictor.error.min(), 2):
-            error_max = round_it(predictor.error.min(), 2)
-    else:
-        error_max = round_it(predictor.error.max(), 2)
-
-    t_0_max = (
-        str(pd.to_datetime(t_0_max)) if t_0_max else predictor.t_0.astype(str).max()
-    )
-
-    c_0_min_slider = alt.binding_range(
-        min=0,
-        max=round_it(predictor.c_0.max(), 2),
-        step=1 / 100,
-        name="c₀ min: ",
-    )
-    c_0_min_selection = alt.selection_single(
-        name="c_0_min",
-        fields=["c_0_min"],
-        bind=c_0_min_slider,
-        init={"c_0_min": c_0_min},
-    )
-    t_0_slider = alt.binding(
-        input="t_0",
-        name="t₀ max: ",
-    )
-    t_0_selection = alt.selection_single(
-        name="t_0",
-        fields=["t_0"],
-        bind=t_0_slider,
-        init={"t_0": t_0_max},
-    )
-    if fitted_model.name == "RectangleFunction":
-        t_1_min = (
-            str(pd.to_datetime(t_1_min)) if t_1_min else predictor.t_1.astype(str).min()
-        )
-        t_1_slider = alt.binding(
-            input="t_1",
-            name="t₁ min: ",
-        )
-        t_1_selection = alt.selection_single(
-            name="t_1",
-            fields=["t_1"],
-            bind=t_1_slider,
-            init={"t_1": t_1_min},
-        )
-    error_max_slider = alt.binding_range(
-        min=round_it(predictor.error.min(), 2),
-        max=round_it(predictor.error.max(), 2),
-        step=scale_it(predictor.error.max()) / 100,
-        name="error max: ",
-    )
-    error_max_selection = alt.selection_single(
-        name="error_max",
-        fields=["error_max"],
-        bind=error_max_slider,
-        init={"error_max": error_max},
-    )
-
-    alt.data_transformers.disable_max_rows()
-
-    base_chart = (
-        alt.Chart(predictor).encode(
-            x=alt.X(
-                "normalized_date:Q",
-                title=x_axis_title,
-                scale=alt.Scale(nice=False),
-            ),
-        )
-    ).properties(width=900, height=300)
+    ):
+        """Script to be used by [``compute()``][edsteva.probes.base.BaseProbe.compute]
 
-    transform_chart = (
-        base_chart.transform_joinaggregate(
-            mean_c_0="mean(c_0)",
-            mean_error="mean(error)",
-            groupby=["care_site_short_name"] + index,
-        )
-        .transform_filter(alt.datum.mean_c_0 >= c_0_min_selection.c_0_min)
-        .transform_filter(alt.datum.mean_error <= error_max_selection.error_max)
-        .transform_filter(alt.datum.t_0 <= t_0_selection.t_0)
-    )
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        transform_chart = transform_chart.transform_filter(
-            alt.datum.t_1 >= t_1_selection.t_1
-        )
-
-    mean_line = transform_chart.mark_line().encode(
-        y=alt.Y(
-            "mean(normalized_c):Q",
-        )
-    )
-
-    error_line = transform_chart.mark_errorband(extent="stdev").encode(
-        y=alt.Y(
-            "normalized_c:Q",
-            title=y_axis_title,
-        ),
-        stroke=alt.Stroke(
-            "legend_error_band",
-            title="Error band",
-            legend=alt.Legend(symbolType="square", orient="top"),
-        ),
-    )
-
-    model_line = base_chart.mark_line(
-        color="black", interpolate="step-after", strokeDash=[5, 5]
-    ).encode(
-        y="model:Q",
-        strokeWidth=alt.StrokeWidth(
-            "legend_model",
-            title="Model line",
-            legend=alt.Legend(orient="top", symbolDash=[2, 2]),
-        ),
-    )
-
-    chart = mean_line + error_line + model_line
-
-    if len(index) >= 2:
-        index_selection = alt.selection_single(
-            fields=["index"],
-            bind=alt.binding_radio(name="Group by: ", options=index),
-            init={"index": index[0]},
-        )
-        chart = (
-            chart.transform_fold(index, as_=["index", "value"])
-            .encode(
-                color=alt.Color(
-                    "value:N",
-                    sort={"field": "c_0", "op": "min", "order": "descending"},
-                    title=None,
-                ),
-            )
-            .transform_filter(index_selection)
-            .add_selection(index_selection)
-        )
-
-    elif len(index) == 1:
-        chart = chart.encode(
-            color=alt.Color(
-                "{}:N".format(index[0]),
-                sort={"field": "c_0", "op": "min", "order": "descending"},
-            ),
-        )
-
-    chart = (
-        chart.add_selection(error_max_selection)
-        .add_selection(c_0_min_selection)
-        .add_selection(t_0_selection)
-    )
-    # RectangleModel
-    if fitted_model.name == "RectangleFunction":
-        chart = chart.add_selection(t_1_selection)
-
-    if save_path:
-        save_html(
-            obj=chart.configure_axis(
-                labelFontSize=labelFontSize, titleFontSize=titleFontSize
-            ).configure_legend(labelFontSize=labelFontSize),
-            filename=save_path,
-        )
+        Parameters
+        ----------
+        data : Data
+            Instantiated [``HiveData``][edsteva.io.hive.HiveData], [``PostgresData``][edsteva.io.postgres.PostgresData] or [``LocalData``][edsteva.io.files.LocalData]
+        care_site_relationship : pd.DataFrame
+            DataFrame computed in the [``compute()``][edsteva.probes.base.BaseProbe.compute] that gives the hierarchy of the care site structure.
+        start_date : datetime, optional
+            **EXAMPLE**: `"2019-05-01"`
+        end_date : datetime, optional
+            **EXAMPLE**: `"2021-07-01"`
+        care_site_levels : List[str], optional
+            **EXAMPLE**: `["Hospital", "Pole", "UF"]`
+        stay_types : Union[str, Dict[str, str]], optional
+            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "Urg_and_consult": "urgences|consultation"}` or `"hospitalisés`
+        care_site_ids : List[int], optional
+            **EXAMPLE**: `[8312056386, 8312027648]`
+        care_site_short_names : List[str], optional
+            **EXAMPLE**: `["HOSPITAL 1", "HOSPITAL 2"]`
+        care_site_specialties : List[str], optional
+            **EXAMPLE**: `["CARDIOLOGIE", "CHIRURGIE"]`
+        concept_codes : List[str], optional
+            **EXAMPLE**: ['E3180', 'G1974', 'J1002', 'A7813', 'A0094', 'G1975', 'J1172', 'G7834', 'F9409', 'F9410', 'C0697', 'H4038']`
+        care_sites_sets : Union[str, Dict[str, str]], optional
+            **EXAMPLE**: `{"All AP-HP": ".*"}` or `{"All AP-HP": ".*", "Pediatrics": r"debre|trousseau|necker"}`
+        specialties_sets : Union[str, Dict[str, str]], optional
+            **EXAMPLE**: `{"All": ".*"}` or `{"All": ".*", "ICU": r"REA\s|USI\s|SC\s"}`
+        concepts_sets : Union[str, Dict[str, str]], optional
+            **EXAMPLE**: `{"Créatinine": "E3180|G1974|J1002|A7813|A0094|G1975|J1172|G7834|F9409|F9410|C0697|H4038|F2621", "Leucocytes": r"A0174|K3232|H6740|E4358|C9784|C8824|E6953"}`
+        length_of_stays : List[float], optional
+            **EXAMPLE**: `[1, 30]`
+        source_terminologies : Dict[str, str], optional
+            Dictionary of regex used to detect terminology in the column `vocabulary_id`.
+            **EXAMPLE**: `{"GLIMS_LOINC": r"GLIMS.{0,20}LOINC"}`
+        mapping : List[Tuple[str, str, str]], optional
+            List of values to filter in the column `relationship_id` in order to map between 2 terminologies.
+            **EXAMPLE**: `[("ANALYSES_LABORATOIRE", "GLIMS_ANABIO", "Maps to")]`
+        """
+        if specialties_sets is None and "specialties_set" in self._index:
+            self._index.remove("specialties_set")
+        if length_of_stays is None and "length_of_stay" in self._index:
+            self._index.remove("length_of_stay")
+        if care_sites_sets is None and "care_sites_set" in self._index:
+            self._index.remove("care_sites_set")
+        if concepts_sets is None and "concepts_set" in self._index:
+            self._index.remove("concepts_set")
+        else:
+            for terminology in self._standard_terminologies:
+                if "{}_concept_code".format(terminology) in self._index:
+                    self._index.remove("{}_concept_code".format(terminology))
+
+        return completeness_predictors.get(self._completeness_predictor)(
+            self,
+            data=data,
+            care_site_relationship=care_site_relationship,
+            start_date=start_date,
+            end_date=end_date,
+            care_site_levels=care_site_levels,
+            stay_types=stay_types,
+            care_site_ids=care_site_ids,
+            care_site_short_names=care_site_short_names,
+            care_site_specialties=care_site_specialties,
+            concept_codes=concept_codes,
+            care_sites_sets=care_sites_sets,
+            specialties_sets=specialties_sets,
+            concepts_sets=concepts_sets,
+            length_of_stays=length_of_stays,
+            source_terminologies=source_terminologies,
+            mapping=mapping,
+            **kwargs,
+        )
+
+    def get_viz_config(self, viz_type: str, **kwargs):
+        if viz_type in viz_configs.keys():
+            _viz_config = self._viz_config.get(viz_type)
+            if _viz_config is None:
+                _viz_config = self._completeness_predictor
+        else:
+            raise ValueError(f"edsteva has no {viz_type} registry !")
+        return viz_configs[viz_type].get(_viz_config)(self, **kwargs)
 
-    return chart
+    def available_completeness_predictors(self):
+        return list(completeness_predictors.get_all().keys())
```

### Comparing `edsteva-0.1.4/pyproject.toml` & `edsteva-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edsteva"
-version = "0.1.4"
+version = "0.2.0"
 description = "EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records."
 authors = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Benoit Playe <benoit.playe@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>", "Paul Bernard <paul.bernard@aphp.fr>"]
 keywords = ["OMOP", "Data Analysis", "Electronic health record"]
 readme = "README.md"
 maintainers = ["Adam Remaki <adam.remaki@aphp.fr>", "Vicent Maladiere <vincent.maladiere-ext@aphp.fr>", "Thomas Petit-Jean <thomas.petitjean@aphp.fr>", "Romain Bey <romain.bey@aphp.fr>"]
 homepage = "https://github.com/aphp/edsteva"
 repository = "https://github.com/aphp/edsteva"
@@ -23,29 +23,29 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/aphp/edsteva/issues"
 
 [tool.poetry.dependencies]
 python = "~3.7.1"
 pyspark = "~2.4.3"
 pandas = "^1.3"
-altair = "^4.2"
+altair = "^5.0"
 numpy = "<1.20.0" # https://github.com/databricks/koalas/pull/2166
-loguru = "0.6.0"
+loguru = "0.7.0"
 ipython = "^7.31.0"
 koalas = "^1.8.2"
 pgpasslib = "^1.1.0"
 psycopg2-binary = "^2.9.3"
 pyarrow = ">=0.15, <0.17.0"
+catalogue = "^2.0.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pre-commit = "^2.17.0"
 ipykernel = "^6.15.3"
-nb-black = "^1.0.7"
-jupyterlab-rise = "0.1.0"
+jupyterlab-rise = "0.2.0"
 jupyterlab = "^3.0.0"
 
 [tool.poetry.group.docs.dependencies]
 pypandoc = "1.7.5"
 markdown = "^3.3.4"
 mkdocs-autorefs = "0.4.1"
 mkdocs-bibtex = "^2.0.1"
@@ -61,38 +61,58 @@
 jinja2 = "~3.0.0"
 mkdocstrings = "0.19.0"
 mkdocstrings-python = "0.8.2"
 mknotebooks = "0.7.1"
 mike = "^1.1.2"
 
 [tool.poetry.group.test.dependencies]
-flake8 = "^3.0.1"
+ruff = "0.0.241"
 pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-html = "^3.1.1"
 pylic = "^3.4.0"
 
+[tool.ruff]
+ignore = ["E501"]
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".eggs",
+    ".git",
+    ".gitignore",
+    ".ruff_cache",
+    ".tox",
+    ".venv",
+    ".pytest_cache",
+    ".ipynb_checkpoints",
+    "__pycache__",
+    "__init__.py",
+    "dist",
+    "node_modules",
+    "venv",
+]
+
 [tool.pylic]
 safe_licenses = [
   "BSD License",
   "BSD 3-Clause",
+  "BSD 3-Clause License",
   "BSD-3-Clause-LBNL",
   "BSD",
   "The Unlicense (Unlicense)",
   "ISC",
   "ISC License (ISCL)",
   "Apache Software License",
   "MIT",
   "MIT License",
   "Python Software Foundation License",
   "Apache License 2.0",
   "http://www.apache.org/licenses/LICENSE-2.0",
   "Mozilla Public License 2.0 (MPL 2.0)",
-  "MPL-2.0",
   "Eclipse Public License 2.0 (EPL-2.0)",
   "GNU Library or Lesser General Public License (LGPL)",
 ]
+unsafe_packages  = ["ypy-websocket"]
 ignore_packages = ["pgpasslib"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `edsteva-0.1.4/setup.py` & `edsteva-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,109 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: edsteva
+Version: 0.2.0
+Summary: EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.
+Home-page: https://github.com/aphp/edsteva
+License: BSD 3-Clause
+Keywords: OMOP,Data Analysis,Electronic health record
+Author: Adam Remaki
+Author-email: adam.remaki@aphp.fr
+Maintainer: Adam Remaki
+Maintainer-email: adam.remaki@aphp.fr
+Requires-Python: >=3.7.1,<3.8.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: altair (>=5.0,<6.0)
+Requires-Dist: catalogue (>=2.0.8,<3.0.0)
+Requires-Dist: ipython (>=7.31.0,<8.0.0)
+Requires-Dist: koalas (>=1.8.2,<2.0.0)
+Requires-Dist: loguru (==0.7.0)
+Requires-Dist: numpy (<1.20.0)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pgpasslib (>=1.1.0,<2.0.0)
+Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
+Requires-Dist: pyarrow (>=0.15,<0.17.0)
+Requires-Dist: pyspark (>=2.4.3,<2.5.0)
+Project-URL: Bug Tracker, https://github.com/aphp/edsteva/issues
+Project-URL: Documentation, https://aphp.github.io/edsteva/latest/
+Project-URL: Repository, https://github.com/aphp/edsteva
+Description-Content-Type: text/markdown
+
+<p align="center">
+<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>
+</p>
+
+<div align="center">
+
+<p align="center">
+  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>
+</p>
+
+# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)
+
+<p align="center">
+<a href="https://aphp.github.io/edsteva/latest/" target="_blank">
+    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">
+</a>
+<a href="https://pypi.org/project/edsteva/" target="_blank">
+    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">
+</a>
+<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">
+    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">
+</a>
+<a href="https://github.com/psf/black" target="_blank">
+    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
+</a>
+<a href="https://python-poetry.org/" target="_blank">
+    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">
+</a>
+<a href="https://www.python.org/" target="_blank">
+    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">
+</a>
+</p>
+</div>
+
+**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>
+
+**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>
+
+---
+
+EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.
+
+## Requirements
+EDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:
+
+- Python ~3.7.1
+- Java 8
+
+## Installation
+
+You can install EDS-TeVa through ``pip``:
+
+```shell
+pip install edsteva
+```
+We recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).
+
+```
+pip install edsteva==0.2.0
+```
+## Example
+
+A scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.
 
-packages = \
-['edsteva',
- 'edsteva.io',
- 'edsteva.io.synthetic',
- 'edsteva.metrics',
- 'edsteva.models',
- 'edsteva.models.rectangle_function',
- 'edsteva.models.rectangle_function.algos',
- 'edsteva.models.step_function',
- 'edsteva.models.step_function.algos',
- 'edsteva.probes',
- 'edsteva.utils',
- 'edsteva.viz',
- 'edsteva.viz.dashboards',
- 'edsteva.viz.dashboards.predictor_dashboard',
- 'edsteva.viz.plots',
- 'edsteva.viz.plots.plot_probe']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['altair>=4.2,<5.0',
- 'ipython>=7.31.0,<8.0.0',
- 'koalas>=1.8.2,<2.0.0',
- 'loguru==0.6.0',
- 'numpy<1.20.0',
- 'pandas>=1.3,<2.0',
- 'pgpasslib>=1.1.0,<2.0.0',
- 'psycopg2-binary>=2.9.3,<3.0.0',
- 'pyarrow>=0.15,<0.17.0',
- 'pyspark>=2.4.3,<2.5.0']
-
-setup_kwargs = {
-    'name': 'edsteva',
-    'version': '0.1.4',
-    'description': 'EDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.',
-    'long_description': '<p align="center">\n<b>DISCLAIMER: </b>EDS-TeVa is intended to be a module of <a href="https://github.com/aphp/EDS-Scikit">EDS-Scikit</a>\n</p>\n\n<div align="center">\n\n<p align="center">\n  <a href="https://aphp.github.io/edsteva/latest/"><img src="https://aphp.github.io/edsteva/latest/assets/logo/edsteva_logo_small.svg" alt="EDS-TeVa"></a>\n</p>\n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n<p align="center">\n<a href="https://aphp.github.io/edsteva/latest/" target="_blank">\n    <img src="https://img.shields.io/github/actions/workflow/status/aphp/edsteva/documentation.yaml?branch=main&label=docs&style=flat" alt="Documentation">\n</a>\n<a href="https://pypi.org/project/edsteva/" target="_blank">\n    <img src="https://img.shields.io/pypi/v/edsteva?color=blue&style=flat" alt="PyPI">\n</a>\n<a href="https://codecov.io/github/aphp/edsteva?branch=main" target="_blank">\n    <img src="https://codecov.io/github/aphp/edsteva/coverage.svg?branch=main" alt="Codecov">\n</a>\n<a href="https://github.com/psf/black" target="_blank">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n</a>\n<a href="https://python-poetry.org/" target="_blank">\n    <img src="https://img.shields.io/badge/reproducibility-poetry-blue" alt="Poetry">\n</a>\n<a href="https://www.python.org/" target="_blank">\n    <img src="https://img.shields.io/badge/python-~3.7.1-brightgreen" alt="Supported Python versions">\n</a>\n</p>\n</div>\n\n**Documentation**: <a href="https://aphp.github.io/edsteva/latest/" target="_blank">https://aphp.github.io/edsteva/latest/</a>\n\n**Source Code**: <a href="https://github.com/aphp/edsteva" target="_blank">https://github.com/aphp/edsteva</a>\n\n---\n\nEDS-TeVa provides a set of tools that aims at modeling the adoption over time and across space of the Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning the library version in your projects, or use a strict package manager like [Poetry](https://python-poetry.org/).\n\n```\npip install edsteva==0.1.4\n```\n## Example\n\nA scientific paper is currently being written that describes extensively the use of the library on the study of pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.\n\n## Acknowledgement\n\nWe would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
-    'author': 'Adam Remaki',
-    'author_email': 'adam.remaki@aphp.fr',
-    'maintainer': 'Adam Remaki',
-    'maintainer_email': 'adam.remaki@aphp.fr',
-    'url': 'https://github.com/aphp/edsteva',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.8.0',
-}
+## Contributing
 
+Contributions are welcome, and they are greatly appreciated! Every little bit helps, and credit will always be given.
+
+## Acknowledgement
+
+We would like to thank [Assistance Publique – Hôpitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation](https://fondationrechercheaphp.fr/) for funding this project.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,45 +1,41 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['edsteva',
-'edsteva.io', 'edsteva.io.synthetic', 'edsteva.metrics', 'edsteva.models',
-'edsteva.models.rectangle_function', 'edsteva.models.rectangle_function.algos',
-'edsteva.models.step_function', 'edsteva.models.step_function.algos',
-'edsteva.probes', 'edsteva.utils', 'edsteva.viz', 'edsteva.viz.dashboards',
-'edsteva.viz.dashboards.predictor_dashboard', 'edsteva.viz.plots',
-'edsteva.viz.plots.plot_probe'] package_data = \ {'': ['*']} install_requires =
-\ ['altair>=4.2,<5.0', 'ipython>=7.31.0,<8.0.0', 'koalas>=1.8.2,<2.0.0',
-'loguru==0.6.0', 'numpy<1.20.0', 'pandas>=1.3,<2.0', 'pgpasslib>=1.1.0,<2.0.0',
-'psycopg2-binary>=2.9.3,<3.0.0', 'pyarrow>=0.15,<0.17.0',
-'pyspark>=2.4.3,<2.5.0'] setup_kwargs = { 'name': 'edsteva', 'version':
-'0.1.4', 'description': 'EDS-TeVa provides a set of tools that aims at modeling
-the adoption over time and across space of the Electronic Health Records.',
-'long_description': '
-       \nDISCLAIMER:EDS-TeVa is intended to be a module of EDS-Scikit\n
-\n\n
-                                     \n\n
-                                \n [EDS-TeVa]\n
-   \n\n# EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://
-                       mybinder.org/v2/gh/aphp/edsteva/
-              HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)\n\n
-    \n\n_[Documentation]\n\n\n_[PyPI]\n\n\n_[Codecov]\n\n\n_[Black]\n\n\n_
-                [Poetry]\n\n\n_[Supported_Python_versions]\n\n
-                                      \n
-\n\n**Documentation**: https://aphp.github.io/edsteva/latest/\n\n**Source
-Code**: https://github.com/aphp/edsteva\n\n---\n\nEDS-TeVa provides a set of
-tools that aims at modeling the adoption over time and across space of the
-Electronic Health Records.\n\n## Requirements\nEDS-TeVa stands on the shoulders
-of [Spark 2.4](https://spark.apache.org/docs/2.4.8/index.html) which requires:
-\n\n- Python ~3.7.1\n- Java 8\n\n## Installation\n\nYou can install EDS-TeVa
-through ``pip``:\n\n```shell\npip install edsteva\n```\nWe recommend pinning
-the library version in your projects, or use a strict package manager like
-[Poetry](https://python-poetry.org/).\n\n```\npip install
-edsteva==0.1.4\n```\n## Example\n\nA scientific paper is currently being
+Metadata-Version: 2.1 Name: edsteva Version: 0.2.0 Summary: EDS-TeVa provides a
+set of tools that aims at modeling the adoption over time and across space of
+the Electronic Health Records. Home-page: https://github.com/aphp/edsteva
+License: BSD 3-Clause Keywords: OMOP,Data Analysis,Electronic health record
+Author: Adam Remaki Author-email: adam.remaki@aphp.fr Maintainer: Adam Remaki
+Maintainer-email: adam.remaki@aphp.fr Requires-Python: >=3.7.1,<3.8.0
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Software Development :: Libraries Requires-Dist: altair
+(>=5.0,<6.0) Requires-Dist: catalogue (>=2.0.8,<3.0.0) Requires-Dist: ipython
+(>=7.31.0,<8.0.0) Requires-Dist: koalas (>=1.8.2,<2.0.0) Requires-Dist: loguru
+(==0.7.0) Requires-Dist: numpy (<1.20.0) Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: pgpasslib (>=1.1.0,<2.0.0) Requires-Dist: psycopg2-binary
+(>=2.9.3,<3.0.0) Requires-Dist: pyarrow (>=0.15,<0.17.0) Requires-Dist: pyspark
+(>=2.4.3,<2.5.0) Project-URL: Bug Tracker, https://github.com/aphp/edsteva/
+issues Project-URL: Documentation, https://aphp.github.io/edsteva/latest/
+Project-URL: Repository, https://github.com/aphp/edsteva Description-Content-
+Type: text/markdown
+         DISCLAIMER:EDS-TeVa is intended to be a module of EDS-Scikit
+                                  [EDS-TeVa]
+     # EDS-TeVa [![Binder](https://mybinder.org/badge_logo.svg)](https://
+mybinder.org/v2/gh/aphp/edsteva/HEAD?labpath=notebooks%2Fsynthetic_data.ipynb)
+ [Documentation] [PyPI] [Codecov] [Black] [Poetry] [Supported_Python_versions]
+**Documentation**: https://aphp.github.io/edsteva/latest/ **Source Code**:
+https://github.com/aphp/edsteva --- EDS-TeVa provides a set of tools that aims
+at modeling the adoption over time and across space of the Electronic Health
+Records. ## Requirements EDS-TeVa stands on the shoulders of [Spark 2.4](https:
+//spark.apache.org/docs/2.4.8/index.html) which requires: - Python ~3.7.1 -
+Java 8 ## Installation You can install EDS-TeVa through ``pip``: ```shell pip
+install edsteva ``` We recommend pinning the library version in your projects,
+or use a strict package manager like [Poetry](https://python-poetry.org/). ```
+pip install edsteva==0.2.0 ``` ## Example A scientific paper is currently being
 written that describes extensively the use of the library on the study of
-pulmonary embolism of cancer patients.\n\n## Contributing\n\nContributions are
+pulmonary embolism of cancer patients. ## Contributing Contributions are
 welcome, and they are greatly appreciated! Every little bit helps, and credit
-will always be given.\n\n## Acknowledgement\n\nWe would like to thank
-[Assistance Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP
-Foundation](https://fondationrechercheaphp.fr/) for funding this project.\n',
-'author': 'Adam Remaki', 'author_email': 'adam.remaki@aphp.fr', 'maintainer':
-'Adam Remaki', 'maintainer_email': 'adam.remaki@aphp.fr', 'url': 'https://
-github.com/aphp/edsteva', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7.1,<3.8.0', }
-setup(**setup_kwargs)
+will always be given. ## Acknowledgement We would like to thank [Assistance
+Publique â HÃ´pitaux de Paris](https://www.aphp.fr/) and [AP-HP Foundation]
+(https://fondationrechercheaphp.fr/) for funding this project.
```

