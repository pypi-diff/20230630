# Comparing `tmp/pm4py-2.7.4.tar.gz` & `tmp/pm4py-2.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pm4py-2.7.4.tar", last modified: Mon May  8 08:14:56 2023, max compression
+gzip compressed data, was "pm4py-2.7.5.tar", last modified: Fri Jun 30 14:33:07 2023, max compression
```

## Comparing `pm4py-2.7.4.tar` & `pm4py-2.7.5.tar`

### file list

```diff
@@ -1,1658 +1,1666 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.694383 pm4py-2.7.4/
--rw-rw-rw-   0        0        0    34817 2023-03-27 13:12:16.000000 pm4py-2.7.4/LICENSE
--rw-rw-rw-   0        0        0     2683 2023-05-08 08:14:56.694383 pm4py-2.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     2249 2023-05-08 08:14:47.000000 pm4py-2.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.826360 pm4py-2.7.4/pm4py/
--rw-rw-rw-   0        0        0     7281 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.873230 pm4py-2.7.4/pm4py/algo/
--rw-rw-rw-   0        0        0      854 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.873230 pm4py-2.7.4/pm4py/algo/analysis/
--rw-rw-rw-   0        0        0      833 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.873230 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.888853 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/variants/
--rw-rw-rw-   0        0        0      810 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    21448 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.888853 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/__init__.py
--rw-rw-rw-   0        0        0     2689 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.888853 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/variants/__init__.py
--rw-rw-rw-   0        0        0    11636 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/marking_equation/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.904473 pm4py-2.7.4/pm4py/algo/analysis/woflan/
--rw-rw-rw-   0        0        0      836 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/__init__.py
--rw-rw-rw-   0        0        0    32365 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.904473 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/
--rw-rw-rw-   0        0        0      868 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.920095 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
--rw-rw-rw-   0        0        0      835 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     7988 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.920095 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
--rw-rw-rw-   0        0        0     2451 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.926606 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
--rw-rw-rw-   0        0        0      841 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
--rw-rw-rw-   0        0        0     4061 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
--rw-rw-rw-   0        0        0     5745 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/utility.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.926606 pm4py-2.7.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
--rw-rw-rw-   0        0        0     2632 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.942237 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/
--rw-rw-rw-   0        0        0      849 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py
--rw-rw-rw-   0        0        0     4269 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
--rw-rw-rw-   0        0        0     3668 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py
--rw-rw-rw-   0        0        0     1098 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
--rw-rw-rw-   0        0        0     8245 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/utility.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.942237 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/__init__.py
--rw-rw-rw-   0        0        0     1565 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.957859 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/variants/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3257 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.957859 pm4py-2.7.4/pm4py/algo/anonymization/
--rw-rw-rw-   0        0        0      967 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.957859 pm4py-2.7.4/pm4py/algo/anonymization/pripel/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/__init__.py
--rw-rw-rw-   0        0        0     3170 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.973479 pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/
--rw-rw-rw-   0        0        0    13889 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
--rw-rw-rw-   0        0        0    14468 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
--rw-rw-rw-   0        0        0      837 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/__init__.py
--rw-rw-rw-   0        0        0     1754 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.973479 pm4py-2.7.4/pm4py/algo/anonymization/pripel/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/variants/__init__.py
--rw-rw-rw-   0        0        0     5291 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/pripel/variants/pripel.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.973479 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.989101 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/
--rw-rw-rw-   0        0        0      839 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
--rw-rw-rw-   0        0        0     6862 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
--rw-rw-rw-   0        0        0     1323 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
--rw-rw-rw-   0        0        0     1687 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.004723 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/
--rw-rw-rw-   0        0        0      817 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
--rw-rw-rw-   0        0        0     7677 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
--rw-rw-rw-   0        0        0    11317 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.004723 pm4py-2.7.4/pm4py/algo/clustering/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.004723 pm4py-2.7.4/pm4py/algo/clustering/profiles/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/profiles/__init__.py
--rw-rw-rw-   0        0        0     2118 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.004723 pm4py-2.7.4/pm4py/algo/clustering/profiles/variants/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/profiles/variants/__init__.py
--rw-rw-rw-   0        0        0     3544 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.020343 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/
--rw-rw-rw-   0        0        0      984 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py
--rw-rw-rw-   0        0        0     4712 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.026852 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/dfg/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
--rw-rw-rw-   0        0        0     3892 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.026852 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
--rw-rw-rw-   0        0        0     5473 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.026852 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
--rw-rw-rw-   0        0        0    13583 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.042480 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
--rw-rw-rw-   0        0        0     4290 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.042480 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/
--rw-rw-rw-   0        0        0      824 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
--rw-rw-rw-   0        0        0     3396 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
--rw-rw-rw-   0        0        0    15534 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.058100 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/
--rw-rw-rw-   0        0        0      855 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
--rw-rw-rw-   0        0        0    18357 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
--rw-rw-rw-   0        0        0     6772 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
--rw-rw-rw-   0        0        0     6295 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
--rw-rw-rw-   0        0        0    15717 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.058100 pm4py-2.7.4/pm4py/algo/comparison/
--rw-rw-rw-   0        0        0      940 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/comparison/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.073722 pm4py-2.7.4/pm4py/algo/comparison/petrinet/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/comparison/petrinet/__init__.py
--rw-rw-rw-   0        0        0     6739 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.073722 pm4py-2.7.4/pm4py/algo/conformance/
--rw-rw-rw-   0        0        0      946 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.073722 pm4py-2.7.4/pm4py/algo/conformance/alignments/
--rw-rw-rw-   0        0        0      838 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.073722 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/__init__.py
--rw-rw-rw-   0        0        0     2025 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.089344 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/variants/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
--rw-rw-rw-   0        0        0    19023 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.089344 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/__init__.py
--rw-rw-rw-   0        0        0     1956 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.089344 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/variants/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    20411 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.104964 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/
--rw-rw-rw-   0        0        0      918 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py
--rw-rw-rw-   0        0        0     1876 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.104964 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/variants/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     7202 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.127094 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/__init__.py
--rw-rw-rw-   0        0        0    17405 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.127094 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/utils/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0     2896 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.158345 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/
--rw-rw-rw-   0        0        0      925 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0    27653 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17218 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    23651 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
--rw-rw-rw-   0        0        0    23624 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
--rw-rw-rw-   0        0        0    17546 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
--rw-rw-rw-   0        0        0    24029 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
--rw-rw-rw-   0        0        0    27972 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.173967 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/__init__.py
--rw-rw-rw-   0        0        0     2279 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.205209 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/
--rw-rw-rw-   0        0        0      870 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
--rw-rw-rw-   0        0        0    15712 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.220829 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/
--rw-rw-rw-   0        0        0      833 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.242969 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
--rw-rw-rw-   0        0        0      871 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
--rw-rw-rw-   0        0        0     5361 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
--rw-rw-rw-   0        0        0    49808 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
--rw-rw-rw-   0        0        0    36425 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
--rw-rw-rw-   0        0        0     6660 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
--rw-rw-rw-   0        0        0    17913 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.242969 pm4py-2.7.4/pm4py/algo/conformance/antialignments/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/antialignments/__init__.py
--rw-rw-rw-   0        0        0     3166 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/antialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.258586 pm4py-2.7.4/pm4py/algo/conformance/antialignments/variants/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/antialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     7582 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.258586 pm4py-2.7.4/pm4py/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     2073 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.274208 pm4py-2.7.4/pm4py/algo/conformance/footprints/util/
--rw-rw-rw-   0        0        0      817 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/util/__init__.py
--rw-rw-rw-   0        0        0     6154 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/util/evaluation.py
--rw-rw-rw-   0        0        0     3573 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/util/tree_visualization.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.289829 pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      832 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/log_extensive.py
--rw-rw-rw-   0        0        0     5095 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/log_model.py
--rw-rw-rw-   0        0        0     7117 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.305451 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.305451 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/variants/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    13187 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.321587 pm4py-2.7.4/pm4py/algo/conformance/multialignments/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/multialignments/__init__.py
--rw-rw-rw-   0        0        0     3143 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/multialignments/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.327593 pm4py-2.7.4/pm4py/algo/conformance/multialignments/variants/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/multialignments/variants/__init__.py
--rw-rw-rw-   0        0        0     6557 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.327593 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     4645 2023-04-26 05:58:14.000000 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.343223 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/
--rw-rw-rw-   0        0        0      929 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     5418 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5999 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.343223 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/
--rw-rw-rw-   0        0        0      815 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/__init__.py
--rw-rw-rw-   0        0        0     3041 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.358844 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/
--rw-rw-rw-   0        0        0      836 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
--rw-rw-rw-   0        0        0     6439 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
--rw-rw-rw-   0        0        0    10823 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.358844 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py
--rw-rw-rw-   0        0        0    12117 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py
--rw-rw-rw-   0        0        0    59010 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.374468 pm4py-2.7.4/pm4py/algo/connectors/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.374468 pm4py-2.7.4/pm4py/algo/connectors/util/
--rw-rw-rw-   0        0        0      781 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/util/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/util/mail.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.405708 pm4py-2.7.4/pm4py/algo/connectors/variants/
--rw-rw-rw-   0        0        0      736 2023-03-28 09:25:12.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/__init__.py
--rw-rw-rw-   0        0        0     2556 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/camunda_workflow.py
--rw-rw-rw-   0        0        0     3645 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/chrome_history.py
--rw-rw-rw-   0        0        0     3598 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/firefox_history.py
--rw-rw-rw-   0        0        0     5034 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/github_repo.py
--rw-rw-rw-   0        0        0     4166 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/outlook_calendar.py
--rw-rw-rw-   0        0        0     4354 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py
--rw-rw-rw-   0        0        0     3132 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/sap_accounting.py
--rw-rw-rw-   0        0        0     3976 2023-03-28 05:40:06.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/sap_o2c.py
--rw-rw-rw-   0        0        0     4110 2023-03-27 13:13:01.000000 pm4py-2.7.4/pm4py/algo/connectors/variants/windows_events.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.405708 pm4py-2.7.4/pm4py/algo/decision_mining/
--rw-rw-rw-   0        0        0      888 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/decision_mining/__init__.py
--rw-rw-rw-   0        0        0    23391 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/decision_mining/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.405708 pm4py-2.7.4/pm4py/algo/discovery/
--rw-rw-rw-   0        0        0     1035 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.421329 pm4py-2.7.4/pm4py/algo/discovery/alpha/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/__init__.py
--rw-rw-rw-   0        0        0     4784 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.427836 pm4py-2.7.4/pm4py/algo/discovery/alpha/data_structures/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/data_structures/__init__.py
--rw-rw-rw-   0        0        0     2420 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.427836 pm4py-2.7.4/pm4py/algo/discovery/alpha/utils/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/utils/__init__.py
--rw-rw-rw-   0        0        0     1622 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/utils/endpoints.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.427836 pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/__init__.py
--rw-rw-rw-   0        0        0    10923 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/classic.py
--rw-rw-rw-   0        0        0    22108 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/plus.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.443464 pm4py-2.7.4/pm4py/algo/discovery/batches/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/__init__.py
--rw-rw-rw-   0        0        0     3724 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.443464 pm4py-2.7.4/pm4py/algo/discovery/batches/utils/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/utils/__init__.py
--rw-rw-rw-   0        0        0     9636 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/utils/detection.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.459087 pm4py-2.7.4/pm4py/algo/discovery/batches/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/variants/__init__.py
--rw-rw-rw-   0        0        0     5216 2023-03-27 13:12:16.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/variants/log.py
--rw-rw-rw-   0        0        0     6111 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/batches/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.459087 pm4py-2.7.4/pm4py/algo/discovery/causal/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/causal/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/causal/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.459087 pm4py-2.7.4/pm4py/algo/discovery/causal/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/causal/variants/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/causal/variants/alpha.py
--rw-rw-rw-   0        0        0     1611 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/causal/variants/heuristic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.474706 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/__init__.py
--rw-rw-rw-   0        0        0     2249 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/algorithm.py
--rw-rw-rw-   0        0        0     7934 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.490327 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/
--rw-rw-rw-   0        0        0      832 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py
--rw-rw-rw-   0        0        0     9665 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/classic.py
--rw-rw-rw-   0        0        0     4390 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
--rw-rw-rw-   0        0        0    10277 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.490327 pm4py-2.7.4/pm4py/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      822 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.490327 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.511322 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
--rw-rw-rw-   0        0        0    14930 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
--rw-rw-rw-   0        0        0     2902 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
--rw-rw-rw-   0        0        0     5200 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/algorithm.py
--rw-rw-rw-   0        0        0     1260 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/replacement.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.511322 pm4py-2.7.4/pm4py/algo/discovery/dfg/utils/
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0      783 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.527954 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      958 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     4609 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/case_attributes.py
--rw-rw-rw-   0        0        0     2852 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/clean.py
--rw-rw-rw-   0        0        0     2795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/clean_polars.py
--rw-rw-rw-   0        0        0     2200 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/freq_triples.py
--rw-rw-rw-   0        0        0     2597 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/native.py
--rw-rw-rw-   0        0        0     5836 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.527954 pm4py-2.7.4/pm4py/algo/discovery/footprints/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/__init__.py
--rw-rw-rw-   0        0        0     3227 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.527954 pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.543581 pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/variants/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     2265 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.543581 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.559205 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/
--rw-rw-rw-   0        0        0      843 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/__init__.py
--rw-rw-rw-   0        0        0     4610 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
--rw-rw-rw-   0        0        0     3357 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
--rw-rw-rw-   0        0        0     3282 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.559205 pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.559205 pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/variants/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.559205 pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.574824 pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/variants/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py
--rw-rw-rw-   0        0        0    13417 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.574824 pm4py-2.7.4/pm4py/algo/discovery/heuristics/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/heuristics/__init__.py
--rw-rw-rw-   0        0        0     7559 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/heuristics/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.590444 pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/__init__.py
--rw-rw-rw-   0        0        0    26234 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/classic.py
--rw-rw-rw-   0        0        0    24321 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/plusplus.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.590444 pm4py-2.7.4/pm4py/algo/discovery/ilp/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ilp/__init__.py
--rw-rw-rw-   0        0        0     1782 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ilp/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.590444 pm4py-2.7.4/pm4py/algo/discovery/ilp/variants/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ilp/variants/__init__.py
--rw-rw-rw-   0        0        0    12788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ilp/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.606066 pm4py-2.7.4/pm4py/algo/discovery/inductive/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/__init__.py
--rw-rw-rw-   0        0        0     3790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.606066 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/
--rw-rw-rw-   0        0        0      829 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/__init__.py
--rw-rw-rw-   0        0        0     1533 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/abc.py
--rw-rw-rw-   0        0        0     1768 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/empty_log.py
--rw-rw-rw-   0        0        0     2268 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/factory.py
--rw-rw-rw-   0        0        0     2060 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/single_activity.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.643830 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/__init__.py
--rw-rw-rw-   0        0        0     2100 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/abc.py
--rw-rw-rw-   0        0        0     4570 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/concurrency.py
--rw-rw-rw-   0        0        0     2463 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/factory.py
--rw-rw-rw-   0        0        0    10916 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/loop.py
--rw-rw-rw-   0        0        0    11571 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/sequence.py
--rw-rw-rw-   0        0        0     1104 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/utils.py
--rw-rw-rw-   0        0        0     4316 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/xor.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.643830 pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/__init__.py
--rw-rw-rw-   0        0        0     1050 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
--rw-rw-rw-   0        0        0     2568 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.675074 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/
--rw-rw-rw-   0        0        0      897 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/__init__.py
--rw-rw-rw-   0        0        0     1385 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/abc.py
--rw-rw-rw-   0        0        0     4792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
--rw-rw-rw-   0        0        0     1643 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
--rw-rw-rw-   0        0        0     2709 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
--rw-rw-rw-   0        0        0     2672 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/factory.py
--rw-rw-rw-   0        0        0     3059 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/flower.py
--rw-rw-rw-   0        0        0     2441 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
--rw-rw-rw-   0        0        0     1520 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.690695 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/abc.py
--rw-rw-rw-   0        0        0     1740 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/im.py
--rw-rw-rw-   0        0        0     1098 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/imd.py
--rw-rw-rw-   0        0        0     4381 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/imf.py
--rw-rw-rw-   0        0        0      881 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/instances.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.706316 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/
--rw-rw-rw-   0        0        0      815 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/__init__.py
--rw-rw-rw-   0        0        0     2520 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/algorithm.py
--rw-rw-rw-   0        0        0     3194 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/trace_skel.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.714055 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/variants/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py
--rw-rw-rw-   0        0        0    11119 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.714055 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py
--rw-rw-rw-   0        0        0     3132 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.728061 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/
--rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     2878 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py
--rw-rw-rw-   0        0        0     2883 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.728061 pm4py-2.7.4/pm4py/algo/discovery/ocel/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.728061 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/
--rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/__init__.py
--rw-rw-rw-   0        0        0     2007 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.728061 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/utils/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
--rw-rw-rw-   0        0        0     4441 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.743694 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0     6622 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.743694 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py
--rw-rw-rw-   0        0        0     1841 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.759317 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/variants/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     6497 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.759317 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py
--rw-rw-rw-   0        0        0     1775 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.759317 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0     5629 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.774935 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/__init__.py
--rw-rw-rw-   0        0        0     1780 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.774935 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0     4718 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.774935 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py
--rw-rw-rw-   0        0        0     1800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.790556 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
--rw-rw-rw-   0        0        0     7010 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.790556 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/__init__.py
--rw-rw-rw-   0        0        0     3570 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.806177 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      855 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     4307 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
--rw-rw-rw-   0        0        0     5045 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
--rw-rw-rw-   0        0        0     3402 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/log.py
--rw-rw-rw-   0        0        0     4386 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.806177 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.822273 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/
--rw-rw-rw-   0        0        0      925 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py
--rw-rw-rw-   0        0        0     4044 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
--rw-rw-rw-   0        0        0     5278 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/log.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.828295 pm4py-2.7.4/pm4py/algo/discovery/transition_system/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/transition_system/__init__.py
--rw-rw-rw-   0        0        0     1991 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/transition_system/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.828295 pm4py-2.7.4/pm4py/algo/discovery/transition_system/variants/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     5900 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/discovery/transition_system/variants/view_based.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.828295 pm4py-2.7.4/pm4py/algo/evaluation/
--rw-rw-rw-   0        0        0      836 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/__init__.py
--rw-rw-rw-   0        0        0     4839 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.828295 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/
--rw-rw-rw-   0        0        0      919 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py
--rw-rw-rw-   0        0        0     1692 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.843924 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/variants/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.843924 pm4py-2.7.4/pm4py/algo/evaluation/generalization/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/generalization/__init__.py
--rw-rw-rw-   0        0        0     1710 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/generalization/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.859545 pm4py-2.7.4/pm4py/algo/evaluation/generalization/variants/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/generalization/variants/__init__.py
--rw-rw-rw-   0        0        0     4674 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/generalization/variants/token_based.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.859545 pm4py-2.7.4/pm4py/algo/evaluation/precision/
--rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/__init__.py
--rw-rw-rw-   0        0        0     3071 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.875169 pm4py-2.7.4/pm4py/algo/evaluation/precision/dfg/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/dfg/__init__.py
--rw-rw-rw-   0        0        0     3992 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/dfg/algorithm.py
--rw-rw-rw-   0        0        0     5463 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.890788 pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/
--rw-rw-rw-   0        0        0      829 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/__init__.py
--rw-rw-rw-   0        0        0    13827 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py
--rw-rw-rw-   0        0        0     6196 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.890788 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/__init__.py
--rw-rw-rw-   0        0        0     4559 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.906411 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/
--rw-rw-rw-   0        0        0      823 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
--rw-rw-rw-   0        0        0     6835 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
--rw-rw-rw-   0        0        0     5190 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.906411 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/__init__.py
--rw-rw-rw-   0        0        0     1686 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.928537 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/
--rw-rw-rw-   0        0        0      841 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/__init__.py
--rw-rw-rw-   0        0        0     2790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
--rw-rw-rw-   0        0        0     1602 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
--rw-rw-rw-   0        0        0     2120 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.928537 pm4py-2.7.4/pm4py/algo/filtering/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.928537 pm4py-2.7.4/pm4py/algo/filtering/common/
--rw-rw-rw-   0        0        0      852 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.944169 pm4py-2.7.4/pm4py/algo/filtering/common/attributes/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/attributes/__init__.py
--rw-rw-rw-   0        0        0      951 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/attributes/attributes_common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.944169 pm4py-2.7.4/pm4py/algo/filtering/common/end_activities/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/end_activities/__init__.py
--rw-rw-rw-   0        0        0      851 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py
--rw-rw-rw-   0        0        0      845 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/filtering_constants.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.959791 pm4py-2.7.4/pm4py/algo/filtering/common/start_activities/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/start_activities/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.959791 pm4py-2.7.4/pm4py/algo/filtering/common/timestamp/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/timestamp/__init__.py
--rw-rw-rw-   0        0        0     1208 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.959791 pm4py-2.7.4/pm4py/algo/filtering/dfg/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/dfg/__init__.py
--rw-rw-rw-   0        0        0    25920 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/dfg/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.959791 pm4py-2.7.4/pm4py/algo/filtering/log/
--rw-rw-rw-   0        0        0      866 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.975412 pm4py-2.7.4/pm4py/algo/filtering/log/attr_value_repetition/
--rw-rw-rw-   0        0        0      918 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2754 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.975412 pm4py-2.7.4/pm4py/algo/filtering/log/attributes/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/attributes/__init__.py
--rw-rw-rw-   0        0        0    18535 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.975412 pm4py-2.7.4/pm4py/algo/filtering/log/between/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/between/__init__.py
--rw-rw-rw-   0        0        0     2944 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.991033 pm4py-2.7.4/pm4py/algo/filtering/log/cases/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/cases/__init__.py
--rw-rw-rw-   0        0        0     4661 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.991033 pm4py-2.7.4/pm4py/algo/filtering/log/end_activities/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/end_activities/__init__.py
--rw-rw-rw-   0        0        0     4067 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.991033 pm4py-2.7.4/pm4py/algo/filtering/log/ltl/
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/ltl/__init__.py
--rw-rw-rw-   0        0        0    11165 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:54.991033 pm4py-2.7.4/pm4py/algo/filtering/log/paths/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/paths/__init__.py
--rw-rw-rw-   0        0        0     9848 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/paths/paths_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.006654 pm4py-2.7.4/pm4py/algo/filtering/log/prefixes/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.006654 pm4py-2.7.4/pm4py/algo/filtering/log/rework/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/rework/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.006654 pm4py-2.7.4/pm4py/algo/filtering/log/start_activities/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/start_activities/__init__.py
--rw-rw-rw-   0        0        0     4358 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.022276 pm4py-2.7.4/pm4py/algo/filtering/log/suffixes/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3223 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.028784 pm4py-2.7.4/pm4py/algo/filtering/log/timestamp/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/timestamp/__init__.py
--rw-rw-rw-   0        0        0    11514 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.028784 pm4py-2.7.4/pm4py/algo/filtering/log/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/variants/__init__.py
--rw-rw-rw-   0        0        0     9229 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/log/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.044411 pm4py-2.7.4/pm4py/algo/filtering/ocel/
--rw-rw-rw-   0        0        0      865 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/__init__.py
--rw-rw-rw-   0        0        0     3392 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/activity_type_matching.py
--rw-rw-rw-   0        0        0     3843 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/event_attributes.py
--rw-rw-rw-   0        0        0     2319 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/object_attributes.py
--rw-rw-rw-   0        0        0     3436 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     4262 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/ocel/ot_endpoints.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.044411 pm4py-2.7.4/pm4py/algo/filtering/pandas/
--rw-rw-rw-   0        0        0      891 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.044411 pm4py-2.7.4/pm4py/algo/filtering/pandas/attr_value_repetition/
--rw-rw-rw-   0        0        0      921 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
--rw-rw-rw-   0        0        0     2786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.044411 pm4py-2.7.4/pm4py/algo/filtering/pandas/attributes/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/attributes/__init__.py
--rw-rw-rw-   0        0        0    13483 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.060033 pm4py-2.7.4/pm4py/algo/filtering/pandas/between/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/between/__init__.py
--rw-rw-rw-   0        0        0     3266 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/between/between_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.060033 pm4py-2.7.4/pm4py/algo/filtering/pandas/cases/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/cases/__init__.py
--rw-rw-rw-   0        0        0     6315 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/cases/case_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.060033 pm4py-2.7.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
--rw-rw-rw-   0        0        0      842 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3079 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.060033 pm4py-2.7.4/pm4py/algo/filtering/pandas/end_activities/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/end_activities/__init__.py
--rw-rw-rw-   0        0        0     6348 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.075653 pm4py-2.7.4/pm4py/algo/filtering/pandas/ends_with/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/ends_with/__init__.py
--rw-rw-rw-   0        0        0     3745 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.075653 pm4py-2.7.4/pm4py/algo/filtering/pandas/ltl/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/ltl/__init__.py
--rw-rw-rw-   0        0        0    11785 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.075653 pm4py-2.7.4/pm4py/algo/filtering/pandas/paths/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/paths/__init__.py
--rw-rw-rw-   0        0        0     6897 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/paths/paths_filter.py
--rw-rw-rw-   0        0        0      832 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.075653 pm4py-2.7.4/pm4py/algo/filtering/pandas/prefixes/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/prefixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.091275 pm4py-2.7.4/pm4py/algo/filtering/pandas/rework/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/rework/__init__.py
--rw-rw-rw-   0        0        0     3383 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/rework/rework_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.091275 pm4py-2.7.4/pm4py/algo/filtering/pandas/start_activities/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/start_activities/__init__.py
--rw-rw-rw-   0        0        0     5738 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.091275 pm4py-2.7.4/pm4py/algo/filtering/pandas/starts_with/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/starts_with/__init__.py
--rw-rw-rw-   0        0        0     3747 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.091275 pm4py-2.7.4/pm4py/algo/filtering/pandas/suffixes/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/suffixes/__init__.py
--rw-rw-rw-   0        0        0     3950 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.106896 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp/__init__.py
--rw-rw-rw-   0        0        0     8848 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.106896 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/
--rw-rw-rw-   0        0        0      830 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
--rw-rw-rw-   0        0        0     3504 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.106896 pm4py-2.7.4/pm4py/algo/filtering/pandas/traces/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/traces/__init__.py
--rw-rw-rw-   0        0        0     4030 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/traces/trace_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.122517 pm4py-2.7.4/pm4py/algo/filtering/pandas/variants/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     6219 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/filtering/pandas/variants/variants_filter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.122517 pm4py-2.7.4/pm4py/algo/merging/
--rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/merging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.129023 pm4py-2.7.4/pm4py/algo/merging/case_relations/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/merging/case_relations/__init__.py
--rw-rw-rw-   0        0        0     2326 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/merging/case_relations/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.129023 pm4py-2.7.4/pm4py/algo/merging/case_relations/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/merging/case_relations/variants/__init__.py
--rw-rw-rw-   0        0        0     3474 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/merging/case_relations/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.129023 pm4py-2.7.4/pm4py/algo/organizational_mining/
--rw-rw-rw-   0        0        0      855 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.129023 pm4py-2.7.4/pm4py/algo/organizational_mining/local_diagnostics/
--rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
--rw-rw-rw-   0        0        0    12486 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.144651 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/
--rw-rw-rw-   0        0        0      817 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/__init__.py
--rw-rw-rw-   0        0        0     1840 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.144651 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0    10571 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.144651 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py
--rw-rw-rw-   0        0        0    12016 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.160272 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
--rw-rw-rw-   0        0        0    23662 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
--rw-rw-rw-   0        0        0    24339 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.160272 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/
--rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/__init__.py
--rw-rw-rw-   0        0        0     2502 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.160272 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/common/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/common/__init__.py
--rw-rw-rw-   0        0        0     8411 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/common/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.175893 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/__init__.py
--rw-rw-rw-   0        0        0     2448 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/log.py
--rw-rw-rw-   0        0        0     2209 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.175893 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/
--rw-rw-rw-   0        0        0      810 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/__init__.py
--rw-rw-rw-   0        0        0     3689 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/algorithm.py
--rw-rw-rw-   0        0        0     3199 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.175893 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.191514 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/
--rw-rw-rw-   0        0        0      857 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
--rw-rw-rw-   0        0        0     3735 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py
--rw-rw-rw-   0        0        0     3286 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
--rw-rw-rw-   0        0        0     3525 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
--rw-rw-rw-   0        0        0     3155 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.191514 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/
--rw-rw-rw-   0        0        0      860 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     4235 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
--rw-rw-rw-   0        0        0     2986 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
--rw-rw-rw-   0        0        0     3804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
--rw-rw-rw-   0        0        0     3432 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
--rw-rw-rw-   0        0        0     7599 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/organizational_mining/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.207137 pm4py-2.7.4/pm4py/algo/querying/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/querying/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.229267 pm4py-2.7.4/pm4py/algo/querying/openai/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/querying/openai/__init__.py
--rw-rw-rw-   0        0        0     3080 2023-04-03 09:02:28.000000 pm4py-2.7.4/pm4py/algo/querying/openai/log_to_cols_descr.py
--rw-rw-rw-   0        0        0     4160 2023-04-03 05:34:08.000000 pm4py-2.7.4/pm4py/algo/querying/openai/log_to_dfg_descr.py
--rw-rw-rw-   0        0        0     4428 2023-04-03 05:34:08.000000 pm4py-2.7.4/pm4py/algo/querying/openai/log_to_variants_descr.py
--rw-rw-rw-   0        0        0     1931 2023-05-08 08:05:19.000000 pm4py-2.7.4/pm4py/algo/querying/openai/net_to_descr.py
--rw-rw-rw-   0        0        0     5546 2023-05-08 08:10:26.000000 pm4py-2.7.4/pm4py/algo/querying/openai/ocel_fea_descr.py
--rw-rw-rw-   0        0        0     3680 2023-05-08 08:10:26.000000 pm4py-2.7.4/pm4py/algo/querying/openai/ocel_ocdfg_descr.py
--rw-rw-rw-   0        0        0     1543 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/querying/openai/perform_query.py
--rw-rw-rw-   0        0        0     3004 2023-04-03 12:43:47.000000 pm4py-2.7.4/pm4py/algo/querying/openai/stream_to_descr.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.229267 pm4py-2.7.4/pm4py/algo/reduction/
--rw-rw-rw-   0        0        0      879 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/reduction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.229267 pm4py-2.7.4/pm4py/algo/reduction/process_tree/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/reduction/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1601 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/reduction/process_tree/reducer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.229267 pm4py-2.7.4/pm4py/algo/reduction/process_tree/variants/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/reduction/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     3766 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.229267 pm4py-2.7.4/pm4py/algo/simulation/
--rw-rw-rw-   0        0        0      892 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.244894 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/
--rw-rw-rw-   0        0        0      919 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/__init__.py
--rw-rw-rw-   0        0        0     4575 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.244894 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/utils/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/utils/__init__.py
--rw-rw-rw-   0        0        0     5327 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/utils/replay.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.244894 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/variants/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/variants/__init__.py
--rw-rw-rw-   0        0        0    19795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.244894 pm4py-2.7.4/pm4py/algo/simulation/playout/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.260521 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/__init__.py
--rw-rw-rw-   0        0        0     1953 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.260521 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/
--rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0    14546 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/classic.py
--rw-rw-rw-   0        0        0     6018 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/performance.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.260521 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/__init__.py
--rw-rw-rw-   0        0        0     2579 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.276137 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/
--rw-rw-rw-   0        0        0      821 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     9045 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
--rw-rw-rw-   0        0        0     5225 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
--rw-rw-rw-   0        0        0     7927 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.276137 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/
--rw-rw-rw-   0        0        0      810 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1889 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.291758 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/
--rw-rw-rw-   0        0        0      835 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     1722 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
--rw-rw-rw-   0        0        0    13591 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
--rw-rw-rw-   0        0        0     4891 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.291758 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/__init__.py
--rw-rw-rw-   0        0        0     1779 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.291758 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/__init__.py
--rw-rw-rw-   0        0        0     5364 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/basic.py
--rw-rw-rw-   0        0        0    12993 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.291758 pm4py-2.7.4/pm4py/algo/transformation/
--rw-rw-rw-   0        0        0      824 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.307379 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.307379 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/util/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/util/__init__.py
--rw-rw-rw-   0        0        0     3901 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.307379 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/
--rw-rw-rw-   0        0        0      823 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/__init__.py
--rw-rw-rw-   0        0        0     6689 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/event_based.py
--rw-rw-rw-   0        0        0     6610 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/temporal.py
--rw-rw-rw-   0        0        0    50270 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.323001 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/
--rw-rw-rw-   0        0        0      923 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py
--rw-rw-rw-   0        0        0     2171 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.329508 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/variants/
--rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     3439 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.329508 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/__init__.py
--rw-rw-rw-   0        0        0     2161 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.329508 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/
--rw-rw-rw-   0        0        0      837 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/__init__.py
--rw-rw-rw-   0        0        0     2922 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py
--rw-rw-rw-   0        0        0     2526 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/next_time.py
--rw-rw-rw-   0        0        0     2385 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.345135 pm4py-2.7.4/pm4py/algo/transformation/log_to_trie/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_trie/__init__.py
--rw-rw-rw-   0        0        0     2262 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/log_to_trie/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.345135 pm4py-2.7.4/pm4py/algo/transformation/ocel/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.345135 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/__init__.py
--rw-rw-rw-   0        0        0     1684 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.345135 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/variants/
--rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/variants/__init__.py
--rw-rw-rw-   0        0        0     3318 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/description/variants/variant1.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.360756 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/
--rw-rw-rw-   0        0        0      821 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.392001 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/
--rw-rw-rw-   0        0        0     1002 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/__init__.py
--rw-rw-rw-   0        0        0     9033 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/algorithm.py
--rw-rw-rw-   0        0        0     1890 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_activity.py
--rw-rw-rw-   0        0        0     1991 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
--rw-rw-rw-   0        0        0     2467 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
--rw-rw-rw-   0        0        0     1608 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
--rw-rw-rw-   0        0        0     2212 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
--rw-rw-rw-   0        0        0     1970 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
--rw-rw-rw-   0        0        0     2956 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
--rw-rw-rw-   0        0        0     1948 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
--rw-rw-rw-   0        0        0     1905 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py
--rw-rw-rw-   0        0        0     2722 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.392001 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/
--rw-rw-rw-   0        0        0      831 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
--rw-rw-rw-   0        0        0     3843 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
--rw-rw-rw-   0        0        0     4874 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.429748 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/
--rw-rw-rw-   0        0        0     1268 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/__init__.py
--rw-rw-rw-   0        0        0    18595 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py
--rw-rw-rw-   0        0        0     3377 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
--rw-rw-rw-   0        0        0     1827 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     1827 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
--rw-rw-rw-   0        0        0     1901 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
--rw-rw-rw-   0        0        0     2015 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
--rw-rw-rw-   0        0        0     2067 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
--rw-rw-rw-   0        0        0     1857 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
--rw-rw-rw-   0        0        0     1868 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
--rw-rw-rw-   0        0        0     2004 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
--rw-rw-rw-   0        0        0     1631 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
--rw-rw-rw-   0        0        0     2094 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
--rw-rw-rw-   0        0        0     1750 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
--rw-rw-rw-   0        0        0     2499 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
--rw-rw-rw-   0        0        0     2975 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
--rw-rw-rw-   0        0        0     2394 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
--rw-rw-rw-   0        0        0     2342 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
--rw-rw-rw-   0        0        0     2978 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
--rw-rw-rw-   0        0        0     2713 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.445374 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/
--rw-rw-rw-   0        0        0      906 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/__init__.py
--rw-rw-rw-   0        0        0     2302 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
--rw-rw-rw-   0        0        0     2091 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
--rw-rw-rw-   0        0        0     2324 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
--rw-rw-rw-   0        0        0     2840 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
--rw-rw-rw-   0        0        0     1738 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
--rw-rw-rw-   0        0        0     3632 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.445374 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.460996 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     3423 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
--rw-rw-rw-   0        0        0     3339 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
--rw-rw-rw-   0        0        0    19612 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/analysis.py
--rw-rw-rw-   0        0        0    13401 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/cli.py
--rw-rw-rw-   0        0        0    44042 2023-04-26 05:57:30.000000 pm4py-2.7.4/pm4py/conformance.py
--rw-rw-rw-   0        0        0    19636 2023-03-27 13:48:22.000000 pm4py-2.7.4/pm4py/connectors.py
--rw-rw-rw-   0        0        0    19130 2023-04-25 06:11:22.000000 pm4py-2.7.4/pm4py/convert.py
--rw-rw-rw-   0        0        0    45434 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/discovery.py
--rw-rw-rw-   0        0        0    57976 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/filtering.py
--rw-rw-rw-   0        0        0     5014 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/hof.py
--rw-rw-rw-   0        0        0     1055 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/meta.py
--rw-rw-rw-   0        0        0    16489 2023-04-26 10:56:14.000000 pm4py-2.7.4/pm4py/ml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.460996 pm4py-2.7.4/pm4py/objects/
--rw-rw-rw-   0        0        0      935 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.460996 pm4py-2.7.4/pm4py/objects/bpmn/
--rw-rw-rw-   0        0        0      901 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.476621 pm4py-2.7.4/pm4py/objects/bpmn/exporter/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/exporter/__init__.py
--rw-rw-rw-   0        0        0     2130 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.476621 pm4py-2.7.4/pm4py/objects/bpmn/exporter/variants/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     7496 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/exporter/variants/etree.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.476621 pm4py-2.7.4/pm4py/objects/bpmn/importer/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/importer/__init__.py
--rw-rw-rw-   0        0        0     2085 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/importer/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.476621 pm4py-2.7.4/pm4py/objects/bpmn/importer/variants/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    16488 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/importer/variants/lxml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.492240 pm4py-2.7.4/pm4py/objects/bpmn/layout/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/layout/__init__.py
--rw-rw-rw-   0        0        0     1534 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/layout/layouter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.492240 pm4py-2.7.4/pm4py/objects/bpmn/layout/variants/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/layout/variants/__init__.py
--rw-rw-rw-   0        0        0    18042 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/layout/variants/graphviz.py
--rw-rw-rw-   0        0        0    20950 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/obj.py
--rw-rw-rw-   0        0        0     9205 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/semantics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.507860 pm4py-2.7.4/pm4py/objects/bpmn/util/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/util/__init__.py
--rw-rw-rw-   0        0        0     6246 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/util/bpmn_utils.py
--rw-rw-rw-   0        0        0     3352 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/util/reduction.py
--rw-rw-rw-   0        0        0     3729 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/bpmn/util/sorting.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.507860 pm4py-2.7.4/pm4py/objects/conversion/
--rw-rw-rw-   0        0        0      825 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.507860 pm4py-2.7.4/pm4py/objects/conversion/bpmn/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/bpmn/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/bpmn/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.507860 pm4py-2.7.4/pm4py/objects/conversion/bpmn/variants/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0    10026 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.523481 pm4py-2.7.4/pm4py/objects/conversion/dfg/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/dfg/__init__.py
--rw-rw-rw-   0        0        0     1340 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/dfg/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.529990 pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/
--rw-rw-rw-   0        0        0      860 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     3494 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
--rw-rw-rw-   0        0        0     4229 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.529990 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.529990 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/variants/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    11773 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.545621 pm4py-2.7.4/pm4py/objects/conversion/log/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/__init__.py
--rw-rw-rw-   0        0        0     1061 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/constants.py
--rw-rw-rw-   0        0        0     1319 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.561241 pm4py-2.7.4/pm4py/objects/conversion/log/variants/
--rw-rw-rw-   0        0        0      870 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/__init__.py
--rw-rw-rw-   0        0        0     1923 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
--rw-rw-rw-   0        0        0     2535 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
--rw-rw-rw-   0        0        0     3303 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_data_frame.py
--rw-rw-rw-   0        0        0     4382 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_event_log.py
--rw-rw-rw-   0        0        0    10279 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_event_stream.py
--rw-rw-rw-   0        0        0     5186 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_nx.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.561241 pm4py-2.7.4/pm4py/objects/conversion/ocel/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/ocel/__init__.py
--rw-rw-rw-   0        0        0     1814 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/ocel/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.561241 pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/__init__.py
--rw-rw-rw-   0        0        0     4056 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
--rw-rw-rw-   0        0        0     2754 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.561241 pm4py-2.7.4/pm4py/objects/conversion/process_tree/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.576861 pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/
--rw-rw-rw-   0        0        0      850 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0    10273 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    21550 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
--rw-rw-rw-   0        0        0     4772 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.576861 pm4py-2.7.4/pm4py/objects/conversion/wf_net/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/wf_net/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/wf_net/converter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.592483 pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/__init__.py
--rw-rw-rw-   0        0        0     3774 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
--rw-rw-rw-   0        0        0    10818 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.592483 pm4py-2.7.4/pm4py/objects/dfg/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.592483 pm4py-2.7.4/pm4py/objects/dfg/exporter/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/exporter/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.608105 pm4py-2.7.4/pm4py/objects/dfg/exporter/variants/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     4211 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/exporter/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.608105 pm4py-2.7.4/pm4py/objects/dfg/filtering/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/filtering/__init__.py
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/filtering/dfg_filtering.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.608105 pm4py-2.7.4/pm4py/objects/dfg/importer/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/importer/__init__.py
--rw-rw-rw-   0        0        0     2278 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/importer/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.623726 pm4py-2.7.4/pm4py/objects/dfg/importer/variants/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/importer/variants/classic.py
--rw-rw-rw-   0        0        0     1881 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.630234 pm4py-2.7.4/pm4py/objects/dfg/retrieval/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/retrieval/__init__.py
--rw-rw-rw-   0        0        0      913 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/retrieval/log.py
--rw-rw-rw-   0        0        0      873 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/retrieval/pandas.py
--rw-rw-rw-   0        0        0     5465 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/util.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.630234 pm4py-2.7.4/pm4py/objects/dfg/utils/
--rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/utils/__init__.py
--rw-rw-rw-   0        0        0    26492 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/dfg/utils/dfg_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.645864 pm4py-2.7.4/pm4py/objects/heuristics_net/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/heuristics_net/__init__.py
--rw-rw-rw-   0        0        0     1226 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/heuristics_net/defaults.py
--rw-rw-rw-   0        0        0     2689 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/heuristics_net/edge.py
--rw-rw-rw-   0        0        0     9877 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/heuristics_net/node.py
--rw-rw-rw-   0        0        0     5871 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/heuristics_net/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.645864 pm4py-2.7.4/pm4py/objects/log/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.645864 pm4py-2.7.4/pm4py/objects/log/exporter/
--rw-rw-rw-   0        0        0      778 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.645864 pm4py-2.7.4/pm4py/objects/log/exporter/xes/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/__init__.py
--rw-rw-rw-   0        0        0     2578 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.661485 pm4py-2.7.4/pm4py/objects/log/exporter/xes/util/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/util/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/util/compression.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.661485 pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/
--rw-rw-rw-   0        0        0      815 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/__init__.py
--rw-rw-rw-   0        0        0    12291 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
--rw-rw-rw-   0        0        0    10417 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.661485 pm4py-2.7.4/pm4py/objects/log/importer/
--rw-rw-rw-   0        0        0      778 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.661485 pm4py-2.7.4/pm4py/objects/log/importer/xes/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     3888 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.677107 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/
--rw-rw-rw-   0        0        0      850 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9593 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py
--rw-rw-rw-   0        0        0    17461 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse.py
--rw-rw-rw-   0        0        0    17730 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py
--rw-rw-rw-   0        0        0    18029 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
--rw-rw-rw-   0        0        0    11435 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/line_by_line.py
--rw-rw-rw-   0        0        0    12284 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.708350 pm4py-2.7.4/pm4py/objects/log/util/
--rw-rw-rw-   0        0        0     1102 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/__init__.py
--rw-rw-rw-   0        0        0     3114 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/artificial.py
--rw-rw-rw-   0        0        0     3974 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/basic_filter.py
--rw-rw-rw-   0        0        0    18098 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/dataframe_utils.py
--rw-rw-rw-   0        0        0     2283 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/filtering_utils.py
--rw-rw-rw-   0        0        0     4898 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/get_class_representation.py
--rw-rw-rw-   0        0        0     3195 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/get_log_encoded.py
--rw-rw-rw-   0        0        0     8099 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/get_prefixes.py
--rw-rw-rw-   0        0        0     1752 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/index_attribute.py
--rw-rw-rw-   0        0        0     4067 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/insert_classifier.py
--rw-rw-rw-   0        0        0    12644 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/interval_lifecycle.py
--rw-rw-rw-   0        0        0     5167 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/log.py
--rw-rw-rw-   0        0        0     4484 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/log_regex.py
--rw-rw-rw-   0        0        0     2867 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/move_attrs_to_trace.py
--rw-rw-rw-   0        0        0     4527 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/pandas_log_wrapper.py
--rw-rw-rw-   0        0        0     3066 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/pandas_numpy_variants.py
--rw-rw-rw-   0        0        0     2488 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/sampling.py
--rw-rw-rw-   0        0        0     6049 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/sorting.py
--rw-rw-rw-   0        0        0     2078 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/split_train_test.py
--rw-rw-rw-   0        0        0     1695 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/log/util/xes.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.730480 pm4py-2.7.4/pm4py/objects/ocel/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.730480 pm4py-2.7.4/pm4py/objects/ocel/exporter/
--rw-rw-rw-   0        0        0      899 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.730480 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/__init__.py
--rw-rw-rw-   0        0        0     1695 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.730480 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     1637 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.746107 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1550 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.746107 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.746107 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1673 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.761728 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     4838 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     1679 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.761728 pm4py-2.7.4/pm4py/objects/ocel/exporter/util/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/util/__init__.py
--rw-rw-rw-   0        0        0     1671 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.761728 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.777352 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     7889 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0    10788 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.777352 pm4py-2.7.4/pm4py/objects/ocel/importer/
--rw-rw-rw-   0        0        0      893 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.777352 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1731 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.777352 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/variants/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     1889 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/csv/variants/pandas.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.792983 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/__init__.py
--rw-rw-rw-   0        0        0     1585 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.792983 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/variants/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
--rw-rw-rw-   0        0        0     4973 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.792983 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.792983 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
--rw-rw-rw-   0        0        0     6746 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
--rw-rw-rw-   0        0        0     1883 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.808593 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/__init__.py
--rw-rw-rw-   0        0        0     1611 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.808593 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
--rw-rw-rw-   0        0        0     8499 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
--rw-rw-rw-   0        0        0     9252 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
--rw-rw-rw-   0        0        0     6408 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.861971 pm4py-2.7.4/pm4py/objects/ocel/util/
--rw-rw-rw-   0        0        0     1067 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/attributes_names.py
--rw-rw-rw-   0        0        0     2424 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
--rw-rw-rw-   0        0        0     2690 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/e2o_qualification.py
--rw-rw-rw-   0        0        0     3668 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py
--rw-rw-rw-   0        0        0     4377 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
--rw-rw-rw-   0        0        0     2178 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/events_per_object_type.py
--rw-rw-rw-   0        0        0     3214 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/events_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1654 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/explode.py
--rw-rw-rw-   0        0        0     4499 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/extended_table.py
--rw-rw-rw-   0        0        0     6047 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/filtering_utils.py
--rw-rw-rw-   0        0        0     3117 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/flattening.py
--rw-rw-rw-   0        0        0    16914 2023-04-25 06:11:22.000000 pm4py-2.7.4/pm4py/objects/ocel/util/log_ocel.py
--rw-rw-rw-   0        0        0      942 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/names_stripping.py
--rw-rw-rw-   0        0        0     3214 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py
--rw-rw-rw-   0        0        0     1894 2023-04-25 06:12:03.000000 pm4py-2.7.4/pm4py/objects/ocel/util/ocel_consistency.py
--rw-rw-rw-   0        0        0     1976 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/ocel_iterator.py
--rw-rw-rw-   0        0        0     2479 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/parent_children_ref.py
--rw-rw-rw-   0        0        0     1297 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/related_events.py
--rw-rw-rw-   0        0        0     1744 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/related_objects.py
--rw-rw-rw-   0        0        0     2610 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
--rw-rw-rw-   0        0        0     3725 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/util/sampling.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.861971 pm4py-2.7.4/pm4py/objects/ocel/validation/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/validation/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/validation/jsonocel.py
--rw-rw-rw-   0        0        0     1200 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/ocel/validation/xmlocel.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.861971 pm4py-2.7.4/pm4py/objects/org/
--rw-rw-rw-   0        0        0      776 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/org/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.877592 pm4py-2.7.4/pm4py/objects/org/roles/
--rw-rw-rw-   0        0        0      775 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/org/roles/__init__.py
--rw-rw-rw-   0        0        0     1339 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/org/roles/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.877592 pm4py-2.7.4/pm4py/objects/org/sna/
--rw-rw-rw-   0        0        0      773 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/org/sna/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/org/sna/obj.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.893213 pm4py-2.7.4/pm4py/objects/petri_net/
--rw-rw-rw-   0        0        0      828 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.893213 pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/__init__.py
--rw-rw-rw-   0        0        0     1287 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py
--rw-rw-rw-   0        0        0     6212 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/semantics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.893213 pm4py-2.7.4/pm4py/objects/petri_net/exporter/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/exporter/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.908833 pm4py-2.7.4/pm4py/objects/petri_net/exporter/variants/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0    12697 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/exporter/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.908833 pm4py-2.7.4/pm4py/objects/petri_net/importer/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/importer/__init__.py
--rw-rw-rw-   0        0        0     1910 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/importer/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.908833 pm4py-2.7.4/pm4py/objects/petri_net/importer/variants/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/importer/variants/__init__.py
--rw-rw-rw-   0        0        0    14894 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/importer/variants/pnml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.908833 pm4py-2.7.4/pm4py/objects/petri_net/inhibitor_reset/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py
--rw-rw-rw-   0        0        0     4665 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py
--rw-rw-rw-   0        0        0    13270 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/obj.py
--rw-rw-rw-   0        0        0     1225 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/properties.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.930961 pm4py-2.7.4/pm4py/objects/petri_net/saw_net/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/saw_net/__init__.py
--rw-rw-rw-   0        0        0     4805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/saw_net/convert.py
--rw-rw-rw-   0        0        0     1546 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/saw_net/obj.py
--rw-rw-rw-   0        0        0    10807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/saw_net/semantics.py
--rw-rw-rw-   0        0        0     1503 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/sem_interface.py
--rw-rw-rw-   0        0        0     5339 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/semantics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.930961 pm4py-2.7.4/pm4py/objects/petri_net/stochastic/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/stochastic/__init__.py
--rw-rw-rw-   0        0        0     1448 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/stochastic/obj.py
--rw-rw-rw-   0        0        0     2619 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/stochastic/semantics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.962210 pm4py-2.7.4/pm4py/objects/petri_net/utils/
--rw-rw-rw-   0        0        0     1035 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/__init__.py
--rw-rw-rw-   0        0        0    18755 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/align_utils.py
--rw-rw-rw-   0        0        0     5923 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/check_soundness.py
--rw-rw-rw-   0        0        0     4014 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/consumption_matrix.py
--rw-rw-rw-   0        0        0     6609 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/decomposition.py
--rw-rw-rw-   0        0        0     1672 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py
--rw-rw-rw-   0        0        0     5751 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/explore_path.py
--rw-rw-rw-   0        0        0     1195 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/final_marking.py
--rw-rw-rw-   0        0        0     2272 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/incidence_matrix.py
--rw-rw-rw-   0        0        0     1227 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/initial_marking.py
--rw-rw-rw-   0        0        0     4243 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/murata.py
--rw-rw-rw-   0        0        0     4281 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/networkx_graph.py
--rw-rw-rw-   0        0        0     4124 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/obj_marking.py
--rw-rw-rw-   0        0        0    23057 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/performance_map.py
--rw-rw-rw-   0        0        0    20532 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/petri_utils.py
--rw-rw-rw-   0        0        0     4602 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/projection.py
--rw-rw-rw-   0        0        0     5570 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/reachability_graph.py
--rw-rw-rw-   0        0        0    14266 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/reduction.py
--rw-rw-rw-   0        0        0     7288 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/petri_net/utils/synchronous_product.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.977831 pm4py-2.7.4/pm4py/objects/process_tree/
--rw-rw-rw-   0        0        0      917 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.977831 pm4py-2.7.4/pm4py/objects/process_tree/exporter/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/exporter/__init__.py
--rw-rw-rw-   0        0        0     1888 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/exporter/exporter.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.977831 pm4py-2.7.4/pm4py/objects/process_tree/exporter/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/exporter/variants/__init__.py
--rw-rw-rw-   0        0        0     5527 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/exporter/variants/ptml.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.993465 pm4py-2.7.4/pm4py/objects/process_tree/importer/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/importer/__init__.py
--rw-rw-rw-   0        0        0     2048 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/importer/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.993465 pm4py-2.7.4/pm4py/objects/process_tree/importer/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/importer/variants/__init__.py
--rw-rw-rw-   0        0        0     5214 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/importer/variants/ptml.py
--rw-rw-rw-   0        0        0     7135 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/obj.py
--rw-rw-rw-   0        0        0     8883 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/semantics.py
--rw-rw-rw-   0        0        0      887 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/state.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:55.993465 pm4py-2.7.4/pm4py/objects/process_tree/utils/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/utils/__init__.py
--rw-rw-rw-   0        0        0     7128 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/utils/bottomup.py
--rw-rw-rw-   0        0        0    15797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/utils/generic.py
--rw-rw-rw-   0        0        0     3362 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/process_tree/utils/regex.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.009074 pm4py-2.7.4/pm4py/objects/random_variables/
--rw-rw-rw-   0        0        0      958 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/__init__.py
--rw-rw-rw-   0        0        0     3878 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/basic_structure.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.009074 pm4py-2.7.4/pm4py/objects/random_variables/constant0/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/constant0/__init__.py
--rw-rw-rw-   0        0        0     3586 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/constant0/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.009074 pm4py-2.7.4/pm4py/objects/random_variables/exponential/
--rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/exponential/__init__.py
--rw-rw-rw-   0        0        0     3684 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/exponential/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.009074 pm4py-2.7.4/pm4py/objects/random_variables/gamma/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/gamma/__init__.py
--rw-rw-rw-   0        0        0     3749 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/gamma/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.024695 pm4py-2.7.4/pm4py/objects/random_variables/lognormal/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/lognormal/__init__.py
--rw-rw-rw-   0        0        0     3568 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/lognormal/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.031202 pm4py-2.7.4/pm4py/objects/random_variables/normal/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/normal/__init__.py
--rw-rw-rw-   0        0        0     3594 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/normal/random_variable.py
--rw-rw-rw-   0        0        0     9224 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.031202 pm4py-2.7.4/pm4py/objects/random_variables/uniform/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/uniform/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/random_variables/uniform/random_variable.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.031202 pm4py-2.7.4/pm4py/objects/stochastic_petri/
--rw-rw-rw-   0        0        0      912 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/stochastic_petri/__init__.py
--rw-rw-rw-   0        0        0    12887 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/stochastic_petri/ctmc.py
--rw-rw-rw-   0        0        0     4714 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/stochastic_petri/tangible_reachability.py
--rw-rw-rw-   0        0        0     1616 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/stochastic_petri/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.046829 pm4py-2.7.4/pm4py/objects/transition_system/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/transition_system/__init__.py
--rw-rw-rw-   0        0        0      825 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/transition_system/constants.py
--rw-rw-rw-   0        0        0     3958 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/transition_system/obj.py
--rw-rw-rw-   0        0        0     3625 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/transition_system/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.046829 pm4py-2.7.4/pm4py/objects/trie/
--rw-rw-rw-   0        0        0      770 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/trie/__init__.py
--rw-rw-rw-   0        0        0     1911 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/objects/trie/obj.py
--rw-rw-rw-   0        0        0    21530 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/ocel.py
--rw-rw-rw-   0        0        0    11351 2023-05-08 08:10:22.000000 pm4py-2.7.4/pm4py/openai.py
--rw-rw-rw-   0        0        0    15446 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/org.py
--rw-rw-rw-   0        0        0     3805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/privacy.py
--rw-rw-rw-   0        0        0    12248 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/read.py
--rw-rw-rw-   0        0        0     3789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/sim.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.046829 pm4py-2.7.4/pm4py/statistics/
--rw-rw-rw-   0        0        0      899 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.046829 pm4py-2.7.4/pm4py/statistics/attributes/
--rw-rw-rw-   0        0        0      894 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.062451 pm4py-2.7.4/pm4py/statistics/attributes/common/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/common/__init__.py
--rw-rw-rw-   0        0        0     6609 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/common/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.062451 pm4py-2.7.4/pm4py/statistics/attributes/log/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/log/__init__.py
--rw-rw-rw-   0        0        0    13308 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/log/get.py
--rw-rw-rw-   0        0        0     6933 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/log/select.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.062451 pm4py-2.7.4/pm4py/statistics/attributes/pandas/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/pandas/__init__.py
--rw-rw-rw-   0        0        0     9789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/attributes/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.062451 pm4py-2.7.4/pm4py/statistics/concurrent_activities/
--rw-rw-rw-   0        0        0      906 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/concurrent_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.078071 pm4py-2.7.4/pm4py/statistics/concurrent_activities/log/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/concurrent_activities/log/__init__.py
--rw-rw-rw-   0        0        0     4092 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/concurrent_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.078071 pm4py-2.7.4/pm4py/statistics/concurrent_activities/pandas/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/concurrent_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     3697 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/concurrent_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.078071 pm4py-2.7.4/pm4py/statistics/end_activities/
--rw-rw-rw-   0        0        0      902 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.078071 pm4py-2.7.4/pm4py/statistics/end_activities/common/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.094361 pm4py-2.7.4/pm4py/statistics/end_activities/log/
--rw-rw-rw-   0        0        0      787 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2764 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.094361 pm4py-2.7.4/pm4py/statistics/end_activities/pandas/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2636 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/end_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.094361 pm4py-2.7.4/pm4py/statistics/eventually_follows/
--rw-rw-rw-   0        0        0      900 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/eventually_follows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.094361 pm4py-2.7.4/pm4py/statistics/eventually_follows/log/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/eventually_follows/log/__init__.py
--rw-rw-rw-   0        0        0     3026 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/eventually_follows/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.109982 pm4py-2.7.4/pm4py/statistics/eventually_follows/pandas/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/eventually_follows/pandas/__init__.py
--rw-rw-rw-   0        0        0     2890 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/eventually_follows/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.125614 pm4py-2.7.4/pm4py/statistics/ocel/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/__init__.py
--rw-rw-rw-   0        0        0     3744 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/act_ot_dependent.py
--rw-rw-rw-   0        0        0     5677 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/act_utils.py
--rw-rw-rw-   0        0        0     9399 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/edge_metrics.py
--rw-rw-rw-   0        0        0     2387 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/objects_ot_count.py
--rw-rw-rw-   0        0        0     2395 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/ocel/ot_activities.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.131140 pm4py-2.7.4/pm4py/statistics/overlap/
--rw-rw-rw-   0        0        0      881 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.131140 pm4py-2.7.4/pm4py/statistics/overlap/cases/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.131140 pm4py-2.7.4/pm4py/statistics/overlap/cases/log/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2713 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.131140 pm4py-2.7.4/pm4py/statistics/overlap/cases/pandas/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.131140 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.146767 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/log/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/log/__init__.py
--rw-rw-rw-   0        0        0     2767 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.146767 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/pandas/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py
--rw-rw-rw-   0        0        0     2570 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/interval_events/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.146767 pm4py-2.7.4/pm4py/statistics/overlap/utils/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/utils/__init__.py
--rw-rw-rw-   0        0        0     1986 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/overlap/utils/compute.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.146767 pm4py-2.7.4/pm4py/statistics/passed_time/
--rw-rw-rw-   0        0        0      888 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.162388 pm4py-2.7.4/pm4py/statistics/passed_time/log/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/__init__.py
--rw-rw-rw-   0        0        0     1806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.162388 pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/
--rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/__init__.py
--rw-rw-rw-   0        0        0     2412 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/post.py
--rw-rw-rw-   0        0        0     2394 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/pre.py
--rw-rw-rw-   0        0        0     3075 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.162388 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     1793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.178009 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/
--rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/__init__.py
--rw-rw-rw-   0        0        0     4156 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/post.py
--rw-rw-rw-   0        0        0     4260 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/pre.py
--rw-rw-rw-   0        0        0     5079 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/prepost.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.178009 pm4py-2.7.4/pm4py/statistics/rework/
--rw-rw-rw-   0        0        0      783 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.178009 pm4py-2.7.4/pm4py/statistics/rework/cases/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/cases/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.178009 pm4py-2.7.4/pm4py/statistics/rework/cases/log/
--rw-rw-rw-   0        0        0      785 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/cases/log/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/cases/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.193632 pm4py-2.7.4/pm4py/statistics/rework/cases/pandas/
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/cases/pandas/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/cases/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.193632 pm4py-2.7.4/pm4py/statistics/rework/log/
--rw-rw-rw-   0        0        0      779 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/log/__init__.py
--rw-rw-rw-   0        0        0     2265 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.193632 pm4py-2.7.4/pm4py/statistics/rework/pandas/
--rw-rw-rw-   0        0        0      782 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/pandas/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/rework/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.193632 pm4py-2.7.4/pm4py/statistics/sojourn_time/
--rw-rw-rw-   0        0        0      888 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/sojourn_time/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.209253 pm4py-2.7.4/pm4py/statistics/sojourn_time/log/
--rw-rw-rw-   0        0        0      785 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/sojourn_time/log/__init__.py
--rw-rw-rw-   0        0        0     5495 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/sojourn_time/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.209253 pm4py-2.7.4/pm4py/statistics/sojourn_time/pandas/
--rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/sojourn_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     4929 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/sojourn_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.209253 pm4py-2.7.4/pm4py/statistics/start_activities/
--rw-rw-rw-   0        0        0      904 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.209253 pm4py-2.7.4/pm4py/statistics/start_activities/common/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/common/__init__.py
--rw-rw-rw-   0        0        0     1813 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/common/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.224874 pm4py-2.7.4/pm4py/statistics/start_activities/log/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/log/__init__.py
--rw-rw-rw-   0        0        0     2787 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.224874 pm4py-2.7.4/pm4py/statistics/start_activities/pandas/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/pandas/__init__.py
--rw-rw-rw-   0        0        0     2594 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/start_activities/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/
--rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/log/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/log/__init__.py
--rw-rw-rw-   0        0        0     3191 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/pandas/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py
--rw-rw-rw-   0        0        0     3255 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/pandas/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/util/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/util/__init__.py
--rw-rw-rw-   0        0        0     2385 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/cycle_time/util/compute.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.231382 pm4py-2.7.4/pm4py/statistics/traces/generic/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.247010 pm4py-2.7.4/pm4py/statistics/traces/generic/common/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/common/__init__.py
--rw-rw-rw-   0        0        0     2950 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/common/case_duration.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.247010 pm4py-2.7.4/pm4py/statistics/traces/generic/log/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/log/__init__.py
--rw-rw-rw-   0        0        0     5339 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/log/case_arrival.py
--rw-rw-rw-   0        0        0    13275 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/log/case_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.247010 pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/__init__.py
--rw-rw-rw-   0        0        0     4213 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/case_arrival.py
--rw-rw-rw-   0        0        0    16506 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/case_statistics.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.262631 pm4py-2.7.4/pm4py/statistics/util/
--rw-rw-rw-   0        0        0      898 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/util/__init__.py
--rw-rw-rw-   0        0        0     2370 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/util/times_bipartite_matching.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.262631 pm4py-2.7.4/pm4py/statistics/variants/
--rw-rw-rw-   0        0        0      880 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.262631 pm4py-2.7.4/pm4py/statistics/variants/log/
--rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/variants/log/__init__.py
--rw-rw-rw-   0        0        0     7359 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/variants/log/get.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.262631 pm4py-2.7.4/pm4py/statistics/variants/pandas/
--rw-rw-rw-   0        0        0      784 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/variants/pandas/__init__.py
--rw-rw-rw-   0        0        0     2197 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/statistics/variants/pandas/get.py
--rw-rw-rw-   0        0        0    30520 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/stats.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.262631 pm4py-2.7.4/pm4py/streaming/
--rw-rw-rw-   0        0        0      804 2023-04-05 11:57:19.000000 pm4py-2.7.4/pm4py/streaming/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/conformance/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/
--rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/__init__.py
--rw-rw-rw-   0        0        0     1515 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/variants/
--rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0    10995 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.278260 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
--rw-rw-rw-   0        0        0    17212 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.293875 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/__init__.py
--rw-rw-rw-   0        0        0     2135 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.293875 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/variants/
--rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
--rw-rw-rw-   0        0        0     9602 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.293875 pm4py-2.7.4/pm4py/streaming/algo/discovery/
--rw-rw-rw-   0        0        0      782 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.309493 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/algorithm.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.309493 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/variants/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     7399 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     1503 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/algo/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.309493 pm4py-2.7.4/pm4py/streaming/conversion/
--rw-rw-rw-   0        0        0     1468 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/conversion/__init__.py
--rw-rw-rw-   0        0        0     4925 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/conversion/from_pandas.py
--rw-rw-rw-   0        0        0     5211 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/conversion/ocel_flatts_distributor.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.309493 pm4py-2.7.4/pm4py/streaming/importer/
--rw-rw-rw-   0        0        0      875 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.331498 pm4py-2.7.4/pm4py/streaming/importer/csv/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/csv/__init__.py
--rw-rw-rw-   0        0        0     1488 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/csv/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.331498 pm4py-2.7.4/pm4py/streaming/importer/csv/variants/
--rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/csv/variants/__init__.py
--rw-rw-rw-   0        0        0     3406 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.331498 pm4py-2.7.4/pm4py/streaming/importer/xes/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/xes/__init__.py
--rw-rw-rw-   0        0        0     1523 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/xes/importer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.331498 pm4py-2.7.4/pm4py/streaming/importer/xes/variants/
--rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/xes/variants/__init__.py
--rw-rw-rw-   0        0        0     9461 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py
--rw-rw-rw-   0        0        0     9317 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.347126 pm4py-2.7.4/pm4py/streaming/stream/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/stream/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/stream/live_event_stream.py
--rw-rw-rw-   0        0        0     3109 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/stream/live_trace_stream.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.347126 pm4py-2.7.4/pm4py/streaming/util/
--rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.347126 pm4py-2.7.4/pm4py/streaming/util/dictio/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/__init__.py
--rw-rw-rw-   0        0        0     1461 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/generator.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.362747 pm4py-2.7.4/pm4py/streaming/util/dictio/versions/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/versions/__init__.py
--rw-rw-rw-   0        0        0      941 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/versions/classic.py
--rw-rw-rw-   0        0        0     3540 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/versions/redis.py
--rw-rw-rw-   0        0        0     1949 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/dictio/versions/thread_safe.py
--rw-rw-rw-   0        0        0     1039 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/event_stream_printer.py
--rw-rw-rw-   0        0        0     1039 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/streaming/util/trace_stream_printer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.393997 pm4py-2.7.4/pm4py/util/
--rw-rw-rw-   0        0        0      918 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/__init__.py
--rw-rw-rw-   0        0        0     5000 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/business_hours.py
--rw-rw-rw-   0        0        0     2225 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/colors.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.393997 pm4py-2.7.4/pm4py/util/compression/
--rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/compression/__init__.py
--rw-rw-rw-   0        0        0     1314 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/compression/dtypes.py
--rw-rw-rw-   0        0        0    12024 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/compression/util.py
--rw-rw-rw-   0        0        0     4854 2023-05-08 08:05:18.000000 pm4py-2.7.4/pm4py/util/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.409615 pm4py-2.7.4/pm4py/util/dt_parsing/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/__init__.py
--rw-rw-rw-   0        0        0     2608 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/parser.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.409615 pm4py-2.7.4/pm4py/util/dt_parsing/variants/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/variants/__init__.py
--rw-rw-rw-   0        0        0     1029 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/variants/cs8601.py
--rw-rw-rw-   0        0        0     1470 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/variants/dummy.py
--rw-rw-rw-   0        0        0     1294 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/dt_parsing/variants/strpfromiso.py
--rw-rw-rw-   0        0        0     1564 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/exec_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.425234 pm4py-2.7.4/pm4py/util/lp/
--rw-rw-rw-   0        0        0      784 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/__init__.py
--rw-rw-rw-   0        0        0     5359 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/solver.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.425234 pm4py-2.7.4/pm4py/util/lp/util/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.447367 pm4py-2.7.4/pm4py/util/lp/variants/
--rw-rw-rw-   0        0        0      926 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver.py
--rw-rw-rw-   0        0        0     3420 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
--rw-rw-rw-   0        0        0     3059 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
--rw-rw-rw-   0        0        0     3937 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
--rw-rw-rw-   0        0        0     5153 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/ortools_solver.py
--rw-rw-rw-   0        0        0     6101 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/pulp_solver.py
--rw-rw-rw-   0        0        0     1876 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/lp/variants/scipy_solver.py
--rw-rw-rw-   0        0        0    11130 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/pandas_utils.py
--rw-rw-rw-   0        0        0     1494 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/points_subset.py
--rw-rw-rw-   0        0        0     1712 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/regex.py
--rw-rw-rw-   0        0        0     3663 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/string_distance.py
--rw-rw-rw-   0        0        0     1095 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/typing.py
--rw-rw-rw-   0        0        0     2261 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/variants_util.py
--rw-rw-rw-   0        0        0     5861 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/vis_utils.py
--rw-rw-rw-   0        0        0     1614 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/util/xes_constants.py
--rw-rw-rw-   0        0        0    23609 2023-03-27 13:12:17.000000 pm4py-2.7.4/pm4py/utils.py
--rw-rw-rw-   0        0        0    65769 2023-05-08 08:05:18.000000 pm4py-2.7.4/pm4py/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.447367 pm4py-2.7.4/pm4py/visualization/
--rw-rw-rw-   0        0        0     1837 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.447367 pm4py-2.7.4/pm4py/visualization/align_table/
--rw-rw-rw-   0        0        0      790 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/align_table/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.447367 pm4py-2.7.4/pm4py/visualization/align_table/variants/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/align_table/variants/__init__.py
--rw-rw-rw-   0        0        0     3868 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/visualization/align_table/variants/classic.py
--rw-rw-rw-   0        0        0     2973 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/align_table/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.447367 pm4py-2.7.4/pm4py/visualization/bpmn/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/bpmn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.462989 pm4py-2.7.4/pm4py/visualization/bpmn/variants/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/bpmn/variants/__init__.py
--rw-rw-rw-   0        0        0     3626 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/bpmn/variants/classic.py
--rw-rw-rw-   0        0        0     2613 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/bpmn/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.478611 pm4py-2.7.4/pm4py/visualization/common/
--rw-rw-rw-   0        0        0      817 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/common/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/common/dot_util.py
--rw-rw-rw-   0        0        0     3058 2023-05-08 08:05:18.000000 pm4py-2.7.4/pm4py/visualization/common/gview.py
--rw-rw-rw-   0        0        0     3394 2023-05-08 08:10:31.000000 pm4py-2.7.4/pm4py/visualization/common/html.py
--rw-rw-rw-   0        0        0     1531 2023-05-08 08:05:18.000000 pm4py-2.7.4/pm4py/visualization/common/save.py
--rw-rw-rw-   0        0        0     2526 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/common/svg_pos_parser.py
--rw-rw-rw-   0        0        0      879 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/common/utils.py
--rw-rw-rw-   0        0        0     1540 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/common/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.478611 pm4py-2.7.4/pm4py/visualization/decisiontree/
--rw-rw-rw-   0        0        0      932 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.478611 pm4py-2.7.4/pm4py/visualization/decisiontree/util/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/util/__init__.py
--rw-rw-rw-   0        0        0     2621 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/util/dt_to_string.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.478611 pm4py-2.7.4/pm4py/visualization/decisiontree/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/variants/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/variants/classic.py
--rw-rw-rw-   0        0        0     2854 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/decisiontree/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.497413 pm4py-2.7.4/pm4py/visualization/dfg/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.500521 pm4py-2.7.4/pm4py/visualization/dfg/util/
--rw-rw-rw-   0        0        0      787 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/util/__init__.py
--rw-rw-rw-   0        0        0     8672 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/util/dfg_gviz.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.500521 pm4py-2.7.4/pm4py/visualization/dfg/variants/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/variants/__init__.py
--rw-rw-rw-   0        0        0     5223 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/variants/cost.py
--rw-rw-rw-   0        0        0     4761 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/variants/frequency.py
--rw-rw-rw-   0        0        0     5374 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/variants/performance.py
--rw-rw-rw-   0        0        0     3272 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.500521 pm4py-2.7.4/pm4py/visualization/dotted_chart/
--rw-rw-rw-   0        0        0      905 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dotted_chart/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.500521 pm4py-2.7.4/pm4py/visualization/dotted_chart/variants/
--rw-rw-rw-   0        0        0      797 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/dotted_chart/variants/__init__.py
--rw-rw-rw-   0        0        0     9224 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/visualization/dotted_chart/variants/classic.py
--rw-rw-rw-   0        0        0     3776 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/visualization/dotted_chart/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.516142 pm4py-2.7.4/pm4py/visualization/footprints/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.516142 pm4py-2.7.4/pm4py/visualization/footprints/variants/
--rw-rw-rw-   0        0        0      828 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/variants/__init__.py
--rw-rw-rw-   0        0        0     3827 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/variants/comparison.py
--rw-rw-rw-   0        0        0     4359 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/variants/comparison_symmetric.py
--rw-rw-rw-   0        0        0     3265 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/variants/single.py
--rw-rw-rw-   0        0        0     3119 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/footprints/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.531653 pm4py-2.7.4/pm4py/visualization/graphs/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.531653 pm4py-2.7.4/pm4py/visualization/graphs/util/
--rw-rw-rw-   0        0        0      786 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/util/__init__.py
--rw-rw-rw-   0        0        0     2791 2023-04-05 11:57:19.000000 pm4py-2.7.4/pm4py/visualization/graphs/util/common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.547279 pm4py-2.7.4/pm4py/visualization/graphs/variants/
--rw-rw-rw-   0        0        0      817 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/variants/__init__.py
--rw-rw-rw-   0        0        0     4548 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/variants/attributes.py
--rw-rw-rw-   0        0        0     2770 2023-04-03 08:54:35.000000 pm4py-2.7.4/pm4py/visualization/graphs/variants/barplot.py
--rw-rw-rw-   0        0        0     4549 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/variants/cases.py
--rw-rw-rw-   0        0        0     4594 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/variants/dates.py
--rw-rw-rw-   0        0        0     3873 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/graphs/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.547279 pm4py-2.7.4/pm4py/visualization/heuristics_net/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/heuristics_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.547279 pm4py-2.7.4/pm4py/visualization/heuristics_net/variants/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/heuristics_net/variants/__init__.py
--rw-rw-rw-   0        0        0    13224 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
--rw-rw-rw-   0        0        0     4470 2023-04-05 11:57:19.000000 pm4py-2.7.4/pm4py/visualization/heuristics_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.562901 pm4py-2.7.4/pm4py/visualization/network_analysis/
--rw-rw-rw-   0        0        0      805 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/network_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.562901 pm4py-2.7.4/pm4py/visualization/network_analysis/variants/
--rw-rw-rw-   0        0        0      816 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/network_analysis/variants/__init__.py
--rw-rw-rw-   0        0        0     4951 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/network_analysis/variants/frequency.py
--rw-rw-rw-   0        0        0     6130 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/network_analysis/variants/performance.py
--rw-rw-rw-   0        0        0     2481 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/network_analysis/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.562901 pm4py-2.7.4/pm4py/visualization/ocel/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.578522 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/
--rw-rw-rw-   0        0        0      807 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.578522 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/variants/
--rw-rw-rw-   0        0        0      804 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/variants/__init__.py
--rw-rw-rw-   0        0        0    14981 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py
--rw-rw-rw-   0        0        0     2989 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/interleavings/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.578522 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.578522 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/variants/
--rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/variants/__init__.py
--rw-rw-rw-   0        0        0     3388 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py
--rw-rw-rw-   0        0        0     2541 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/object_graph/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.594143 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/
--rw-rw-rw-   0        0        0      799 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.594143 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/variants/
--rw-rw-rw-   0        0        0      795 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py
--rw-rw-rw-   0        0        0    12244 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/variants/classic.py
--rw-rw-rw-   0        0        0     2439 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.594143 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/
--rw-rw-rw-   0        0        0      798 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.594143 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/variants/
--rw-rw-rw-   0        0        0      800 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/variants/__init__.py
--rw-rw-rw-   0        0        0     5000 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     2586 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/ocel/ocpn/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.609768 pm4py-2.7.4/pm4py/visualization/performance_spectrum/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/performance_spectrum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.609768 pm4py-2.7.4/pm4py/visualization/performance_spectrum/variants/
--rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/performance_spectrum/variants/__init__.py
--rw-rw-rw-   0        0        0     7035 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/performance_spectrum/variants/neato.py
--rw-rw-rw-   0        0        0     3229 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/visualization/performance_spectrum/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.609768 pm4py-2.7.4/pm4py/visualization/petri_net/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.609768 pm4py-2.7.4/pm4py/visualization/petri_net/common/
--rw-rw-rw-   0        0        0      794 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/common/__init__.py
--rw-rw-rw-   0        0        0     9490 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/common/visualize.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.625386 pm4py-2.7.4/pm4py/visualization/petri_net/util/
--rw-rw-rw-   0        0        0      847 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/util/__init__.py
--rw-rw-rw-   0        0        0     2935 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/util/alignments_decoration.py
--rw-rw-rw-   0        0        0     1121 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/util/performance_map.py
--rw-rw-rw-   0        0        0    11279 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.631892 pm4py-2.7.4/pm4py/visualization/petri_net/variants/
--rw-rw-rw-   0        0        0      937 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/alignments.py
--rw-rw-rw-   0        0        0     4750 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
--rw-rw-rw-   0        0        0     4857 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
--rw-rw-rw-   0        0        0     5690 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
--rw-rw-rw-   0        0        0     5900 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py
--rw-rw-rw-   0        0        0     2257 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     3807 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/petri_net/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.647519 pm4py-2.7.4/pm4py/visualization/process_tree/
--rw-rw-rw-   0        0        0      801 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.647519 pm4py-2.7.4/pm4py/visualization/process_tree/variants/
--rw-rw-rw-   0        0        0      813 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/variants/__init__.py
--rw-rw-rw-   0        0        0     4713 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/variants/frequency_annotation.py
--rw-rw-rw-   0        0        0     3951 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/variants/symbolic.py
--rw-rw-rw-   0        0        0     4083 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/variants/wo_decoration.py
--rw-rw-rw-   0        0        0     2813 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/process_tree/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.663141 pm4py-2.7.4/pm4py/visualization/sna/
--rw-rw-rw-   0        0        0      792 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/sna/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.663141 pm4py-2.7.4/pm4py/visualization/sna/variants/
--rw-rw-rw-   0        0        0      796 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/sna/variants/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-04-05 11:57:19.000000 pm4py-2.7.4/pm4py/visualization/sna/variants/networkx.py
--rw-rw-rw-   0        0        0     5429 2023-04-24 10:28:37.000000 pm4py-2.7.4/pm4py/visualization/sna/variants/pyvis.py
--rw-rw-rw-   0        0        0     2561 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/sna/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.663141 pm4py-2.7.4/pm4py/visualization/transition_system/
--rw-rw-rw-   0        0        0      812 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.678762 pm4py-2.7.4/pm4py/visualization/transition_system/util/
--rw-rw-rw-   0        0        0      809 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/util/__init__.py
--rw-rw-rw-   0        0        0     3291 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/util/visualize_graphviz.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.678762 pm4py-2.7.4/pm4py/visualization/transition_system/variants/
--rw-rw-rw-   0        0        0      822 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/variants/__init__.py
--rw-rw-rw-   0        0        0     3114 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/variants/trans_frequency.py
--rw-rw-rw-   0        0        0     1659 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/variants/view_based.py
--rw-rw-rw-   0        0        0     2702 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/transition_system/visualizer.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.678762 pm4py-2.7.4/pm4py/visualization/trie/
--rw-rw-rw-   0        0        0      793 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/trie/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.694383 pm4py-2.7.4/pm4py/visualization/trie/variants/
--rw-rw-rw-   0        0        0      789 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/trie/variants/__init__.py
--rw-rw-rw-   0        0        0     2737 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/trie/variants/classic.py
--rw-rw-rw-   0        0        0     2497 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/visualization/trie/visualizer.py
--rw-rw-rw-   0        0        0    12749 2023-03-27 13:12:18.000000 pm4py-2.7.4/pm4py/write.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:53.873230 pm4py-2.7.4/pm4py.egg-info/
--rw-rw-rw-   0        0        0     2683 2023-05-08 08:14:52.000000 pm4py-2.7.4/pm4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    60445 2023-05-08 08:14:53.000000 pm4py-2.7.4/pm4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 08:14:52.000000 pm4py-2.7.4/pm4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2023-05-08 08:14:52.000000 pm4py-2.7.4/pm4py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-08 08:14:52.000000 pm4py-2.7.4/pm4py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 08:14:56.694383 pm4py-2.7.4/setup.cfg
--rw-rw-rw-   0        0        0    22528 2023-03-27 13:12:18.000000 pm4py-2.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 08:14:56.694383 pm4py-2.7.4/tests/
--rw-rw-rw-   0        0        0     4971 2023-03-27 13:12:18.000000 pm4py-2.7.4/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.308836 pm4py-2.7.5/
+-rw-rw-rw-   0        0        0    34817 2023-03-27 13:12:16.000000 pm4py-2.7.5/LICENSE
+-rw-rw-rw-   0        0        0     2683 2023-06-30 14:33:07.304846 pm4py-2.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2249 2023-06-30 14:32:57.000000 pm4py-2.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.844297 pm4py-2.7.5/pm4py/
+-rw-rw-rw-   0        0        0     7322 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.884451 pm4py-2.7.5/pm4py/algo/
+-rw-rw-rw-   0        0        0      854 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.886446 pm4py-2.7.5/pm4py/algo/analysis/
+-rw-rw-rw-   0        0        0      833 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.889436 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     3588 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.894428 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/variants/
+-rw-rw-rw-   0        0        0      810 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    21448 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.899411 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/__init__.py
+-rw-rw-rw-   0        0        0     2689 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.903399 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/variants/__init__.py
+-rw-rw-rw-   0        0        0    11636 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/marking_equation/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.907439 pm4py-2.7.5/pm4py/algo/analysis/woflan/
+-rw-rw-rw-   0        0        0      836 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/__init__.py
+-rw-rw-rw-   0        0        0    32365 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.912431 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/
+-rw-rw-rw-   0        0        0      868 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.917416 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/
+-rw-rw-rw-   0        0        0      835 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     7988 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.921407 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/reachability_graph/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py
+-rw-rw-rw-   0        0        0     2451 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.925394 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/
+-rw-rw-rw-   0        0        0      841 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py
+-rw-rw-rw-   0        0        0     4061 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py
+-rw-rw-rw-   0        0        0     5745 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.931379 pm4py-2.7.5/pm4py/algo/analysis/woflan/not_well_handled_pairs/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py
+-rw-rw-rw-   0        0        0     2632 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.942350 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/
+-rw-rw-rw-   0        0        0      849 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/__init__.py
+-rw-rw-rw-   0        0        0     4269 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py
+-rw-rw-rw-   0        0        0     3668 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/s_component.py
+-rw-rw-rw-   0        0        0     1098 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py
+-rw-rw-rw-   0        0        0     8245 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.946339 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.951325 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/variants/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3257 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/analysis/workflow_net/variants/petri_net.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.953320 pm4py-2.7.5/pm4py/algo/anonymization/
+-rw-rw-rw-   0        0        0      967 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.958309 pm4py-2.7.5/pm4py/algo/anonymization/pripel/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/__init__.py
+-rw-rw-rw-   0        0        0     3170 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.967183 pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/
+-rw-rw-rw-   0        0        0    13889 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py
+-rw-rw-rw-   0        0        0    14468 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/TraceMatcher.py
+-rw-rw-rw-   0        0        0      837 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/__init__.py
+-rw-rw-rw-   0        0        0     1754 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.970178 pm4py-2.7.5/pm4py/algo/anonymization/pripel/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/variants/__init__.py
+-rw-rw-rw-   0        0        0     5291 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/pripel/variants/pripel.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.975165 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/__init__.py
+-rw-rw-rw-   0        0        0     3980 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.984142 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/
+-rw-rw-rw-   0        0        0      839 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/__init__.py
+-rw-rw-rw-   0        0        0     6862 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py
+-rw-rw-rw-   0        0        0     1323 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py
+-rw-rw-rw-   0        0        0     1687 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.990126 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/
+-rw-rw-rw-   0        0        0      817 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py
+-rw-rw-rw-   0        0        0     7677 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py
+-rw-rw-rw-   0        0        0    11317 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.992120 pm4py-2.7.5/pm4py/algo/clustering/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.996111 pm4py-2.7.5/pm4py/algo/clustering/profiles/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/profiles/__init__.py
+-rw-rw-rw-   0        0        0     2118 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.001096 pm4py-2.7.5/pm4py/algo/clustering/profiles/variants/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0     3544 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.006085 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/
+-rw-rw-rw-   0        0        0      984 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/__init__.py
+-rw-rw-rw-   0        0        0     4712 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.009074 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/dfg/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3892 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.013064 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/leven_dist/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py
+-rw-rw-rw-   0        0        0     5473 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.018052 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/linkage_method/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py
+-rw-rw-rw-   0        0        0    13583 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.023038 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/merge_log/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py
+-rw-rw-rw-   0        0        0     4290 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.032014 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/
+-rw-rw-rw-   0        0        0      824 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py
+-rw-rw-rw-   0        0        0     3396 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py
+-rw-rw-rw-   0        0        0    15534 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.045977 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/
+-rw-rw-rw-   0        0        0      855 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py
+-rw-rw-rw-   0        0        0    18357 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py
+-rw-rw-rw-   0        0        0     6772 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py
+-rw-rw-rw-   0        0        0     6295 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py
+-rw-rw-rw-   0        0        0    15717 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.048968 pm4py-2.7.5/pm4py/algo/comparison/
+-rw-rw-rw-   0        0        0      940 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/comparison/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.056948 pm4py-2.7.5/pm4py/algo/comparison/petrinet/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/comparison/petrinet/__init__.py
+-rw-rw-rw-   0        0        0     6739 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/comparison/petrinet/element_usage_comparison.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.059939 pm4py-2.7.5/pm4py/algo/conformance/
+-rw-rw-rw-   0        0        0      946 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.062931 pm4py-2.7.5/pm4py/algo/conformance/alignments/
+-rw-rw-rw-   0        0        0      838 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.071907 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/__init__.py
+-rw-rw-rw-   0        0        0     2025 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.076893 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/variants/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py
+-rw-rw-rw-   0        0        0    19023 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.085870 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1956 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.091855 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/variants/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    20411 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.098942 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/
+-rw-rw-rw-   0        0        0      918 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/__init__.py
+-rw-rw-rw-   0        0        0     1876 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.108809 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/variants/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     7202 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.128755 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/__init__.py
+-rw-rw-rw-   0        0        0    17405 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.149699 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/utils/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0     2896 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.180619 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/
+-rw-rw-rw-   0        0        0      925 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    27653 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17218 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    23651 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py
+-rw-rw-rw-   0        0        0    23624 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py
+-rw-rw-rw-   0        0        0    17546 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py
+-rw-rw-rw-   0        0        0    24029 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py
+-rw-rw-rw-   0        0        0    27972 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.186599 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     2279 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.199566 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/
+-rw-rw-rw-   0        0        0      870 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py
+-rw-rw-rw-   0        0        0    15712 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.204555 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/
+-rw-rw-rw-   0        0        0      833 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.218516 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/
+-rw-rw-rw-   0        0        0      871 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py
+-rw-rw-rw-   0        0        0     5361 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py
+-rw-rw-rw-   0        0        0    49808 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py
+-rw-rw-rw-   0        0        0    36425 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py
+-rw-rw-rw-   0        0        0     6660 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py
+-rw-rw-rw-   0        0        0    17913 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.223501 pm4py-2.7.5/pm4py/algo/conformance/antialignments/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/antialignments/__init__.py
+-rw-rw-rw-   0        0        0     3166 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/antialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.228487 pm4py-2.7.5/pm4py/algo/conformance/antialignments/variants/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/antialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     7582 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.237464 pm4py-2.7.5/pm4py/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     2073 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.245443 pm4py-2.7.5/pm4py/algo/conformance/footprints/util/
+-rw-rw-rw-   0        0        0      817 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/util/__init__.py
+-rw-rw-rw-   0        0        0     6154 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/util/evaluation.py
+-rw-rw-rw-   0        0        0     3573 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/util/tree_visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.256413 pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      832 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/log_extensive.py
+-rw-rw-rw-   0        0        0     5095 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/log_model.py
+-rw-rw-rw-   0        0        0     7117 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/trace_extensive.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.261400 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.270376 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    13187 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.276360 pm4py-2.7.5/pm4py/algo/conformance/multialignments/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/multialignments/__init__.py
+-rw-rw-rw-   0        0        0     3143 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/multialignments/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.284338 pm4py-2.7.5/pm4py/algo/conformance/multialignments/variants/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/multialignments/variants/__init__.py
+-rw-rw-rw-   0        0        0     6557 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.293315 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     4645 2023-04-26 05:58:14.000000 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.303290 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      929 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     5418 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5999 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.311267 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/
+-rw-rw-rw-   0        0        0      815 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/__init__.py
+-rw-rw-rw-   0        0        0     3041 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.320243 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/
+-rw-rw-rw-   0        0        0      836 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     6439 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py
+-rw-rw-rw-   0        0        0    10823 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.329219 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/__init__.py
+-rw-rw-rw-   0        0        0    12117 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/backwards.py
+-rw-rw-rw-   0        0        0    59010 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.335203 pm4py-2.7.5/pm4py/algo/connectors/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.339192 pm4py-2.7.5/pm4py/algo/connectors/util/
+-rw-rw-rw-   0        0        0      781 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/util/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/util/mail.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.364954 pm4py-2.7.5/pm4py/algo/connectors/variants/
+-rw-rw-rw-   0        0        0      736 2023-03-28 09:25:12.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/__init__.py
+-rw-rw-rw-   0        0        0     2556 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/camunda_workflow.py
+-rw-rw-rw-   0        0        0     3645 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/chrome_history.py
+-rw-rw-rw-   0        0        0     3598 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/firefox_history.py
+-rw-rw-rw-   0        0        0     5034 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/github_repo.py
+-rw-rw-rw-   0        0        0     4166 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/outlook_calendar.py
+-rw-rw-rw-   0        0        0     4354 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/outlook_mail_extractor.py
+-rw-rw-rw-   0        0        0     3132 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/sap_accounting.py
+-rw-rw-rw-   0        0        0     3976 2023-03-28 05:40:06.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/sap_o2c.py
+-rw-rw-rw-   0        0        0     4110 2023-03-27 13:13:01.000000 pm4py-2.7.5/pm4py/algo/connectors/variants/windows_events.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.369112 pm4py-2.7.5/pm4py/algo/decision_mining/
+-rw-rw-rw-   0        0        0      888 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/decision_mining/__init__.py
+-rw-rw-rw-   0        0        0    23391 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/decision_mining/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.372105 pm4py-2.7.5/pm4py/algo/discovery/
+-rw-rw-rw-   0        0        0     1035 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.376093 pm4py-2.7.5/pm4py/algo/discovery/alpha/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/__init__.py
+-rw-rw-rw-   0        0        0     5090 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.382079 pm4py-2.7.5/pm4py/algo/discovery/alpha/data_structures/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/data_structures/__init__.py
+-rw-rw-rw-   0        0        0     2420 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.387064 pm4py-2.7.5/pm4py/algo/discovery/alpha/utils/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/utils/__init__.py
+-rw-rw-rw-   0        0        0     1622 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/utils/endpoints.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.394047 pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/__init__.py
+-rw-rw-rw-   0        0        0    10923 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/classic.py
+-rw-rw-rw-   0        0        0    22108 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/plus.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.400029 pm4py-2.7.5/pm4py/algo/discovery/batches/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/__init__.py
+-rw-rw-rw-   0        0        0     3724 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.405016 pm4py-2.7.5/pm4py/algo/discovery/batches/utils/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/utils/__init__.py
+-rw-rw-rw-   0        0        0     9636 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/utils/detection.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.411000 pm4py-2.7.5/pm4py/algo/discovery/batches/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/variants/__init__.py
+-rw-rw-rw-   0        0        0     5216 2023-03-27 13:12:16.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/variants/log.py
+-rw-rw-rw-   0        0        0     6111 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/batches/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.416984 pm4py-2.7.5/pm4py/algo/discovery/causal/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/causal/__init__.py
+-rw-rw-rw-   0        0        0     1668 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/causal/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.424962 pm4py-2.7.5/pm4py/algo/discovery/causal/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/causal/variants/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/causal/variants/alpha.py
+-rw-rw-rw-   0        0        0     1611 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/causal/variants/heuristic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.432942 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/__init__.py
+-rw-rw-rw-   0        0        0     2249 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/algorithm.py
+-rw-rw-rw-   0        0        0     7934 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.441917 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/
+-rw-rw-rw-   0        0        0      832 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/__init__.py
+-rw-rw-rw-   0        0        0     9665 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/classic.py
+-rw-rw-rw-   0        0        0     4390 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/classic_split.py
+-rw-rw-rw-   0        0        0    10277 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.450894 pm4py-2.7.5/pm4py/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      822 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.452888 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.461864 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py
+-rw-rw-rw-   0        0        0    14930 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py
+-rw-rw-rw-   0        0        0     2902 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py
+-rw-rw-rw-   0        0        0     5200 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     1260 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/replacement.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.469843 pm4py-2.7.5/pm4py/algo/discovery/dfg/utils/
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.491786 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      958 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     4609 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/case_attributes.py
+-rw-rw-rw-   0        0        0     2852 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/clean.py
+-rw-rw-rw-   0        0        0     2795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/clean_polars.py
+-rw-rw-rw-   0        0        0     2200 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/freq_triples.py
+-rw-rw-rw-   0        0        0     2597 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/native.py
+-rw-rw-rw-   0        0        0     5836 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.499763 pm4py-2.7.5/pm4py/algo/discovery/footprints/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/__init__.py
+-rw-rw-rw-   0        0        0     3227 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.502755 pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.507742 pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/variants/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     2265 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/variants/dfg.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.510733 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.522701 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/
+-rw-rw-rw-   0        0        0      843 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     4610 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py
+-rw-rw-rw-   0        0        0     3357 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py
+-rw-rw-rw-   0        0        0     3282 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.525693 pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.533672 pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/variants/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/variants/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.536663 pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.541650 pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/variants/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    13417 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/variants/bottomup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.550627 pm4py-2.7.5/pm4py/algo/discovery/heuristics/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/heuristics/__init__.py
+-rw-rw-rw-   0        0        0     7559 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/heuristics/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.558607 pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/__init__.py
+-rw-rw-rw-   0        0        0    26234 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/classic.py
+-rw-rw-rw-   0        0        0    24321 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/plusplus.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.562594 pm4py-2.7.5/pm4py/algo/discovery/ilp/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ilp/__init__.py
+-rw-rw-rw-   0        0        0     1782 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ilp/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.569575 pm4py-2.7.5/pm4py/algo/discovery/ilp/variants/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ilp/variants/__init__.py
+-rw-rw-rw-   0        0        0    12788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ilp/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.574562 pm4py-2.7.5/pm4py/algo/discovery/inductive/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/__init__.py
+-rw-rw-rw-   0        0        0     3790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.587528 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/
+-rw-rw-rw-   0        0        0      829 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/__init__.py
+-rw-rw-rw-   0        0        0     1533 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/abc.py
+-rw-rw-rw-   0        0        0     1768 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/empty_log.py
+-rw-rw-rw-   0        0        0     2268 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/factory.py
+-rw-rw-rw-   0        0        0     2060 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/single_activity.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.618445 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/__init__.py
+-rw-rw-rw-   0        0        0     2100 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/abc.py
+-rw-rw-rw-   0        0        0     4570 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/concurrency.py
+-rw-rw-rw-   0        0        0     2463 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/factory.py
+-rw-rw-rw-   0        0        0    10916 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/loop.py
+-rw-rw-rw-   0        0        0    11571 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/sequence.py
+-rw-rw-rw-   0        0        0     1104 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/utils.py
+-rw-rw-rw-   0        0        0     4316 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/xor.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.626424 pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/__init__.py
+-rw-rw-rw-   0        0        0     1050 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/im_dfg.py
+-rw-rw-rw-   0        0        0     2568 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/im_ds.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.651358 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/
+-rw-rw-rw-   0        0        0      897 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/__init__.py
+-rw-rw-rw-   0        0        0     1385 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/abc.py
+-rw-rw-rw-   0        0        0     4792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py
+-rw-rw-rw-   0        0        0     1643 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py
+-rw-rw-rw-   0        0        0     2709 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/empty_traces.py
+-rw-rw-rw-   0        0        0     2672 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/factory.py
+-rw-rw-rw-   0        0        0     3059 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/flower.py
+-rw-rw-rw-   0        0        0     2441 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py
+-rw-rw-rw-   0        0        0     1520 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/tau_loop.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.668312 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/abc.py
+-rw-rw-rw-   0        0        0     1740 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/im.py
+-rw-rw-rw-   0        0        0     1098 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/imd.py
+-rw-rw-rw-   0        0        0     4381 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/imf.py
+-rw-rw-rw-   0        0        0      881 2023-06-30 05:23:04.000000 pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/instances.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.676291 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/
+-rw-rw-rw-   0        0        0      815 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/__init__.py
+-rw-rw-rw-   0        0        0     2520 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/algorithm.py
+-rw-rw-rw-   0        0        0     3194 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/trace_skel.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.681278 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/variants/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/variants/__init__.py
+-rw-rw-rw-   0        0        0    11119 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.689256 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/algorithm.py
+-rw-rw-rw-   0        0        0     3132 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.695239 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/
+-rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     2878 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/log.py
+-rw-rw-rw-   0        0        0     2883 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.699228 pm4py-2.7.5/pm4py/algo/discovery/ocel/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.706210 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/
+-rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/__init__.py
+-rw-rw-rw-   0        0        0     2007 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.710200 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/utils/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py
+-rw-rw-rw-   0        0        0     4441 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.715187 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0     6622 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.721170 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1841 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.725161 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/variants/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     6497 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.730147 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/__init__.py
+-rw-rw-rw-   0        0        0     1775 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.736131 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     5629 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.741118 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/__init__.py
+-rw-rw-rw-   0        0        0     1780 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.746105 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0     4718 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.751091 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/__init__.py
+-rw-rw-rw-   0        0        0     1800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.756077 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py
+-rw-rw-rw-   0        0        0     7010 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.760066 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3570 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.775027 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      855 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     4307 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5045 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py
+-rw-rw-rw-   0        0        0     3402 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/log.py
+-rw-rw-rw-   0        0        0     4386 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.778019 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.786996 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/
+-rw-rw-rw-   0        0        0      925 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/__init__.py
+-rw-rw-rw-   0        0        0     4044 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/dataframe.py
+-rw-rw-rw-   0        0        0     5278 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/log.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.791981 pm4py-2.7.5/pm4py/algo/discovery/transition_system/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/transition_system/__init__.py
+-rw-rw-rw-   0        0        0     1991 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/transition_system/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.798962 pm4py-2.7.5/pm4py/algo/discovery/transition_system/variants/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     5900 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/discovery/transition_system/variants/view_based.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.803948 pm4py-2.7.5/pm4py/algo/evaluation/
+-rw-rw-rw-   0        0        0      836 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/__init__.py
+-rw-rw-rw-   0        0        0     4839 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.808936 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/
+-rw-rw-rw-   0        0        0      919 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/__init__.py
+-rw-rw-rw-   0        0        0     1692 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.814921 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/variants/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py
+-rw-rw-rw-   0        0        0     4871 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.819908 pm4py-2.7.5/pm4py/algo/evaluation/generalization/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/generalization/__init__.py
+-rw-rw-rw-   0        0        0     1710 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/generalization/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.823895 pm4py-2.7.5/pm4py/algo/evaluation/generalization/variants/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/generalization/variants/__init__.py
+-rw-rw-rw-   0        0        0     4674 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/generalization/variants/token_based.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.832873 pm4py-2.7.5/pm4py/algo/evaluation/precision/
+-rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/__init__.py
+-rw-rw-rw-   0        0        0     3071 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.837858 pm4py-2.7.5/pm4py/algo/evaluation/precision/dfg/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/dfg/__init__.py
+-rw-rw-rw-   0        0        0     3992 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/dfg/algorithm.py
+-rw-rw-rw-   0        0        0     5463 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.845839 pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/
+-rw-rw-rw-   0        0        0      829 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/__init__.py
+-rw-rw-rw-   0        0        0    13827 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/align_etconformance.py
+-rw-rw-rw-   0        0        0     6196 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/etconformance_token.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.850824 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/__init__.py
+-rw-rw-rw-   0        0        0     4576 2023-06-30 05:23:18.000000 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.857805 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/
+-rw-rw-rw-   0        0        0      823 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/__init__.py
+-rw-rw-rw-   0        0        0     6835 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py
+-rw-rw-rw-   0        0        0     5190 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.864786 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/__init__.py
+-rw-rw-rw-   0        0        0     1686 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.874759 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/
+-rw-rw-rw-   0        0        0      841 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/__init__.py
+-rw-rw-rw-   0        0        0     2790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/arc_degree.py
+-rw-rw-rw-   0        0        0     1602 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py
+-rw-rw-rw-   0        0        0     2120 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.877753 pm4py-2.7.5/pm4py/algo/filtering/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.883736 pm4py-2.7.5/pm4py/algo/filtering/common/
+-rw-rw-rw-   0        0        0      852 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.888722 pm4py-2.7.5/pm4py/algo/filtering/common/attributes/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/attributes/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/attributes/attributes_common.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.893710 pm4py-2.7.5/pm4py/algo/filtering/common/end_activities/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/end_activities/__init__.py
+-rw-rw-rw-   0        0        0      851 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/end_activities/end_activities_common.py
+-rw-rw-rw-   0        0        0      845 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/filtering_constants.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.899693 pm4py-2.7.5/pm4py/algo/filtering/common/start_activities/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/start_activities/__init__.py
+-rw-rw-rw-   0        0        0      857 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/start_activities/start_activities_common.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.903682 pm4py-2.7.5/pm4py/algo/filtering/common/timestamp/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     1208 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/common/timestamp/timestamp_common.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.909666 pm4py-2.7.5/pm4py/algo/filtering/dfg/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/dfg/__init__.py
+-rw-rw-rw-   0        0        0    25920 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/dfg/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.911661 pm4py-2.7.5/pm4py/algo/filtering/log/
+-rw-rw-rw-   0        0        0      866 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.917645 pm4py-2.7.5/pm4py/algo/filtering/log/attr_value_repetition/
+-rw-rw-rw-   0        0        0      918 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2754 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.921634 pm4py-2.7.5/pm4py/algo/filtering/log/attributes/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/attributes/__init__.py
+-rw-rw-rw-   0        0        0    18535 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.927618 pm4py-2.7.5/pm4py/algo/filtering/log/between/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/between/__init__.py
+-rw-rw-rw-   0        0        0     2944 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.933605 pm4py-2.7.5/pm4py/algo/filtering/log/cases/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/cases/__init__.py
+-rw-rw-rw-   0        0        0     4661 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.937592 pm4py-2.7.5/pm4py/algo/filtering/log/end_activities/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     4067 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.942578 pm4py-2.7.5/pm4py/algo/filtering/log/ltl/
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11165 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.948564 pm4py-2.7.5/pm4py/algo/filtering/log/paths/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/paths/__init__.py
+-rw-rw-rw-   0        0        0     9848 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/paths/paths_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.952551 pm4py-2.7.5/pm4py/algo/filtering/log/prefixes/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3218 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.958535 pm4py-2.7.5/pm4py/algo/filtering/log/rework/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/rework/__init__.py
+-rw-rw-rw-   0        0        0     3412 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.963523 pm4py-2.7.5/pm4py/algo/filtering/log/start_activities/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     4358 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.968508 pm4py-2.7.5/pm4py/algo/filtering/log/suffixes/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3223 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.978484 pm4py-2.7.5/pm4py/algo/filtering/log/timestamp/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/timestamp/__init__.py
+-rw-rw-rw-   0        0        0    11514 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:04.984466 pm4py-2.7.5/pm4py/algo/filtering/log/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     9229 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/log/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.000423 pm4py-2.7.5/pm4py/algo/filtering/ocel/
+-rw-rw-rw-   0        0        0      865 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3392 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/activity_type_matching.py
+-rw-rw-rw-   0        0        0     3843 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/event_attributes.py
+-rw-rw-rw-   0        0        0     2319 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/object_attributes.py
+-rw-rw-rw-   0        0        0     3436 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     4262 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/ocel/ot_endpoints.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.006407 pm4py-2.7.5/pm4py/algo/filtering/pandas/
+-rw-rw-rw-   0        0        0      891 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.010396 pm4py-2.7.5/pm4py/algo/filtering/pandas/attr_value_repetition/
+-rw-rw-rw-   0        0        0      921 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py
+-rw-rw-rw-   0        0        0     2786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.015383 pm4py-2.7.5/pm4py/algo/filtering/pandas/attributes/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/attributes/__init__.py
+-rw-rw-rw-   0        0        0    13483 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/attributes/attributes_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.021367 pm4py-2.7.5/pm4py/algo/filtering/pandas/between/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/between/__init__.py
+-rw-rw-rw-   0        0        0     3266 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/between/between_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.026356 pm4py-2.7.5/pm4py/algo/filtering/pandas/cases/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/cases/__init__.py
+-rw-rw-rw-   0        0        0     6315 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/cases/case_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.032339 pm4py-2.7.5/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/
+-rw-rw-rw-   0        0        0      842 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3079 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.037324 pm4py-2.7.5/pm4py/algo/filtering/pandas/end_activities/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/end_activities/__init__.py
+-rw-rw-rw-   0        0        0     6348 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.041314 pm4py-2.7.5/pm4py/algo/filtering/pandas/ends_with/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/ends_with/__init__.py
+-rw-rw-rw-   0        0        0     3745 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.046301 pm4py-2.7.5/pm4py/algo/filtering/pandas/ltl/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/ltl/__init__.py
+-rw-rw-rw-   0        0        0    11785 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/ltl/ltl_checker.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.052285 pm4py-2.7.5/pm4py/algo/filtering/pandas/paths/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/paths/__init__.py
+-rw-rw-rw-   0        0        0     6897 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/paths/paths_filter.py
+-rw-rw-rw-   0        0        0      832 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/pd_filtering_constants.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.057271 pm4py-2.7.5/pm4py/algo/filtering/pandas/prefixes/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/prefixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.061261 pm4py-2.7.5/pm4py/algo/filtering/pandas/rework/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/rework/__init__.py
+-rw-rw-rw-   0        0        0     3383 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/rework/rework_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.068241 pm4py-2.7.5/pm4py/algo/filtering/pandas/start_activities/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/start_activities/__init__.py
+-rw-rw-rw-   0        0        0     5738 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.073230 pm4py-2.7.5/pm4py/algo/filtering/pandas/starts_with/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/starts_with/__init__.py
+-rw-rw-rw-   0        0        0     3747 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.077218 pm4py-2.7.5/pm4py/algo/filtering/pandas/suffixes/
+-rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/suffixes/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.083202 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp/__init__.py
+-rw-rw-rw-   0        0        0     8848 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.088189 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp_case_grouping/
+-rw-rw-rw-   0        0        0      830 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py
+-rw-rw-rw-   0        0        0     3504 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.093175 pm4py-2.7.5/pm4py/algo/filtering/pandas/traces/
+-rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/traces/__init__.py
+-rw-rw-rw-   0        0        0     4030 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/traces/trace_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.100156 pm4py-2.7.5/pm4py/algo/filtering/pandas/variants/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     6219 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/filtering/pandas/variants/variants_filter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.102151 pm4py-2.7.5/pm4py/algo/merging/
+-rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/merging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.107138 pm4py-2.7.5/pm4py/algo/merging/case_relations/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/merging/case_relations/__init__.py
+-rw-rw-rw-   0        0        0     2326 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/merging/case_relations/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.111127 pm4py-2.7.5/pm4py/algo/merging/case_relations/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/merging/case_relations/variants/__init__.py
+-rw-rw-rw-   0        0        0     3474 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/merging/case_relations/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.117111 pm4py-2.7.5/pm4py/algo/organizational_mining/
+-rw-rw-rw-   0        0        0      855 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.122098 pm4py-2.7.5/pm4py/algo/organizational_mining/local_diagnostics/
+-rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/local_diagnostics/__init__.py
+-rw-rw-rw-   0        0        0    12486 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.126087 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/
+-rw-rw-rw-   0        0        0      817 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1840 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.131074 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0    10571 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.136062 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/__init__.py
+-rw-rw-rw-   0        0        0    12016 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.142045 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py
+-rw-rw-rw-   0        0        0    23662 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/log.py
+-rw-rw-rw-   0        0        0    24339 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.150024 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/
+-rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/__init__.py
+-rw-rw-rw-   0        0        0     2502 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.154013 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/common/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/common/__init__.py
+-rw-rw-rw-   0        0        0     8411 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/common/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.159996 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/__init__.py
+-rw-rw-rw-   0        0        0     2448 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/log.py
+-rw-rw-rw-   0        0        0     2209 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.168973 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/
+-rw-rw-rw-   0        0        0      810 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/__init__.py
+-rw-rw-rw-   0        0        0     3689 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/algorithm.py
+-rw-rw-rw-   0        0        0     3199 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.171965 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.185927 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/
+-rw-rw-rw-   0        0        0      857 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     3735 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/handover.py
+-rw-rw-rw-   0        0        0     3286 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py
+-rw-rw-rw-   0        0        0     3525 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py
+-rw-rw-rw-   0        0        0     3155 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/working_together.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.198893 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/
+-rw-rw-rw-   0        0        0      860 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4235 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
+-rw-rw-rw-   0        0        0     2986 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
+-rw-rw-rw-   0        0        0     3804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
+-rw-rw-rw-   0        0        0     3432 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
+-rw-rw-rw-   0        0        0     7599 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/organizational_mining/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.200887 pm4py-2.7.5/pm4py/algo/querying/
+-rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/querying/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.202881 pm4py-2.7.5/pm4py/algo/querying/llm/
+-rw-rw-rw-   0        0        0      798 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.227815 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/
+-rw-rw-rw-   0        0        0      960 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/__init__.py
+-rw-rw-rw-   0        0        0     3946 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/case_to_descr.py
+-rw-rw-rw-   0        0        0     3080 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
+-rw-rw-rw-   0        0        0     4160 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
+-rw-rw-rw-   0        0        0     6317 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
+-rw-rw-rw-   0        0        0     4428 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
+-rw-rw-rw-   0        0        0     2839 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/logske_to_descr.py
+-rw-rw-rw-   0        0        0     1931 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/net_to_descr.py
+-rw-rw-rw-   0        0        0     5528 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
+-rw-rw-rw-   0        0        0     3680 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
+-rw-rw-rw-   0        0        0     3004 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/stream_to_descr.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.232802 pm4py-2.7.5/pm4py/algo/querying/llm/connectors/
+-rw-rw-rw-   0        0        0      791 2023-06-30 13:58:32.000000 pm4py-2.7.5/pm4py/algo/querying/llm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     1543 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/querying/llm/connectors/openai.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.234796 pm4py-2.7.5/pm4py/algo/reduction/
+-rw-rw-rw-   0        0        0      879 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/reduction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.238785 pm4py-2.7.5/pm4py/algo/reduction/process_tree/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/reduction/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1601 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/reduction/process_tree/reducer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.243773 pm4py-2.7.5/pm4py/algo/reduction/process_tree/variants/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/reduction/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     3766 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.245767 pm4py-2.7.5/pm4py/algo/simulation/
+-rw-rw-rw-   0        0        0      892 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.250754 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/
+-rw-rw-rw-   0        0        0      919 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/__init__.py
+-rw-rw-rw-   0        0        0     4575 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.254744 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/utils/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/utils/__init__.py
+-rw-rw-rw-   0        0        0     5327 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/utils/replay.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.258734 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/variants/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/variants/__init__.py
+-rw-rw-rw-   0        0        0    19795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.260728 pm4py-2.7.5/pm4py/algo/simulation/playout/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.265714 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1953 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.274690 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/
+-rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    14546 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/classic.py
+-rw-rw-rw-   0        0        0     6018 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/performance.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.278679 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/__init__.py
+-rw-rw-rw-   0        0        0     2579 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.289650 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/
+-rw-rw-rw-   0        0        0      821 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     9045 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py
+-rw-rw-rw-   0        0        0     5225 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/extensive.py
+-rw-rw-rw-   0        0        0     7927 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.293638 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/
+-rw-rw-rw-   0        0        0      810 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1889 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.301617 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/
+-rw-rw-rw-   0        0        0      835 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     1722 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py
+-rw-rw-rw-   0        0        0    13591 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/extensive.py
+-rw-rw-rw-   0        0        0     4891 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.306604 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/__init__.py
+-rw-rw-rw-   0        0        0     1779 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.312589 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/__init__.py
+-rw-rw-rw-   0        0        0     5364 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/basic.py
+-rw-rw-rw-   0        0        0    12993 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.315580 pm4py-2.7.5/pm4py/algo/transformation/
+-rw-rw-rw-   0        0        0      824 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.319569 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.324556 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/util/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/util/__init__.py
+-rw-rw-rw-   0        0        0     3901 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.333532 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/
+-rw-rw-rw-   0        0        0      823 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/__init__.py
+-rw-rw-rw-   0        0        0     6689 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/event_based.py
+-rw-rw-rw-   0        0        0     6610 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/temporal.py
+-rw-rw-rw-   0        0        0    50336 2023-06-30 05:23:33.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/trace_based.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.339516 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/
+-rw-rw-rw-   0        0        0      923 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/__init__.py
+-rw-rw-rw-   0        0        0     2171 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.343505 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/variants/
+-rw-rw-rw-   0        0        0      814 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     3439 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.348492 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/__init__.py
+-rw-rw-rw-   0        0        0     2161 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.357468 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/
+-rw-rw-rw-   0        0        0      837 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/__init__.py
+-rw-rw-rw-   0        0        0     2922 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/next_activity.py
+-rw-rw-rw-   0        0        0     2526 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/next_time.py
+-rw-rw-rw-   0        0        0     2385 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/remaining_time.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.362456 pm4py-2.7.5/pm4py/algo/transformation/log_to_trie/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_trie/__init__.py
+-rw-rw-rw-   0        0        0     2262 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/log_to_trie/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.365449 pm4py-2.7.5/pm4py/algo/transformation/ocel/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.374424 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/
+-rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/__init__.py
+-rw-rw-rw-   0        0        0     1684 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.379409 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/variants/
+-rw-rw-rw-   0        0        0      736 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/variants/__init__.py
+-rw-rw-rw-   0        0        0     3318 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/description/variants/variant1.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.382404 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/
+-rw-rw-rw-   0        0        0      821 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.427282 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/
+-rw-rw-rw-   0        0        0     1002 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/__init__.py
+-rw-rw-rw-   0        0        0     9033 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/algorithm.py
+-rw-rw-rw-   0        0        0     1890 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_activity.py
+-rw-rw-rw-   0        0        0     1991 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_end_ot.py
+-rw-rw-rw-   0        0        0     2467 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py
+-rw-rw-rw-   0        0        0     1608 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py
+-rw-rw-rw-   0        0        0     2212 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py
+-rw-rw-rw-   0        0        0     1970 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_start_ot.py
+-rw-rw-rw-   0        0        0     2956 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py
+-rw-rw-rw-   0        0        0     1948 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_timestamp.py
+-rw-rw-rw-   0        0        0     1905 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/new_interactions.py
+-rw-rw-rw-   0        0        0     2722 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/related_objects_features.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.456204 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/
+-rw-rw-rw-   0        0        0      831 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/__init__.py
+-rw-rw-rw-   0        0        0     3843 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py
+-rw-rw-rw-   0        0        0     4874 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.528012 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/
+-rw-rw-rw-   0        0        0     1268 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/__init__.py
+-rw-rw-rw-   0        0        0    18595 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/algorithm.py
+-rw-rw-rw-   0        0        0     3377 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py
+-rw-rw-rw-   0        0        0     1827 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     1827 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     1901 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py
+-rw-rw-rw-   0        0        0     2015 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py
+-rw-rw-rw-   0        0        0     2067 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1857 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py
+-rw-rw-rw-   0        0        0     1868 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py
+-rw-rw-rw-   0        0        0     2004 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py
+-rw-rw-rw-   0        0        0     1631 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py
+-rw-rw-rw-   0        0        0     2094 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py
+-rw-rw-rw-   0        0        0     1750 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py
+-rw-rw-rw-   0        0        0     2499 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py
+-rw-rw-rw-   0        0        0     2975 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py
+-rw-rw-rw-   0        0        0     2394 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py
+-rw-rw-rw-   0        0        0     2342 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py
+-rw-rw-rw-   0        0        0     2978 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py
+-rw-rw-rw-   0        0        0     2713 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/related_events_features.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.553943 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/
+-rw-rw-rw-   0        0        0      906 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/__init__.py
+-rw-rw-rw-   0        0        0     2302 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py
+-rw-rw-rw-   0        0        0     2091 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py
+-rw-rw-rw-   0        0        0     2324 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py
+-rw-rw-rw-   0        0        0     2840 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py
+-rw-rw-rw-   0        0        0     1738 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py
+-rw-rw-rw-   0        0        0     3632 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.560925 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.569900 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     3423 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py
+-rw-rw-rw-   0        0        0     3505 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py
+-rw-rw-rw-   0        0        0    20258 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/analysis.py
+-rw-rw-rw-   0        0        0    13401 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/cli.py
+-rw-rw-rw-   0        0        0    45577 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/conformance.py
+-rw-rw-rw-   0        0        0    19636 2023-03-27 13:48:22.000000 pm4py-2.7.5/pm4py/connectors.py
+-rw-rw-rw-   0        0        0    19130 2023-04-25 06:11:22.000000 pm4py-2.7.5/pm4py/convert.py
+-rw-rw-rw-   0        0        0    45434 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/discovery.py
+-rw-rw-rw-   0        0        0    57976 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/filtering.py
+-rw-rw-rw-   0        0        0     5014 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/hof.py
+-rw-rw-rw-   0        0        0    16123 2023-06-30 14:15:06.000000 pm4py-2.7.5/pm4py/llm.py
+-rw-rw-rw-   0        0        0     1055 2023-06-30 05:23:33.000000 pm4py-2.7.5/pm4py/meta.py
+-rw-rw-rw-   0        0        0    16489 2023-04-26 10:56:14.000000 pm4py-2.7.5/pm4py/ml.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.573890 pm4py-2.7.5/pm4py/objects/
+-rw-rw-rw-   0        0        0      935 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.581868 pm4py-2.7.5/pm4py/objects/bpmn/
+-rw-rw-rw-   0        0        0      901 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.586855 pm4py-2.7.5/pm4py/objects/bpmn/exporter/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2130 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.592839 pm4py-2.7.5/pm4py/objects/bpmn/exporter/variants/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     7496 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/exporter/variants/etree.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.597826 pm4py-2.7.5/pm4py/objects/bpmn/importer/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/importer/__init__.py
+-rw-rw-rw-   0        0        0     2085 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/importer/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.603822 pm4py-2.7.5/pm4py/objects/bpmn/importer/variants/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    16488 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/importer/variants/lxml.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.609794 pm4py-2.7.5/pm4py/objects/bpmn/layout/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/layout/__init__.py
+-rw-rw-rw-   0        0        0     1534 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/layout/layouter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.614781 pm4py-2.7.5/pm4py/objects/bpmn/layout/variants/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/layout/variants/__init__.py
+-rw-rw-rw-   0        0        0    18042 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/layout/variants/graphviz.py
+-rw-rw-rw-   0        0        0    20950 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/obj.py
+-rw-rw-rw-   0        0        0     9205 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/semantics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.625751 pm4py-2.7.5/pm4py/objects/bpmn/util/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/util/__init__.py
+-rw-rw-rw-   0        0        0     6246 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/util/bpmn_utils.py
+-rw-rw-rw-   0        0        0     3352 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/util/reduction.py
+-rw-rw-rw-   0        0        0     3729 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/bpmn/util/sorting.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.629741 pm4py-2.7.5/pm4py/objects/conversion/
+-rw-rw-rw-   0        0        0      825 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.635725 pm4py-2.7.5/pm4py/objects/conversion/bpmn/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/bpmn/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/bpmn/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.639713 pm4py-2.7.5/pm4py/objects/conversion/bpmn/variants/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0    10026 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/bpmn/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.643703 pm4py-2.7.5/pm4py/objects/conversion/dfg/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/dfg/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.652678 pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/
+-rw-rw-rw-   0        0        0      860 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     3494 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py
+-rw-rw-rw-   0        0        0     4229 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.658663 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.663650 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    11773 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.691575 pm4py-2.7.5/pm4py/objects/conversion/log/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/__init__.py
+-rw-rw-rw-   0        0        0     1061 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/constants.py
+-rw-rw-rw-   0        0        0     1319 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.723489 pm4py-2.7.5/pm4py/objects/conversion/log/variants/
+-rw-rw-rw-   0        0        0      870 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     1923 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py
+-rw-rw-rw-   0        0        0     2535 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py
+-rw-rw-rw-   0        0        0     3303 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_data_frame.py
+-rw-rw-rw-   0        0        0     4382 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_event_log.py
+-rw-rw-rw-   0        0        0    10279 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_event_stream.py
+-rw-rw-rw-   0        0        0     5186 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_nx.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.733463 pm4py-2.7.5/pm4py/objects/conversion/ocel/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/ocel/__init__.py
+-rw-rw-rw-   0        0        0     1814 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/ocel/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.740444 pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     4056 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py
+-rw-rw-rw-   0        0        0     2754 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.749420 pm4py-2.7.5/pm4py/objects/conversion/process_tree/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/__init__.py
+-rw-rw-rw-   0        0        0     1824 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.769366 pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/
+-rw-rw-rw-   0        0        0      850 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0    10273 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    21550 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_petri_net.py
+-rw-rw-rw-   0        0        0     4772 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.776347 pm4py-2.7.5/pm4py/objects/conversion/wf_net/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/wf_net/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/wf_net/converter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.795297 pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     3774 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/to_bpmn.py
+-rw-rw-rw-   0        0        0    10818 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/to_process_tree.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.821228 pm4py-2.7.5/pm4py/objects/dfg/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.829207 pm4py-2.7.5/pm4py/objects/dfg/exporter/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2041 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.835192 pm4py-2.7.5/pm4py/objects/dfg/exporter/variants/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     4211 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/exporter/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.841175 pm4py-2.7.5/pm4py/objects/dfg/filtering/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/filtering/__init__.py
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/filtering/dfg_filtering.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.846161 pm4py-2.7.5/pm4py/objects/dfg/importer/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/importer/__init__.py
+-rw-rw-rw-   0        0        0     2278 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/importer/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.850150 pm4py-2.7.5/pm4py/objects/dfg/importer/variants/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/importer/variants/classic.py
+-rw-rw-rw-   0        0        0     1881 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.858129 pm4py-2.7.5/pm4py/objects/dfg/retrieval/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/retrieval/__init__.py
+-rw-rw-rw-   0        0        0      913 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/retrieval/log.py
+-rw-rw-rw-   0        0        0      873 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/retrieval/pandas.py
+-rw-rw-rw-   0        0        0     5465 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/util.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.861121 pm4py-2.7.5/pm4py/objects/dfg/utils/
+-rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/utils/__init__.py
+-rw-rw-rw-   0        0        0    26492 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/dfg/utils/dfg_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.874086 pm4py-2.7.5/pm4py/objects/heuristics_net/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/heuristics_net/__init__.py
+-rw-rw-rw-   0        0        0     1226 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/heuristics_net/defaults.py
+-rw-rw-rw-   0        0        0     2689 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/heuristics_net/edge.py
+-rw-rw-rw-   0        0        0     9877 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/heuristics_net/node.py
+-rw-rw-rw-   0        0        0     5871 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/heuristics_net/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.878077 pm4py-2.7.5/pm4py/objects/log/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.881069 pm4py-2.7.5/pm4py/objects/log/exporter/
+-rw-rw-rw-   0        0        0      778 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.887051 pm4py-2.7.5/pm4py/objects/log/exporter/xes/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/__init__.py
+-rw-rw-rw-   0        0        0     2578 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.893036 pm4py-2.7.5/pm4py/objects/log/exporter/xes/util/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/util/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/util/compression.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.900017 pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/
+-rw-rw-rw-   0        0        0      815 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0    12291 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py
+-rw-rw-rw-   0        0        0    10417 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/line_by_line.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.903009 pm4py-2.7.5/pm4py/objects/log/importer/
+-rw-rw-rw-   0        0        0      778 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.907996 pm4py-2.7.5/pm4py/objects/log/importer/xes/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     3888 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.923953 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/
+-rw-rw-rw-   0        0        0      850 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9593 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/chunk_regex.py
+-rw-rw-rw-   0        0        0    17461 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse.py
+-rw-rw-rw-   0        0        0    17730 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse_20.py
+-rw-rw-rw-   0        0        0    18029 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py
+-rw-rw-rw-   0        0        0    11435 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/line_by_line.py
+-rw-rw-rw-   0        0        0    12284 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.964845 pm4py-2.7.5/pm4py/objects/log/util/
+-rw-rw-rw-   0        0        0     1102 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/__init__.py
+-rw-rw-rw-   0        0        0     3114 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/artificial.py
+-rw-rw-rw-   0        0        0     3974 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/basic_filter.py
+-rw-rw-rw-   0        0        0    18098 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/dataframe_utils.py
+-rw-rw-rw-   0        0        0     2283 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     4898 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/get_class_representation.py
+-rw-rw-rw-   0        0        0     3195 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/get_log_encoded.py
+-rw-rw-rw-   0        0        0     8099 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/get_prefixes.py
+-rw-rw-rw-   0        0        0     1752 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/index_attribute.py
+-rw-rw-rw-   0        0        0     4067 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/insert_classifier.py
+-rw-rw-rw-   0        0        0    12644 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/interval_lifecycle.py
+-rw-rw-rw-   0        0        0     5167 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/log.py
+-rw-rw-rw-   0        0        0     4484 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/log_regex.py
+-rw-rw-rw-   0        0        0     2867 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/move_attrs_to_trace.py
+-rw-rw-rw-   0        0        0     4527 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/pandas_log_wrapper.py
+-rw-rw-rw-   0        0        0     3066 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/pandas_numpy_variants.py
+-rw-rw-rw-   0        0        0     2488 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/sampling.py
+-rw-rw-rw-   0        0        0     6049 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/sorting.py
+-rw-rw-rw-   0        0        0     2078 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/split_train_test.py
+-rw-rw-rw-   0        0        0     1695 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/log/util/xes.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.970212 pm4py-2.7.5/pm4py/objects/ocel/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.972207 pm4py-2.7.5/pm4py/objects/ocel/exporter/
+-rw-rw-rw-   0        0        0      899 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.975200 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/__init__.py
+-rw-rw-rw-   0        0        0     1695 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.977194 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/variants/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     1637 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.984176 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1550 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.987168 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.991157 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1673 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:05.999135 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     4838 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     1679 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.003124 pm4py-2.7.5/pm4py/objects/ocel/exporter/util/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/util/__init__.py
+-rw-rw-rw-   0        0        0     1671 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/util/clean_dataframes.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.007114 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.015093 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     7889 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0     9353 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.018084 pm4py-2.7.5/pm4py/objects/ocel/importer/
+-rw-rw-rw-   0        0        0      893 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.022073 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1731 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.026063 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/variants/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     1889 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/csv/variants/pandas.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.032046 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/__init__.py
+-rw-rw-rw-   0        0        0     1585 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.035038 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/variants/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     4973 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.038030 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.043017 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/__init__.py
+-rw-rw-rw-   0        0        0     7439 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py
+-rw-rw-rw-   0        0        0     1883 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.048005 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/__init__.py
+-rw-rw-rw-   0        0        0     1611 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.052990 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py
+-rw-rw-rw-   0        0        0     8499 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/classic.py
+-rw-rw-rw-   0        0        0     9295 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py
+-rw-rw-rw-   0        0        0     6466 2023-06-30 05:23:33.000000 pm4py-2.7.5/pm4py/objects/ocel/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.092477 pm4py-2.7.5/pm4py/objects/ocel/util/
+-rw-rw-rw-   0        0        0     1067 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/__init__.py
+-rw-rw-rw-   0        0        0     1690 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/attributes_names.py
+-rw-rw-rw-   0        0        0     2424 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py
+-rw-rw-rw-   0        0        0     2690 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/e2o_qualification.py
+-rw-rw-rw-   0        0        0     3668 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/ev_att_to_obj_type.py
+-rw-rw-rw-   0        0        0     4377 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py
+-rw-rw-rw-   0        0        0     2178 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/events_per_object_type.py
+-rw-rw-rw-   0        0        0     3214 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/events_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1654 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/explode.py
+-rw-rw-rw-   0        0        0     4499 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/extended_table.py
+-rw-rw-rw-   0        0        0     6047 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/filtering_utils.py
+-rw-rw-rw-   0        0        0     3117 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/flattening.py
+-rw-rw-rw-   0        0        0    16914 2023-04-25 06:11:22.000000 pm4py-2.7.5/pm4py/objects/ocel/util/log_ocel.py
+-rw-rw-rw-   0        0        0      942 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/names_stripping.py
+-rw-rw-rw-   0        0        0     3214 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/objects_per_type_per_activity.py
+-rw-rw-rw-   0        0        0     1894 2023-04-25 06:12:03.000000 pm4py-2.7.5/pm4py/objects/ocel/util/ocel_consistency.py
+-rw-rw-rw-   0        0        0     1976 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/ocel_iterator.py
+-rw-rw-rw-   0        0        0     2479 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/parent_children_ref.py
+-rw-rw-rw-   0        0        0     1297 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/related_events.py
+-rw-rw-rw-   0        0        0     1744 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/related_objects.py
+-rw-rw-rw-   0        0        0     2610 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
+-rw-rw-rw-   0        0        0     3725 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/util/sampling.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.101453 pm4py-2.7.5/pm4py/objects/ocel/validation/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/validation/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/ocel/validation/jsonocel.py
+-rw-rw-rw-   0        0        0    14786 2023-06-30 13:58:34.000000 pm4py-2.7.5/pm4py/objects/ocel/validation/ocel20_rel_validation.py
+-rw-rw-rw-   0        0        0     1200 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/objects/ocel/validation/xmlocel.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.102450 pm4py-2.7.5/pm4py/objects/org/
+-rw-rw-rw-   0        0        0      776 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/org/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.108435 pm4py-2.7.5/pm4py/objects/org/roles/
+-rw-rw-rw-   0        0        0      775 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/org/roles/__init__.py
+-rw-rw-rw-   0        0        0     1339 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/org/roles/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.113425 pm4py-2.7.5/pm4py/objects/org/sna/
+-rw-rw-rw-   0        0        0      773 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/org/sna/__init__.py
+-rw-rw-rw-   0        0        0     1029 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/org/sna/obj.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.123395 pm4py-2.7.5/pm4py/objects/petri_net/
+-rw-rw-rw-   0        0        0      828 2023-06-30 05:23:04.000000 pm4py-2.7.5/pm4py/objects/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.129379 pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/__init__.py
+-rw-rw-rw-   0        0        0     1287 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/data_marking.py
+-rw-rw-rw-   0        0        0     6212 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/semantics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.134367 pm4py-2.7.5/pm4py/objects/petri_net/exporter/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/exporter/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.137357 pm4py-2.7.5/pm4py/objects/petri_net/exporter/variants/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0    12697 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/exporter/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.143343 pm4py-2.7.5/pm4py/objects/petri_net/importer/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/importer/__init__.py
+-rw-rw-rw-   0        0        0     1910 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/importer/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.147331 pm4py-2.7.5/pm4py/objects/petri_net/importer/variants/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0    14894 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/importer/variants/pnml.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.150323 pm4py-2.7.5/pm4py/objects/petri_net/inhibitor_reset/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/inhibitor_reset/__init__.py
+-rw-rw-rw-   0        0        0     4665 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/inhibitor_reset/semantics.py
+-rw-rw-rw-   0        0        0    13270 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/obj.py
+-rw-rw-rw-   0        0        0     1225 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/properties.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.159299 pm4py-2.7.5/pm4py/objects/petri_net/saw_net/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/saw_net/__init__.py
+-rw-rw-rw-   0        0        0     4805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/saw_net/convert.py
+-rw-rw-rw-   0        0        0     1546 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/saw_net/obj.py
+-rw-rw-rw-   0        0        0    10807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/saw_net/semantics.py
+-rw-rw-rw-   0        0        0     1503 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/sem_interface.py
+-rw-rw-rw-   0        0        0     5339 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/semantics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.165284 pm4py-2.7.5/pm4py/objects/petri_net/stochastic/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/stochastic/__init__.py
+-rw-rw-rw-   0        0        0     1448 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/stochastic/obj.py
+-rw-rw-rw-   0        0        0     2619 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/stochastic/semantics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.203070 pm4py-2.7.5/pm4py/objects/petri_net/utils/
+-rw-rw-rw-   0        0        0     1035 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/__init__.py
+-rw-rw-rw-   0        0        0    18755 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/align_utils.py
+-rw-rw-rw-   0        0        0     5923 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/check_soundness.py
+-rw-rw-rw-   0        0        0     4014 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/consumption_matrix.py
+-rw-rw-rw-   0        0        0     6609 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/decomposition.py
+-rw-rw-rw-   0        0        0     1672 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/embed_stochastic_map.py
+-rw-rw-rw-   0        0        0     5751 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/explore_path.py
+-rw-rw-rw-   0        0        0     1195 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/final_marking.py
+-rw-rw-rw-   0        0        0     2272 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/incidence_matrix.py
+-rw-rw-rw-   0        0        0     1227 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/initial_marking.py
+-rw-rw-rw-   0        0        0     4243 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/murata.py
+-rw-rw-rw-   0        0        0     4281 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/networkx_graph.py
+-rw-rw-rw-   0        0        0     4124 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/obj_marking.py
+-rw-rw-rw-   0        0        0    23057 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/performance_map.py
+-rw-rw-rw-   0        0        0    20532 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/petri_utils.py
+-rw-rw-rw-   0        0        0     4602 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/projection.py
+-rw-rw-rw-   0        0        0     5570 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/reachability_graph.py
+-rw-rw-rw-   0        0        0    14266 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/reduction.py
+-rw-rw-rw-   0        0        0     7288 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/petri_net/utils/synchronous_product.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.211048 pm4py-2.7.5/pm4py/objects/process_tree/
+-rw-rw-rw-   0        0        0      917 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.215039 pm4py-2.7.5/pm4py/objects/process_tree/exporter/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/exporter/__init__.py
+-rw-rw-rw-   0        0        0     1888 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/exporter/exporter.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.221022 pm4py-2.7.5/pm4py/objects/process_tree/exporter/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/exporter/variants/__init__.py
+-rw-rw-rw-   0        0        0     5527 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/exporter/variants/ptml.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.226009 pm4py-2.7.5/pm4py/objects/process_tree/importer/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/importer/__init__.py
+-rw-rw-rw-   0        0        0     2048 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/importer/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.229998 pm4py-2.7.5/pm4py/objects/process_tree/importer/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/importer/variants/__init__.py
+-rw-rw-rw-   0        0        0     5214 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/importer/variants/ptml.py
+-rw-rw-rw-   0        0        0     7135 2023-06-30 05:23:04.000000 pm4py-2.7.5/pm4py/objects/process_tree/obj.py
+-rw-rw-rw-   0        0        0     8883 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/semantics.py
+-rw-rw-rw-   0        0        0      887 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/state.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.239971 pm4py-2.7.5/pm4py/objects/process_tree/utils/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/utils/__init__.py
+-rw-rw-rw-   0        0        0     7128 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/utils/bottomup.py
+-rw-rw-rw-   0        0        0    15797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/utils/generic.py
+-rw-rw-rw-   0        0        0     3362 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/process_tree/utils/regex.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.245956 pm4py-2.7.5/pm4py/objects/random_variables/
+-rw-rw-rw-   0        0        0      958 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/__init__.py
+-rw-rw-rw-   0        0        0     3878 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/basic_structure.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.250942 pm4py-2.7.5/pm4py/objects/random_variables/constant0/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/constant0/__init__.py
+-rw-rw-rw-   0        0        0     3586 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/constant0/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.256926 pm4py-2.7.5/pm4py/objects/random_variables/exponential/
+-rw-rw-rw-   0        0        0      818 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/exponential/__init__.py
+-rw-rw-rw-   0        0        0     3684 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/exponential/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.260916 pm4py-2.7.5/pm4py/objects/random_variables/gamma/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/gamma/__init__.py
+-rw-rw-rw-   0        0        0     3749 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/gamma/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.267900 pm4py-2.7.5/pm4py/objects/random_variables/lognormal/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/lognormal/__init__.py
+-rw-rw-rw-   0        0        0     3568 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/lognormal/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.279882 pm4py-2.7.5/pm4py/objects/random_variables/normal/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/normal/__init__.py
+-rw-rw-rw-   0        0        0     3594 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/normal/random_variable.py
+-rw-rw-rw-   0        0        0     9224 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.285849 pm4py-2.7.5/pm4py/objects/random_variables/uniform/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/uniform/__init__.py
+-rw-rw-rw-   0        0        0     3588 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/random_variables/uniform/random_variable.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.293828 pm4py-2.7.5/pm4py/objects/stochastic_petri/
+-rw-rw-rw-   0        0        0      912 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/stochastic_petri/__init__.py
+-rw-rw-rw-   0        0        0    12887 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/stochastic_petri/ctmc.py
+-rw-rw-rw-   0        0        0     4714 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/stochastic_petri/tangible_reachability.py
+-rw-rw-rw-   0        0        0     1616 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/stochastic_petri/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.303812 pm4py-2.7.5/pm4py/objects/transition_system/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/transition_system/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/transition_system/constants.py
+-rw-rw-rw-   0        0        0     3958 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/transition_system/obj.py
+-rw-rw-rw-   0        0        0     3625 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/transition_system/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.308787 pm4py-2.7.5/pm4py/objects/trie/
+-rw-rw-rw-   0        0        0      770 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/trie/__init__.py
+-rw-rw-rw-   0        0        0     1911 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/objects/trie/obj.py
+-rw-rw-rw-   0        0        0    21530 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/ocel.py
+-rw-rw-rw-   0        0        0    15446 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/org.py
+-rw-rw-rw-   0        0        0     3805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/privacy.py
+-rw-rw-rw-   0        0        0    12248 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/read.py
+-rw-rw-rw-   0        0        0     3789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/sim.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.310782 pm4py-2.7.5/pm4py/statistics/
+-rw-rw-rw-   0        0        0      899 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.314772 pm4py-2.7.5/pm4py/statistics/attributes/
+-rw-rw-rw-   0        0        0      894 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.319759 pm4py-2.7.5/pm4py/statistics/attributes/common/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/common/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/common/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.325742 pm4py-2.7.5/pm4py/statistics/attributes/log/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/log/__init__.py
+-rw-rw-rw-   0        0        0    13308 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/log/get.py
+-rw-rw-rw-   0        0        0     6933 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/log/select.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.334718 pm4py-2.7.5/pm4py/statistics/attributes/pandas/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/pandas/__init__.py
+-rw-rw-rw-   0        0        0     9789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/attributes/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.337710 pm4py-2.7.5/pm4py/statistics/concurrent_activities/
+-rw-rw-rw-   0        0        0      906 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/concurrent_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.341700 pm4py-2.7.5/pm4py/statistics/concurrent_activities/log/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/concurrent_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     4092 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/concurrent_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.349678 pm4py-2.7.5/pm4py/statistics/concurrent_activities/pandas/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/concurrent_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3697 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/concurrent_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.351673 pm4py-2.7.5/pm4py/statistics/end_activities/
+-rw-rw-rw-   0        0        0      902 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.355662 pm4py-2.7.5/pm4py/statistics/end_activities/common/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.367630 pm4py-2.7.5/pm4py/statistics/end_activities/log/
+-rw-rw-rw-   0        0        0      787 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2764 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.371619 pm4py-2.7.5/pm4py/statistics/end_activities/pandas/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2636 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/end_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.374612 pm4py-2.7.5/pm4py/statistics/eventually_follows/
+-rw-rw-rw-   0        0        0      900 2023-06-30 05:23:04.000000 pm4py-2.7.5/pm4py/statistics/eventually_follows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.379598 pm4py-2.7.5/pm4py/statistics/eventually_follows/log/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/eventually_follows/log/__init__.py
+-rw-rw-rw-   0        0        0     3026 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/eventually_follows/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.384585 pm4py-2.7.5/pm4py/statistics/eventually_follows/pandas/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/eventually_follows/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2890 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/eventually_follows/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.398547 pm4py-2.7.5/pm4py/statistics/ocel/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/__init__.py
+-rw-rw-rw-   0        0        0     3744 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/act_ot_dependent.py
+-rw-rw-rw-   0        0        0     5677 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/act_utils.py
+-rw-rw-rw-   0        0        0     9399 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/edge_metrics.py
+-rw-rw-rw-   0        0        0     2387 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/objects_ot_count.py
+-rw-rw-rw-   0        0        0     2395 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/ocel/ot_activities.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.401539 pm4py-2.7.5/pm4py/statistics/overlap/
+-rw-rw-rw-   0        0        0      881 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.403534 pm4py-2.7.5/pm4py/statistics/overlap/cases/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.408523 pm4py-2.7.5/pm4py/statistics/overlap/cases/log/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2713 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.419493 pm4py-2.7.5/pm4py/statistics/overlap/cases/pandas/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.423480 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.442430 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/log/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/log/__init__.py
+-rw-rw-rw-   0        0        0     2767 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.450408 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/pandas/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2570 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/interval_events/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.461382 pm4py-2.7.5/pm4py/statistics/overlap/utils/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/utils/__init__.py
+-rw-rw-rw-   0        0        0     1986 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/overlap/utils/compute.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.463638 pm4py-2.7.5/pm4py/statistics/passed_time/
+-rw-rw-rw-   0        0        0      888 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.468361 pm4py-2.7.5/pm4py/statistics/passed_time/log/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/__init__.py
+-rw-rw-rw-   0        0        0     1806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.478334 pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/
+-rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/__init__.py
+-rw-rw-rw-   0        0        0     2412 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/post.py
+-rw-rw-rw-   0        0        0     2394 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/pre.py
+-rw-rw-rw-   0        0        0     3075 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.483321 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     1793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.494291 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/
+-rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/__init__.py
+-rw-rw-rw-   0        0        0     4156 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/post.py
+-rw-rw-rw-   0        0        0     4260 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/pre.py
+-rw-rw-rw-   0        0        0     5079 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/prepost.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.497284 pm4py-2.7.5/pm4py/statistics/rework/
+-rw-rw-rw-   0        0        0      783 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.499278 pm4py-2.7.5/pm4py/statistics/rework/cases/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/cases/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.504265 pm4py-2.7.5/pm4py/statistics/rework/cases/log/
+-rw-rw-rw-   0        0        0      785 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/cases/log/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/cases/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.509253 pm4py-2.7.5/pm4py/statistics/rework/cases/pandas/
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/cases/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/cases/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.515235 pm4py-2.7.5/pm4py/statistics/rework/log/
+-rw-rw-rw-   0        0        0      779 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/log/__init__.py
+-rw-rw-rw-   0        0        0     2265 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.521220 pm4py-2.7.5/pm4py/statistics/rework/pandas/
+-rw-rw-rw-   0        0        0      782 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/rework/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.524211 pm4py-2.7.5/pm4py/statistics/sojourn_time/
+-rw-rw-rw-   0        0        0      888 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/sojourn_time/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.531193 pm4py-2.7.5/pm4py/statistics/sojourn_time/log/
+-rw-rw-rw-   0        0        0      785 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/sojourn_time/log/__init__.py
+-rw-rw-rw-   0        0        0     5495 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/sojourn_time/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.536180 pm4py-2.7.5/pm4py/statistics/sojourn_time/pandas/
+-rw-rw-rw-   0        0        0      788 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/sojourn_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4929 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/sojourn_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.538174 pm4py-2.7.5/pm4py/statistics/start_activities/
+-rw-rw-rw-   0        0        0      904 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.545155 pm4py-2.7.5/pm4py/statistics/start_activities/common/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/common/__init__.py
+-rw-rw-rw-   0        0        0     1813 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/common/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.552137 pm4py-2.7.5/pm4py/statistics/start_activities/log/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/log/__init__.py
+-rw-rw-rw-   0        0        0     2787 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.557124 pm4py-2.7.5/pm4py/statistics/start_activities/pandas/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2594 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/start_activities/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.560114 pm4py-2.7.5/pm4py/statistics/traces/
+-rw-rw-rw-   0        0        0      791 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.564105 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.570088 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/log/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/log/__init__.py
+-rw-rw-rw-   0        0        0     3191 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.574078 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/pandas/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/pandas/__init__.py
+-rw-rw-rw-   0        0        0     3255 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/pandas/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.577677 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/util/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/util/__init__.py
+-rw-rw-rw-   0        0        0     2385 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/cycle_time/util/compute.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.580669 pm4py-2.7.5/pm4py/statistics/traces/generic/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.585655 pm4py-2.7.5/pm4py/statistics/traces/generic/common/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/common/__init__.py
+-rw-rw-rw-   0        0        0     2950 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/common/case_duration.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.592637 pm4py-2.7.5/pm4py/statistics/traces/generic/log/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/log/__init__.py
+-rw-rw-rw-   0        0        0     5339 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/log/case_arrival.py
+-rw-rw-rw-   0        0        0    13275 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/log/case_statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.601611 pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/__init__.py
+-rw-rw-rw-   0        0        0     4213 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/case_arrival.py
+-rw-rw-rw-   0        0        0    16506 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/case_statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.606666 pm4py-2.7.5/pm4py/statistics/util/
+-rw-rw-rw-   0        0        0      898 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/util/__init__.py
+-rw-rw-rw-   0        0        0     2370 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/util/times_bipartite_matching.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.607668 pm4py-2.7.5/pm4py/statistics/variants/
+-rw-rw-rw-   0        0        0      880 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.611656 pm4py-2.7.5/pm4py/statistics/variants/log/
+-rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/variants/log/__init__.py
+-rw-rw-rw-   0        0        0     7359 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/variants/log/get.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.664515 pm4py-2.7.5/pm4py/statistics/variants/pandas/
+-rw-rw-rw-   0        0        0      784 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/variants/pandas/__init__.py
+-rw-rw-rw-   0        0        0     2197 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/statistics/variants/pandas/get.py
+-rw-rw-rw-   0        0        0    30520 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.673491 pm4py-2.7.5/pm4py/streaming/
+-rw-rw-rw-   0        0        0      804 2023-04-05 11:57:19.000000 pm4py-2.7.5/pm4py/streaming/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.698424 pm4py-2.7.5/pm4py/streaming/algo/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.720366 pm4py-2.7.5/pm4py/streaming/algo/conformance/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.780207 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/
+-rw-rw-rw-   0        0        0      811 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/__init__.py
+-rw-rw-rw-   0        0        0     1515 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.791176 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/variants/
+-rw-rw-rw-   0        0        0      808 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0    10995 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.800153 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/__init__.py
+-rw-rw-rw-   0        0        0     1523 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.808131 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/variants/__init__.py
+-rw-rw-rw-   0        0        0    17212 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.820099 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.825086 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/variants/
+-rw-rw-rw-   0        0        0      806 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/variants/__init__.py
+-rw-rw-rw-   0        0        0     9602 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/variants/classic.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.827080 pm4py-2.7.5/pm4py/streaming/algo/discovery/
+-rw-rw-rw-   0        0        0      782 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.835059 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/algorithm.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.839049 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/variants/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     7399 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     1503 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/algo/interface.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.847027 pm4py-2.7.5/pm4py/streaming/conversion/
+-rw-rw-rw-   0        0        0     1468 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4925 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/conversion/from_pandas.py
+-rw-rw-rw-   0        0        0     5211 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/conversion/ocel_flatts_distributor.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.849022 pm4py-2.7.5/pm4py/streaming/importer/
+-rw-rw-rw-   0        0        0      875 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.854009 pm4py-2.7.5/pm4py/streaming/importer/csv/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/csv/__init__.py
+-rw-rw-rw-   0        0        0     1488 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/csv/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.858006 pm4py-2.7.5/pm4py/streaming/importer/csv/variants/
+-rw-rw-rw-   0        0        0      802 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/csv/variants/__init__.py
+-rw-rw-rw-   0        0        0     3406 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/csv/variants/csv_event_stream.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.867972 pm4py-2.7.5/pm4py/streaming/importer/xes/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/xes/__init__.py
+-rw-rw-rw-   0        0        0     1523 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/xes/importer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.881934 pm4py-2.7.5/pm4py/streaming/importer/xes/variants/
+-rw-rw-rw-   0        0        0      820 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/xes/variants/__init__.py
+-rw-rw-rw-   0        0        0     9461 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/xes/variants/xes_event_stream.py
+-rw-rw-rw-   0        0        0     9317 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/importer/xes/variants/xes_trace_stream.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.888915 pm4py-2.7.5/pm4py/streaming/stream/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/stream/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/stream/live_event_stream.py
+-rw-rw-rw-   0        0        0     3109 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/stream/live_trace_stream.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.896894 pm4py-2.7.5/pm4py/streaming/util/
+-rw-rw-rw-   0        0        0      819 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.902877 pm4py-2.7.5/pm4py/streaming/util/dictio/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/__init__.py
+-rw-rw-rw-   0        0        0     1461 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/generator.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.917837 pm4py-2.7.5/pm4py/streaming/util/dictio/versions/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/versions/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/versions/classic.py
+-rw-rw-rw-   0        0        0     3540 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/versions/redis.py
+-rw-rw-rw-   0        0        0     1949 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/dictio/versions/thread_safe.py
+-rw-rw-rw-   0        0        0     1039 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/event_stream_printer.py
+-rw-rw-rw-   0        0        0     1039 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/streaming/util/trace_stream_printer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.952744 pm4py-2.7.5/pm4py/util/
+-rw-rw-rw-   0        0        0      918 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/__init__.py
+-rw-rw-rw-   0        0        0     5000 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/business_hours.py
+-rw-rw-rw-   0        0        0     2225 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/colors.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.962718 pm4py-2.7.5/pm4py/util/compression/
+-rw-rw-rw-   0        0        0      781 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/compression/__init__.py
+-rw-rw-rw-   0        0        0     1314 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/compression/dtypes.py
+-rw-rw-rw-   0        0        0    12024 2023-06-30 05:23:04.000000 pm4py-2.7.5/pm4py/util/compression/util.py
+-rw-rw-rw-   0        0        0     4854 2023-05-08 08:05:18.000000 pm4py-2.7.5/pm4py/util/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.967705 pm4py-2.7.5/pm4py/util/dt_parsing/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/__init__.py
+-rw-rw-rw-   0        0        0     2608 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/parser.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.977678 pm4py-2.7.5/pm4py/util/dt_parsing/variants/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/variants/__init__.py
+-rw-rw-rw-   0        0        0     1029 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/variants/cs8601.py
+-rw-rw-rw-   0        0        0     1470 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/variants/dummy.py
+-rw-rw-rw-   0        0        0     1294 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/dt_parsing/variants/strpfromiso.py
+-rw-rw-rw-   0        0        0     1564 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/exec_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.985657 pm4py-2.7.5/pm4py/util/lp/
+-rw-rw-rw-   0        0        0      784 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/__init__.py
+-rw-rw-rw-   0        0        0     5359 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/solver.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:06.994632 pm4py-2.7.5/pm4py/util/lp/util/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.017572 pm4py-2.7.5/pm4py/util/lp/variants/
+-rw-rw-rw-   0        0        0      926 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/__init__.py
+-rw-rw-rw-   0        0        0     3639 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver.py
+-rw-rw-rw-   0        0        0     3420 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align.py
+-rw-rw-rw-   0        0        0     3059 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py
+-rw-rw-rw-   0        0        0     3937 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py
+-rw-rw-rw-   0        0        0     5153 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/ortools_solver.py
+-rw-rw-rw-   0        0        0     6101 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/pulp_solver.py
+-rw-rw-rw-   0        0        0     1876 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/lp/variants/scipy_solver.py
+-rw-rw-rw-   0        0        0    11130 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/pandas_utils.py
+-rw-rw-rw-   0        0        0     1494 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/points_subset.py
+-rw-rw-rw-   0        0        0     1712 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/regex.py
+-rw-rw-rw-   0        0        0     3663 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/string_distance.py
+-rw-rw-rw-   0        0        0     1095 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/typing.py
+-rw-rw-rw-   0        0        0     2261 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/variants_util.py
+-rw-rw-rw-   0        0        0     5861 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/vis_utils.py
+-rw-rw-rw-   0        0        0     1614 2023-03-27 13:12:17.000000 pm4py-2.7.5/pm4py/util/xes_constants.py
+-rw-rw-rw-   0        0        0    24096 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/utils.py
+-rw-rw-rw-   0        0        0    65781 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/vis.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.020562 pm4py-2.7.5/pm4py/visualization/
+-rw-rw-rw-   0        0        0     1837 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.024552 pm4py-2.7.5/pm4py/visualization/align_table/
+-rw-rw-rw-   0        0        0      790 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/align_table/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.028542 pm4py-2.7.5/pm4py/visualization/align_table/variants/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/align_table/variants/__init__.py
+-rw-rw-rw-   0        0        0     3868 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/visualization/align_table/variants/classic.py
+-rw-rw-rw-   0        0        0     2973 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/align_table/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.032531 pm4py-2.7.5/pm4py/visualization/bpmn/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/bpmn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.037517 pm4py-2.7.5/pm4py/visualization/bpmn/variants/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/bpmn/variants/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/bpmn/variants/classic.py
+-rw-rw-rw-   0        0        0     2613 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/bpmn/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.051516 pm4py-2.7.5/pm4py/visualization/common/
+-rw-rw-rw-   0        0        0      817 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/common/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/common/dot_util.py
+-rw-rw-rw-   0        0        0     3058 2023-05-08 08:05:18.000000 pm4py-2.7.5/pm4py/visualization/common/gview.py
+-rw-rw-rw-   0        0        0     3394 2023-05-08 08:10:31.000000 pm4py-2.7.5/pm4py/visualization/common/html.py
+-rw-rw-rw-   0        0        0     1531 2023-05-08 08:05:18.000000 pm4py-2.7.5/pm4py/visualization/common/save.py
+-rw-rw-rw-   0        0        0     2526 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/common/svg_pos_parser.py
+-rw-rw-rw-   0        0        0      879 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/common/utils.py
+-rw-rw-rw-   0        0        0     1540 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/common/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.056515 pm4py-2.7.5/pm4py/visualization/decisiontree/
+-rw-rw-rw-   0        0        0      932 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.059510 pm4py-2.7.5/pm4py/visualization/decisiontree/util/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/util/__init__.py
+-rw-rw-rw-   0        0        0     2621 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/util/dt_to_string.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.063682 pm4py-2.7.5/pm4py/visualization/decisiontree/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/variants/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/variants/classic.py
+-rw-rw-rw-   0        0        0     2854 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/decisiontree/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.066677 pm4py-2.7.5/pm4py/visualization/dfg/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.071874 pm4py-2.7.5/pm4py/visualization/dfg/util/
+-rw-rw-rw-   0        0        0      787 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/util/__init__.py
+-rw-rw-rw-   0        0        0     8588 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/visualization/dfg/util/dfg_gviz.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.078052 pm4py-2.7.5/pm4py/visualization/dfg/variants/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/variants/__init__.py
+-rw-rw-rw-   0        0        0     5223 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/variants/cost.py
+-rw-rw-rw-   0        0        0     4974 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/visualization/dfg/variants/frequency.py
+-rw-rw-rw-   0        0        0     5374 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/variants/performance.py
+-rw-rw-rw-   0        0        0     3272 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.081444 pm4py-2.7.5/pm4py/visualization/dotted_chart/
+-rw-rw-rw-   0        0        0      801 2023-06-30 05:23:33.000000 pm4py-2.7.5/pm4py/visualization/dotted_chart/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.085433 pm4py-2.7.5/pm4py/visualization/dotted_chart/variants/
+-rw-rw-rw-   0        0        0      797 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/dotted_chart/variants/__init__.py
+-rw-rw-rw-   0        0        0     9236 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/visualization/dotted_chart/variants/classic.py
+-rw-rw-rw-   0        0        0     3776 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/visualization/dotted_chart/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.089423 pm4py-2.7.5/pm4py/visualization/footprints/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.097401 pm4py-2.7.5/pm4py/visualization/footprints/variants/
+-rw-rw-rw-   0        0        0      828 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/variants/__init__.py
+-rw-rw-rw-   0        0        0     3827 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/variants/comparison.py
+-rw-rw-rw-   0        0        0     4359 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/variants/comparison_symmetric.py
+-rw-rw-rw-   0        0        0     3265 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/variants/single.py
+-rw-rw-rw-   0        0        0     3119 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/footprints/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.101390 pm4py-2.7.5/pm4py/visualization/graphs/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.105379 pm4py-2.7.5/pm4py/visualization/graphs/util/
+-rw-rw-rw-   0        0        0      786 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/util/__init__.py
+-rw-rw-rw-   0        0        0     2791 2023-04-05 11:57:19.000000 pm4py-2.7.5/pm4py/visualization/graphs/util/common.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.115352 pm4py-2.7.5/pm4py/visualization/graphs/variants/
+-rw-rw-rw-   0        0        0      817 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/variants/__init__.py
+-rw-rw-rw-   0        0        0     4548 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/variants/attributes.py
+-rw-rw-rw-   0        0        0     2770 2023-04-03 08:54:35.000000 pm4py-2.7.5/pm4py/visualization/graphs/variants/barplot.py
+-rw-rw-rw-   0        0        0     4549 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/variants/cases.py
+-rw-rw-rw-   0        0        0     4594 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/variants/dates.py
+-rw-rw-rw-   0        0        0     3873 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/graphs/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.120340 pm4py-2.7.5/pm4py/visualization/heuristics_net/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/heuristics_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.124328 pm4py-2.7.5/pm4py/visualization/heuristics_net/variants/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/heuristics_net/variants/__init__.py
+-rw-rw-rw-   0        0        0    13364 2023-06-30 13:57:45.000000 pm4py-2.7.5/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py
+-rw-rw-rw-   0        0        0     4470 2023-04-05 11:57:19.000000 pm4py-2.7.5/pm4py/visualization/heuristics_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.128318 pm4py-2.7.5/pm4py/visualization/network_analysis/
+-rw-rw-rw-   0        0        0      805 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/network_analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.135299 pm4py-2.7.5/pm4py/visualization/network_analysis/variants/
+-rw-rw-rw-   0        0        0      816 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/network_analysis/variants/__init__.py
+-rw-rw-rw-   0        0        0     4951 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/network_analysis/variants/frequency.py
+-rw-rw-rw-   0        0        0     6130 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/network_analysis/variants/performance.py
+-rw-rw-rw-   0        0        0     2481 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/network_analysis/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.137294 pm4py-2.7.5/pm4py/visualization/ocel/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.141284 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/
+-rw-rw-rw-   0        0        0      807 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.146270 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/variants/
+-rw-rw-rw-   0        0        0      804 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/variants/__init__.py
+-rw-rw-rw-   0        0        0    14981 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2989 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/interleavings/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.152255 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.157240 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/variants/
+-rw-rw-rw-   0        0        0      734 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/variants/__init__.py
+-rw-rw-rw-   0        0        0     3388 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/variants/graphviz.py
+-rw-rw-rw-   0        0        0     2541 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/object_graph/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.161229 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/
+-rw-rw-rw-   0        0        0      799 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.167215 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/variants/
+-rw-rw-rw-   0        0        0      795 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/variants/__init__.py
+-rw-rw-rw-   0        0        0    12244 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/variants/classic.py
+-rw-rw-rw-   0        0        0     2439 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.175194 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/
+-rw-rw-rw-   0        0        0      798 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.185165 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/variants/
+-rw-rw-rw-   0        0        0      800 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/variants/__init__.py
+-rw-rw-rw-   0        0        0     5000 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     2586 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/ocel/ocpn/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.190154 pm4py-2.7.5/pm4py/visualization/performance_spectrum/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/performance_spectrum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.196139 pm4py-2.7.5/pm4py/visualization/performance_spectrum/variants/
+-rw-rw-rw-   0        0        0      803 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/performance_spectrum/variants/__init__.py
+-rw-rw-rw-   0        0        0     7035 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/performance_spectrum/variants/neato.py
+-rw-rw-rw-   0        0        0     3229 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/visualization/performance_spectrum/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.201124 pm4py-2.7.5/pm4py/visualization/petri_net/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.206109 pm4py-2.7.5/pm4py/visualization/petri_net/common/
+-rw-rw-rw-   0        0        0      794 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/common/__init__.py
+-rw-rw-rw-   0        0        0     9490 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/common/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.218078 pm4py-2.7.5/pm4py/visualization/petri_net/util/
+-rw-rw-rw-   0        0        0      847 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/util/__init__.py
+-rw-rw-rw-   0        0        0     2935 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/util/alignments_decoration.py
+-rw-rw-rw-   0        0        0     1121 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/util/performance_map.py
+-rw-rw-rw-   0        0        0    11279 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.237027 pm4py-2.7.5/pm4py/visualization/petri_net/variants/
+-rw-rw-rw-   0        0        0      937 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/alignments.py
+-rw-rw-rw-   0        0        0     4750 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py
+-rw-rw-rw-   0        0        0     4857 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py
+-rw-rw-rw-   0        0        0     5690 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/token_decoration_frequency.py
+-rw-rw-rw-   0        0        0     5900 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/token_decoration_performance.py
+-rw-rw-rw-   0        0        0     2257 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     3807 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/petri_net/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.242013 pm4py-2.7.5/pm4py/visualization/process_tree/
+-rw-rw-rw-   0        0        0      801 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.251987 pm4py-2.7.5/pm4py/visualization/process_tree/variants/
+-rw-rw-rw-   0        0        0      813 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/variants/__init__.py
+-rw-rw-rw-   0        0        0     4713 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/variants/frequency_annotation.py
+-rw-rw-rw-   0        0        0     3951 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/variants/symbolic.py
+-rw-rw-rw-   0        0        0     4083 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/variants/wo_decoration.py
+-rw-rw-rw-   0        0        0     2813 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/process_tree/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.255977 pm4py-2.7.5/pm4py/visualization/sna/
+-rw-rw-rw-   0        0        0      792 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/sna/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.265949 pm4py-2.7.5/pm4py/visualization/sna/variants/
+-rw-rw-rw-   0        0        0      796 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/sna/variants/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-04-05 11:57:19.000000 pm4py-2.7.5/pm4py/visualization/sna/variants/networkx.py
+-rw-rw-rw-   0        0        0     5429 2023-04-24 10:28:37.000000 pm4py-2.7.5/pm4py/visualization/sna/variants/pyvis.py
+-rw-rw-rw-   0        0        0     2561 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/sna/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.269940 pm4py-2.7.5/pm4py/visualization/transition_system/
+-rw-rw-rw-   0        0        0      812 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.274925 pm4py-2.7.5/pm4py/visualization/transition_system/util/
+-rw-rw-rw-   0        0        0      809 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/util/__init__.py
+-rw-rw-rw-   0        0        0     3291 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/util/visualize_graphviz.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.284899 pm4py-2.7.5/pm4py/visualization/transition_system/variants/
+-rw-rw-rw-   0        0        0      822 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/variants/__init__.py
+-rw-rw-rw-   0        0        0     3114 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/variants/trans_frequency.py
+-rw-rw-rw-   0        0        0     1659 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/variants/view_based.py
+-rw-rw-rw-   0        0        0     2702 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/transition_system/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.291880 pm4py-2.7.5/pm4py/visualization/trie/
+-rw-rw-rw-   0        0        0      793 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/trie/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.298862 pm4py-2.7.5/pm4py/visualization/trie/variants/
+-rw-rw-rw-   0        0        0      789 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/trie/variants/__init__.py
+-rw-rw-rw-   0        0        0     2737 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/trie/variants/classic.py
+-rw-rw-rw-   0        0        0     2497 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/visualization/trie/visualizer.py
+-rw-rw-rw-   0        0        0    12749 2023-03-27 13:12:18.000000 pm4py-2.7.5/pm4py/write.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:03.882458 pm4py-2.7.5/pm4py.egg-info/
+-rw-rw-rw-   0        0        0     2683 2023-06-30 14:33:02.000000 pm4py-2.7.5/pm4py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    60828 2023-06-30 14:33:03.000000 pm4py-2.7.5/pm4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-30 14:33:02.000000 pm4py-2.7.5/pm4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-06-30 14:33:02.000000 pm4py-2.7.5/pm4py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-30 14:33:02.000000 pm4py-2.7.5/pm4py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-30 14:33:07.308836 pm4py-2.7.5/setup.cfg
+-rw-rw-rw-   0        0        0    22618 2023-06-30 13:57:45.000000 pm4py-2.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-30 14:33:07.301854 pm4py-2.7.5/tests/
+-rw-rw-rw-   0        0        0     4971 2023-03-27 13:12:18.000000 pm4py-2.7.5/tests/test_cli.py
```

### Comparing `pm4py-2.7.4/LICENSE` & `pm4py-2.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/PKG-INFO` & `pm4py-2.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm4py
-Version: 2.7.4
+Version: 2.7.5
 Summary: Process mining for Python
 Home-page: http://www.pm4py.org
 Author: Fraunhofer Institute for Applied Technology
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, http://www.pm4py.org
 Project-URL: Source, https://github.com/pm4py/pm4py-source
```

### Comparing `pm4py-2.7.4/README.md` & `pm4py-2.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/__init__.py` & `pm4py-2.7.5/pm4py/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 import time
 
-from pm4py import util, objects, statistics, algo, visualization, openai, connectors
+from pm4py import util, objects, statistics, algo, visualization, llm, connectors
 from pm4py import analysis, conformance, convert, discovery, filtering, hof, ml, ocel, org, read, sim, stats, utils, vis, write
 from pm4py.read import read_xes, read_dfg, read_bpmn, read_pnml, read_ptml, read_ocel, read_ocel_csv, read_ocel_xml, read_ocel_json, read_ocel_sqlite, read_ocel2, read_ocel2_sqlite, read_ocel2_xml
 from pm4py.write import write_xes, write_dfg, write_bpmn, write_pnml, write_ptml, write_ocel, write_ocel_json, write_ocel_csv, write_ocel_xml, write_ocel_sqlite, write_ocel2, write_ocel2_sqlite, write_ocel2_xml
 from pm4py.utils import format_dataframe, parse_process_tree, serialize, deserialize, set_classifier, parse_event_log_string, project_on_event_attribute, \
     sample_cases, sample_events, rebase
 from pm4py.filtering import filter_log_relative_occurrence_event_attribute, filter_start_activities, filter_end_activities, filter_variants, \
     filter_directly_follows_relation, filter_time_range, \
@@ -37,15 +37,15 @@
     discover_performance_dfg, discover_transition_system, discover_prefix_tree, \
     discover_temporal_profile, discover_log_skeleton, discover_batches, derive_minimum_self_distance, discover_dfg_typed
 from pm4py.conformance import conformance_diagnostics_token_based_replay, conformance_diagnostics_alignments, \
     fitness_token_based_replay, \
     fitness_alignments, precision_token_based_replay, \
     precision_alignments, conformance_diagnostics_footprints, \
     fitness_footprints, precision_footprints, check_is_fitting, conformance_temporal_profile, \
-    conformance_log_skeleton
+    conformance_log_skeleton, replay_prefix_tbr
 from pm4py.ocel import ocel_objects_interactions_summary, ocel_temporal_summary, ocel_objects_summary, ocel_get_object_types, ocel_get_attribute_names, ocel_flattening, ocel_object_type_activities, ocel_objects_ot_count, \
                         discover_ocdfg, discover_oc_petri_net, discover_objects_graph, sample_ocel_objects, ocel_drop_duplicates, ocel_merge_duplicates, ocel_sort_by_additional_column, \
                         ocel_add_index_based_timedelta, sample_ocel_connected_components, ocel_o2o_enrichment, ocel_e2o_lifecycle_enrichment, cluster_equivalent_ocel
 from pm4py.vis import view_petri_net, save_vis_petri_net, view_dfg, save_vis_dfg, view_process_tree, \
     save_vis_process_tree, \
     view_ocdfg, save_vis_ocdfg, view_heuristics_net, save_vis_heuristics_net, view_bpmn, save_vis_bpmn, view_sna, save_vis_sna,\
     view_dotted_chart, save_vis_dotted_chart, view_performance_spectrum, save_vis_performance_spectrum, view_case_duration_graph, view_events_per_time_graph, save_vis_case_duration_graph, \
@@ -54,15 +54,15 @@
     view_prefix_tree, save_vis_prefix_tree, view_object_graph, save_vis_object_graph, view_alignments, save_vis_alignments, \
     view_footprints, save_vis_footprints
 from pm4py.convert import convert_to_event_log, convert_to_event_stream, convert_to_dataframe, convert_to_bpmn, \
     convert_to_petri_net, convert_to_process_tree, convert_to_reachability_graph, convert_log_to_ocel, convert_ocel_to_networkx, convert_log_to_networkx, \
     convert_petri_net_to_networkx, convert_petri_net_type
 from pm4py.analysis import cluster_log, check_soundness, compute_emd, solve_marking_equation, solve_extended_marking_equation, \
     construct_synchronous_product_net, insert_artificial_start_end, check_is_workflow_net, maximal_decomposition, generate_marking, \
-    reduce_petri_net_invisibles, reduce_petri_net_implicit_places, insert_case_arrival_finish_rate, insert_case_service_waiting_time
+    reduce_petri_net_invisibles, reduce_petri_net_implicit_places, insert_case_arrival_finish_rate, insert_case_service_waiting_time, get_enabled_transitions
 from pm4py.stats import get_start_activities, get_end_activities, get_event_attributes, get_event_attribute_values, get_variants, \
     get_trace_attributes, get_variants_as_tuples, get_trace_attribute_values, get_case_arrival_average, \
     get_minimum_self_distances, get_minimum_self_distance_witnesses, \
     get_case_arrival_average, get_rework_cases_per_activity, get_case_overlap, get_cycle_time, \
     get_all_case_durations, get_case_duration, get_activity_position_summary, get_stochastic_language
 from pm4py.sim import play_out, generate_process_tree
 from pm4py.ml import split_train_test, get_prefixes_from_log, extract_ocel_features, extract_features_dataframe, extract_temporal_features_dataframe, extract_outcome_enriched_dataframe, extract_target_vector
```

### Comparing `pm4py-2.7.4/pm4py/algo/__init__.py` & `pm4py-2.7.5/pm4py/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/algorithm.py` & `pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/extended_marking_equation/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/analysis/extended_marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/marking_equation/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/marking_equation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/marking_equation/algorithm.py` & `pm4py-2.7.5/pm4py/algo/analysis/marking_equation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/marking_equation/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/marking_equation/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/marking_equation/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/analysis/marking_equation/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/algorithm.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/minimal_coverability_graph/minimal_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/reachability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/reachability_graph/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/restricted_coverability_graph/restricted_coverability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/graphs/utility.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/graphs/utility.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/not_well_handled_pairs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/not_well_handled_pairs/not_well_handled_pairs.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/place_invariants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/s_component.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/s_component.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/uniform_invariant.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/woflan/place_invariants/utility.py` & `pm4py-2.7.5/pm4py/algo/analysis/woflan/place_invariants/utility.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/workflow_net/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/workflow_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/workflow_net/algorithm.py` & `pm4py-2.7.5/pm4py/algo/analysis/workflow_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/workflow_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/analysis/workflow_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/analysis/workflow_net/variants/petri_net.py` & `pm4py-2.7.5/pm4py/algo/analysis/workflow_net/variants/petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/algorithm.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/AttributeAnonymizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/TraceMatcher.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/TraceMatcher.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/util/trace_levenshtein.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/pripel/variants/pripel.py` & `pm4py-2.7.5/pm4py/algo/anonymization/pripel/variants/pripel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/algorithm.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/behavioralAppropriateness.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/exp_mech.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/util/util.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/util/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/laplace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py` & `pm4py-2.7.5/pm4py/algo/anonymization/trace_variant_query/variants/sacofa.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/profiles/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/profiles/algorithm.py` & `pm4py-2.7.5/pm4py/algo/clustering/profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/profiles/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py` & `pm4py-2.7.5/pm4py/algo/clustering/profiles/variants/sklearn_profiles.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/algorithm.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/dfg/dfg_dist.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/leven_dist/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/leven_dist/leven_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/linkage_method/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/linkage_method/linkage_avg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/merge_log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/merge_log/merge_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/util/filter_subsets.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/act_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/logslice_dist.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/sim_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py` & `pm4py-2.7.5/pm4py/algo/clustering/trace_attribute_driven/variants/suc_dist_calc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/comparison/__init__.py` & `pm4py-2.7.5/pm4py/algo/comparison/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/comparison/petrinet/__init__.py` & `pm4py-2.7.5/pm4py/algo/comparison/petrinet/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/comparison/petrinet/element_usage_comparison.py` & `pm4py-2.7.5/pm4py/algo/comparison/petrinet/element_usage_comparison.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/decomposed/variants/recompos_maximal.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/dfg/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/edit_distance/variants/edit_distance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/utils/log_enrichment.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_less_memory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/generator_dijkstra_no_heuristics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/petri_net/variants/tweaked_state_equation_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/util/search_graph_pt_replay_semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/calculate_a_sa_ea_sets.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/matrix_lp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/original.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/approximated/utilities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py` & `pm4py-2.7.5/pm4py/algo/conformance/alignments/process_tree/variants/search_graph_pt.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/antialignments/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/antialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/antialignments/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/antialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/antialignments/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/antialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py` & `pm4py-2.7.5/pm4py/algo/conformance/antialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/util/evaluation.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/util/tree_visualization.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/util/tree_visualization.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/log_extensive.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/log_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/log_model.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/log_model.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/footprints/variants/trace_extensive.py` & `pm4py-2.7.5/pm4py/algo/conformance/footprints/variants/trace_extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/log_skeleton/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/conformance/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/multialignments/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/multialignments/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/multialignments/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/multialignments/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/multialignments/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/multialignments/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py` & `pm4py-2.7.5/pm4py/algo/conformance/multialignments/variants/discounted_a_star.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/dataframe.py` & `pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/temporal_profile/variants/log.py` & `pm4py-2.7.5/pm4py/algo/conformance/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/algorithm.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/duration_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/diagnostics/root_cause_analysis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/backwards.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/backwards.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/conformance/tokenreplay/variants/token_replay.py` & `pm4py-2.7.5/pm4py/algo/conformance/tokenreplay/variants/token_replay.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/__init__.py` & `pm4py-2.7.5/pm4py/algo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/algorithm.py` & `pm4py-2.7.5/pm4py/algo/connectors/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/connectors/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/util/mail.py` & `pm4py-2.7.5/pm4py/algo/connectors/util/mail.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/camunda_workflow.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/camunda_workflow.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/chrome_history.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/chrome_history.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/firefox_history.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/firefox_history.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/github_repo.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/github_repo.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/outlook_calendar.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/outlook_calendar.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/outlook_mail_extractor.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/outlook_mail_extractor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/sap_accounting.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/sap_accounting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/sap_o2c.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/sap_o2c.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/connectors/variants/windows_events.py` & `pm4py-2.7.5/pm4py/algo/connectors/variants/windows_events.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/decision_mining/__init__.py` & `pm4py-2.7.5/pm4py/algo/decision_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/decision_mining/algorithm.py` & `pm4py-2.7.5/pm4py/algo/decision_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/algorithm.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 '''
 import pkgutil
 from enum import Enum
 
 from pm4py import util as pmutil
 from pm4py.algo.discovery.alpha import variants
 from pm4py.algo.discovery.dfg.adapters.pandas import df_statistics
+from pm4py.statistics.start_activities.pandas import get as start_activities_get
+from pm4py.statistics.end_activities.pandas import get as end_activities_get
 from pm4py.objects.conversion.log import converter as log_conversion
 from pm4py.util import exec_utils
 from pm4py.util import xes_constants as xes_util
 from pm4py.util import constants
 from enum import Enum
 from typing import Optional, Dict, Any, Union, Tuple
 from pm4py.objects.log.obj import EventLog, EventStream
@@ -78,21 +80,22 @@
         parameters = {}
     case_id_glue = exec_utils.get_param_value(Parameters.CASE_ID_KEY, parameters, pmutil.constants.CASE_CONCEPT_NAME)
     activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes_util.DEFAULT_NAME_KEY)
     start_timestamp_key = exec_utils.get_param_value(Parameters.START_TIMESTAMP_KEY, parameters,
                                                      None)
     timestamp_key = exec_utils.get_param_value(Parameters.TIMESTAMP_KEY, parameters, xes_util.DEFAULT_TIMESTAMP_KEY)
 
-    if pkgutil.find_loader("pandas"):
-        import pandas
-        if isinstance(log, pandas.core.frame.DataFrame) and variant == ALPHA_VERSION_CLASSIC:
-            dfg = df_statistics.get_dfg_graph(log, case_id_glue=case_id_glue,
-                                              activity_key=activity_key,
-                                              timestamp_key=timestamp_key, start_timestamp_key=start_timestamp_key)
-            return exec_utils.get_variant(variant).apply_dfg(dfg, parameters=parameters)
+    if isinstance(log, pd.core.frame.DataFrame) and variant == ALPHA_VERSION_CLASSIC:
+        dfg = df_statistics.get_dfg_graph(log, case_id_glue=case_id_glue,
+                                          activity_key=activity_key,
+                                          timestamp_key=timestamp_key, start_timestamp_key=start_timestamp_key)
+        start_activities = start_activities_get.get_start_activities(log, parameters=parameters)
+        end_activities = end_activities_get.get_end_activities(log, parameters=parameters)
+        return exec_utils.get_variant(variant).apply_dfg_sa_ea(dfg, start_activities, end_activities, parameters=parameters)
+
     return exec_utils.get_variant(variant).apply(log_conversion.apply(log, parameters, log_conversion.TO_EVENT_LOG),
                                                  parameters)
 
 
 def apply_dfg(dfg: Dict[Tuple[str, str], int], parameters: Optional[Dict[Union[str, Parameters], Any]] = None, variant=ALPHA_VERSION_CLASSIC) -> Tuple[PetriNet, Marking, Marking]:
     """
     Apply Alpha Miner directly on top of a DFG graph
```

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/data_structures/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/data_structures/alpha_classic_abstraction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/utils/endpoints.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/alpha/variants/plus.py` & `pm4py-2.7.5/pm4py/algo/discovery/alpha/variants/plus.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/utils/detection.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/utils/detection.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/variants/log.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/batches/variants/pandas.py` & `pm4py-2.7.5/pm4py/algo/discovery/batches/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/causal/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/causal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/causal/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/causal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/causal/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/causal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/causal/variants/alpha.py` & `pm4py-2.7.5/pm4py/algo/discovery/causal/variants/alpha.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/causal/variants/heuristic.py` & `pm4py-2.7.5/pm4py/algo/discovery/causal/variants/heuristic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/util.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/classic_split.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/classic_split.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/correlation_mining/variants/trace_based.py` & `pm4py-2.7.5/pm4py/algo/discovery/correlation_mining/variants/trace_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/df_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/adapters/pandas/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/replacement.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/replacement.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/utils/dfg_utils.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/case_attributes.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/case_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/clean.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/clean.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/clean_polars.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/clean_polars.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/freq_triples.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/freq_triples.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/native.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/native.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/dfg/variants/performance.py` & `pm4py-2.7.5/pm4py/algo/discovery/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/dfg/variants/dfg.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/dfg/variants/dfg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/log/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/entire_dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/entire_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/log/variants/trace_by_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/petri/variants/reach_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/footprints/tree/variants/bottomup.py` & `pm4py-2.7.5/pm4py/algo/discovery/footprints/tree/variants/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/heuristics/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/heuristics/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/heuristics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/heuristics/variants/plusplus.py` & `pm4py-2.7.5/pm4py/algo/discovery/heuristics/variants/plusplus.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ilp/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ilp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ilp/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ilp/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ilp/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ilp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ilp/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/ilp/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/abc.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/empty_log.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/empty_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/factory.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/base_case/single_activity.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/base_case/single_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/abc.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/concurrency.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/concurrency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/factory.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/loop.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/sequence.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/sequence.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/utils.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/cuts/xor.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/cuts/xor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/im_dfg.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/im_dfg.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/dtypes/im_ds.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/dtypes/im_ds.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/abc.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/activity_concurrent.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/activity_once_per_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/empty_traces.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/empty_traces.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/factory.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/factory.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/flower.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/flower.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/strict_tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/fall_through/tau_loop.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/fall_through/tau_loop.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/abc.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/abc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/im.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/im.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/imd.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/imd.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/imf.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/imf.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/inductive/variants/instances.py` & `pm4py-2.7.5/pm4py/algo/discovery/inductive/variants/instances.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/trace_skel.py` & `pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/trace_skel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/log_skeleton/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/log_skeleton/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/utils.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/log.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py` & `pm4py-2.7.5/pm4py/algo/discovery/minimum_self_distance/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/utils/merge_dataframe_rel_cases.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/interleavings/variants/timestamp_interleavings.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/link_analysis/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/ocpn/variants/wo_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/discovery/ocel/saw_nets/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/dataframe_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/log.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py` & `pm4py-2.7.5/pm4py/algo/discovery/performance_spectrum/variants/log_disconnected.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/dataframe.py` & `pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/temporal_profile/variants/log.py` & `pm4py-2.7.5/pm4py/algo/discovery/temporal_profile/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/transition_system/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/transition_system/algorithm.py` & `pm4py-2.7.5/pm4py/algo/discovery/transition_system/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/transition_system/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/discovery/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/discovery/transition_system/variants/view_based.py` & `pm4py-2.7.5/pm4py/algo/discovery/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py` & `pm4py-2.7.5/pm4py/algo/evaluation/earth_mover_distance/variants/pyemd.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/generalization/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/generalization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/generalization/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/generalization/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/generalization/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/generalization/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/generalization/variants/token_based.py` & `pm4py-2.7.5/pm4py/algo/evaluation/generalization/variants/token_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/dfg/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/utils.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/align_etconformance.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/align_etconformance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/precision/variants/etconformance_token.py` & `pm4py-2.7.5/pm4py/algo/evaluation/precision/variants/etconformance_token.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/algorithm.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,109 +10,111 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.algo.evaluation.replay_fitness.variants import alignment_based, token_replay
-from pm4py.algo.conformance import alignments
-from pm4py.objects.conversion.log import converter as log_conversion
+from pm4py.algo.discovery.dfg.variants import native, performance
+from pm4py.statistics.attributes.log import get as attr_get
+from pm4py.util import xes_constants as xes
+from pm4py.visualization.petri_net.common import visualize
+from pm4py.visualization.petri_net.util.vis_trans_shortest_paths import get_decorations_from_dfg_spaths_acticount
+from pm4py.visualization.petri_net.util.vis_trans_shortest_paths import get_shortest_paths
 from pm4py.util import exec_utils
-from pm4py.objects.petri_net.utils.check_soundness import check_easy_soundness_net_in_fin_marking
 from enum import Enum
+from pm4py.util.constants import PARAMETER_CONSTANT_ACTIVITY_KEY, PARAMETER_CONSTANT_TIMESTAMP_KEY
+from pm4py.objects.petri_net.obj import PetriNet, Marking
 from typing import Optional, Dict, Any, Union, Tuple
 from pm4py.objects.log.obj import EventLog, EventStream
-from pm4py.objects.petri_net.obj import PetriNet, Marking
-import pandas as pd
-
-
-class Variants(Enum):
-    ALIGNMENT_BASED = alignment_based
-    TOKEN_BASED = token_replay
+import graphviz
 
 
 class Parameters(Enum):
-    ALIGN_VARIANT = "align_variant"
-
+    FORMAT = "format"
+    DEBUG = "debug"
+    RANKDIR = "set_rankdir"
+    ACTIVITY_KEY = PARAMETER_CONSTANT_ACTIVITY_KEY
+    TIMESTAMP_KEY = PARAMETER_CONSTANT_TIMESTAMP_KEY
+    AGGREGATION_MEASURE = "aggregationMeasure"
+    FONT_SIZE = "font_size"
+    STAT_LOCALE = "stat_locale"
 
-ALIGNMENT_BASED = Variants.ALIGNMENT_BASED
-TOKEN_BASED = Variants.TOKEN_BASED
 
-VERSIONS = {ALIGNMENT_BASED, TOKEN_BASED}
-
-
-def apply(log: Union[EventLog, pd.DataFrame], petri_net: PetriNet, initial_marking: Marking, final_marking: Marking, parameters: Optional[Dict[Union[str, Parameters], Any]] = None, variant=None) -> Dict[str, Any]:
+def get_decorated_net(net, initial_marking, final_marking, log, parameters=None, variant="frequency"):
     """
-    Apply fitness evaluation starting from an event log and a marked Petri net,
-    by using one of the replay techniques provided by PM4Py
+    Get a decorated net according to the specified variant (decorate Petri net based on DFG)
 
     Parameters
-    -----------
-    log
-        Trace log object
-    petri_net
+    ------------
+    net
         Petri net
     initial_marking
         Initial marking
     final_marking
         Final marking
+    log
+        Log to use to decorate the Petri net
     parameters
-        Parameters related to the replay algorithm
+        Algorithm parameters
     variant
-        Chosen variant:
-            - Variants.ALIGNMENT_BASED
-            - Variants.TOKEN_BASED
+        Specify if the decoration should take into account the frequency or the performance
 
     Returns
-    ----------
-    fitness_eval
-        Fitness evaluation
+    ------------
+    gviz
+        GraphViz object
     """
     if parameters is None:
         parameters = {}
 
-    # execute the following part of code when the variant is not specified by the user
-    if variant is None:
-        if not (
-                check_easy_soundness_net_in_fin_marking(petri_net, initial_marking,
-                                                                              final_marking)):
-            # in the case the net is not a easy sound workflow net, we must apply token-based replay
-            variant = TOKEN_BASED
-        else:
-            # otherwise, use the align-etconformance approach (safer, in the case the model contains duplicates)
-            variant = ALIGNMENT_BASED
-
-    if variant == TOKEN_BASED:
-        # execute the token-based replay variant
-        return exec_utils.get_variant(variant).apply(log,
-                                                     petri_net,
-                                                     initial_marking, final_marking, parameters=parameters)
+    aggregation_measure = exec_utils.get_param_value(Parameters.AGGREGATION_MEASURE, parameters,
+                                                     "sum" if "frequency" in variant else "mean")
+
+    activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes.DEFAULT_NAME_KEY)
+    stat_locale = exec_utils.get_param_value(Parameters.STAT_LOCALE, parameters, {})
+
+    # we find the DFG
+    if variant == "performance":
+        dfg = performance.performance(log, parameters=parameters)
     else:
-        # execute the alignments based variant, with the specification of the alignments variant
-        align_variant = exec_utils.get_param_value(Parameters.ALIGN_VARIANT, parameters,
-                                                   alignments.petri_net.algorithm.DEFAULT_VARIANT)
-        return exec_utils.get_variant(variant).apply(log,
-                                                     petri_net,
-                                                     initial_marking, final_marking, align_variant=align_variant,
-                                                     parameters=parameters)
+        dfg = native.native(log, parameters=parameters)
+    # we find shortest paths
+    spaths = get_shortest_paths(net)
+    # we find the number of activities occurrences in the log
+    activities_count = attr_get.get_attribute_values(log, activity_key, parameters=parameters)
+    aggregated_statistics = get_decorations_from_dfg_spaths_acticount(net, dfg, spaths,
+                                                                      activities_count,
+                                                                      variant=variant,
+                                                                      aggregation_measure=aggregation_measure,
+                                                                      stat_locale=stat_locale)
+
+    return visualize.apply(net, initial_marking, final_marking, parameters=parameters,
+                           decorations=aggregated_statistics)
 
 
-def evaluate(results, parameters=None, variant=TOKEN_BASED):
+def apply(net: PetriNet, initial_marking: Marking, final_marking: Marking, log: EventLog = None, aggregated_statistics=None, parameters: Optional[Dict[Union[str, Parameters], Any]] = None) -> graphviz.Digraph:
     """
-    Evaluate replay results when the replay algorithm has already been applied
+    Apply performance decoration through greedy algorithm (decorate Petri net based on DFG)
 
     Parameters
-    -----------
-    results
-        Results of the replay algorithm
+    ------------
+    net
+        Petri net
+    initial_marking
+        Initial marking
+    final_marking
+        Final marking
+    log
+        Log to use to decorate the Petri net
+    aggregated_statistics
+        Dictionary containing the frequency statistics
     parameters
-        Possible parameters passed to the evaluation
-    variant
-        Indicates which evaluator is called
+        Algorithm parameters
 
     Returns
-    -----------
-    fitness_eval
-        Fitness evaluation
+    ------------
+    gviz
+        GraphViz object
     """
-    return exec_utils.get_variant(variant).evaluate(results, parameters=parameters)
+    del aggregated_statistics
+    return get_decorated_net(net, initial_marking, final_marking, log, parameters=parameters, variant="performance")
```

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py` & `pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/alignment_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py` & `pm4py-2.7.5/pm4py/algo/evaluation/replay_fitness/variants/token_replay.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/algorithm.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/arc_degree.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/arc_degree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/extended_cardoso.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py` & `pm4py-2.7.5/pm4py/algo/evaluation/simplicity/variants/extended_cyclomatic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/attributes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/attributes/attributes_common.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/attributes/attributes_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/end_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/end_activities/end_activities_common.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/end_activities/end_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/filtering_constants.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/start_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/start_activities/start_activities_common.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/start_activities/start_activities_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/timestamp/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/common/timestamp/timestamp_common.py` & `pm4py-2.7.5/pm4py/algo/filtering/common/timestamp/timestamp_common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/dfg/dfg_filtering.py` & `pm4py-2.7.5/pm4py/algo/filtering/dfg/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/attr_value_repetition/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/attr_value_repetition/filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/attributes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/attributes/attributes_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/between/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/between/between_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/cases/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/cases/case_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/end_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/end_activities/end_activities_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/ltl/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/ltl/ltl_checker.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/paths/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/paths/paths_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/prefixes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/prefixes/prefix_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/rework/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/rework/rework_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/start_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/start_activities/start_activities_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/suffixes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/suffixes/suffix_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/timestamp/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/timestamp/timestamp_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/log/variants/variants_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/log/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/activity_type_matching.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/activity_type_matching.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/event_attributes.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/event_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/object_attributes.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/object_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/objects_ot_count.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/ocel/ot_endpoints.py` & `pm4py-2.7.5/pm4py/algo/filtering/ocel/ot_endpoints.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/attr_value_repetition/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/attr_value_repetition/filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/attributes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/attributes/attributes_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/attributes/attributes_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/between/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/between/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/between/between_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/between/between_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/cases/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/cases/case_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/cases/case_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/consecutive_act_case_grouping/consecutive_act_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/end_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/end_activities/end_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/ends_with/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/ends_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/ends_with/ends_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/ltl/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/ltl/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/ltl/ltl_checker.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/ltl/ltl_checker.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/paths/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/paths/paths_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/paths/paths_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/pd_filtering_constants.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/pd_filtering_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/prefixes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/prefixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/prefixes/prefix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/rework/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/rework/rework_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/rework/rework_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/start_activities/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/start_activities/start_activities_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/starts_with/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/starts_with/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/starts_with/starts_with_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/suffixes/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/suffixes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/suffixes/suffix_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp/timestamp_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp_case_grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/timestamp_case_grouping/timestamp_case_grouping_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/traces/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/traces/trace_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/traces/trace_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/filtering/pandas/variants/variants_filter.py` & `pm4py-2.7.5/pm4py/algo/filtering/pandas/variants/variants_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/merging/__init__.py` & `pm4py-2.7.5/pm4py/algo/merging/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/merging/case_relations/__init__.py` & `pm4py-2.7.5/pm4py/algo/merging/case_relations/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/merging/case_relations/algorithm.py` & `pm4py-2.7.5/pm4py/algo/merging/case_relations/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/merging/case_relations/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/merging/case_relations/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/merging/case_relations/variants/pandas.py` & `pm4py-2.7.5/pm4py/algo/merging/case_relations/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/local_diagnostics/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/local_diagnostics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/local_diagnostics/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/network_analysis/variants/dataframe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/log.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/resource_profiles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/common/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/common/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/common/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/log.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/roles/variants/pandas.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/roles/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/algorithm.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/util.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/handover.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/handover.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/log/working_together.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/log/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/handover.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/organizational_mining/util.py` & `pm4py-2.7.5/pm4py/algo/organizational_mining/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/__init__.py` & `pm4py-2.7.5/pm4py/algo/querying/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/description/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/log_to_cols_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/log_to_dfg_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/log_to_variants_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/net_to_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/net_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/ocel_fea_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
         return "Number of object of type "+stru.split("@@object_interaction_graph_")[1]+" related to the current object in the object interaction graph"
     elif stru.startswith("@@ocel_lif_path_"):
         path = stru.split("@@ocel_lif_path_")[1]
         act1 = path.split("##")[0]
         act2 = path.split("##")[1]
         return "Frequency of the path \""+act1+"\" -> \""+act2+"\" in the lifecycle of the object"
 
-    print(stru)
-    return None
+    return stru
 
 
 def apply(ocel: OCEL, obj_type: str, parameters: Optional[Dict[Any, Any]] = None) -> str:
     if parameters is None:
         parameters = {}
 
     include_header = exec_utils.get_param_value(Parameters.INCLUDE_HEADER, parameters, True)
@@ -79,15 +78,15 @@
 
     fea_df = pm4py.extract_ocel_features(ocel, obj_type, include_obj_id=False)
 
     cols = []
 
     for c in fea_df.columns:
         ser = fea_df[c]
-        ser1 = ser[ser != 0]
+        ser1 = ser[ser > 0]
         if len(ser1) > 0:
             desc = __transform_to_string(c)
             avg = np.average(ser1)
             stdavg = 0 if avg == 0 or len(ser1) == 1 else np.std(ser1)/avg
             cols.append([desc, len(ser1), stdavg, ser1])
 
     cols = sorted(cols, key=lambda x: (x[1], x[2], x[0]), reverse=True)
```

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/ocel_ocdfg_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/perform_query.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/connectors/openai.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/querying/openai/stream_to_descr.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/abstractions/stream_to_descr.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/reduction/__init__.py` & `pm4py-2.7.5/pm4py/algo/reduction/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/reduction/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/algo/reduction/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/reduction/process_tree/reducer.py` & `pm4py-2.7.5/pm4py/algo/reduction/process_tree/reducer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/reduction/process_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/reduction/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py` & `pm4py-2.7.5/pm4py/algo/reduction/process_tree/variants/tree_tr_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/algorithm.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/utils/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/utils/replay.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/utils/replay.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py` & `pm4py-2.7.5/pm4py/algo/simulation/montecarlo/variants/petri_semaph_fifo.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/algorithm.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/classic.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/dfg/variants/performance.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/algorithm.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/extensive.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/petri_net/variants/stochastic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/algorithm.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/basic_playout.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/extensive.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/extensive.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py` & `pm4py-2.7.5/pm4py/algo/simulation/playout/process_tree/variants/topbottom.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/tree_generator/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/tree_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/tree_generator/algorithm.py` & `pm4py-2.7.5/pm4py/algo/simulation/tree_generator/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/basic.py` & `pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/basic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py` & `pm4py-2.7.5/pm4py/algo/simulation/tree_generator/variants/ptandloggenerator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/util/locally_linear_embedding.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/event_based.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/event_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/temporal.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/temporal.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_features/variants/trace_based.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_features/variants/trace_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 actj = trace[j][activity_key]
                 if st > ct:
                     break
                 if act == actj:
                     conc = conc + 1
                 j = j + 1
             i = i + 1
-            max_conc_act[act] = conc
+            max_conc_act[act] = max(max_conc_act[act], conc)
         arr = []
         for act in activities:
             arr.append(max_conc_act[act])
         data.append(arr)
 
     return data, feature_names
 
@@ -194,30 +194,30 @@
     resource_key = exec_utils.get_param_value(Parameters.RESOURCE_KEY, parameters, xes_constants.DEFAULT_RESOURCE_KEY)
     epsilon = exec_utils.get_param_value(Parameters.EPSILON, parameters, 0.000001)
     default_not_present = exec_utils.get_param_value(Parameters.DEFAULT_NOT_PRESENT, parameters, 0)
 
     tree_dict = {}
     for case in log:
         if case:
-            resources = set(x[resource_key] for x in case)
+            resources = set(x[resource_key] for x in case if resource_key in x)
             st = case[0][start_timestamp_key].timestamp() - epsilon
             ct = case[-1][timestamp_key].timestamp() + epsilon
             for res in resources:
                 if res not in tree_dict:
                     tree_dict[res] = IntervalTree()
                 tree_dict[res].add(Interval(st, ct))
 
     resources_list = sorted(list(tree_dict))
 
     data = []
     feature_names = ["resource_workload@@"+r for r in resources_list]
 
     for case in log:
         data.append([])
-        resources = set(x[resource_key] for x in case)
+        resources = set(x[resource_key] for x in case if resource_key in x)
         st = case[0][start_timestamp_key].timestamp() - epsilon
         ct = case[-1][timestamp_key].timestamp() + epsilon
         for res in resources_list:
             if res in resources:
                 data[-1].append(len(tree_dict[res][st:ct]))
             else:
                 data[-1].append(default_not_present)
```

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_interval_tree/variants/open_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/next_activity.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/next_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/next_time.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/next_time.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_target/variants/remaining_time.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_target/variants/remaining_time.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_trie/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/log_to_trie/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/log_to_trie/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/description/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/description/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/description/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/description/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/description/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/filtering/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,7 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-
```

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/description/variants/variant1.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/description/variants/variant1.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_activity.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_end_ot.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_end_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_num_rel_objs_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_start_ot.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_start_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/event_timestamp.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/event_timestamp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/new_interactions.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/new_interactions.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events/related_objects_features.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events/related_objects_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/events_objects/prefix_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/obj_con_in_graph_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_degree_centrality.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_general_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_activities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_duration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_length.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_lifecycle_unq_act.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_num_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_str_attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/object_work_in_progress.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/objects_interaction_graph_ot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/related_activities_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/features/objects/related_events_features.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/features/objects/related_events_features.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_cobirth_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_codeath_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_descendants_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/object_interaction_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/graphs/ocel20_computation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/algorithm.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/ancestors_descendants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py` & `pm4py-2.7.5/pm4py/algo/transformation/ocel/split_ocel/variants/connected_components.py`

 * *Files 13% similar despite different names*

```diff
@@ -79,14 +79,17 @@
                 removed_nodes.add(n)
                 g.remove_node(n)
 
     conn_comp = list(nx.connected_components(g))
 
     ret = []
 
-    for cc in conn_comp:
-        subocel = deepcopy(ocel)
-        subocel.objects = subocel.objects[subocel.objects[subocel.object_id_column].isin(cc)]
-        subocel = filtering_utils.propagate_object_filtering(subocel, parameters=parameters)
+    for index, cc in enumerate(conn_comp):
+        subocel = OCEL()
+        subocel.objects = ocel.objects[ocel.objects[ocel.object_id_column].isin(cc)]
+        subocel.relations = ocel.relations[ocel.relations[ocel.object_id_column].isin(cc)]
+        included_evs = subocel.relations[ocel.event_id_column].unique()
+        subocel.events = ocel.events[ocel.events[ocel.event_id_column].isin(included_evs)]
+
         ret.append(subocel)
 
     return ret
```

### Comparing `pm4py-2.7.4/pm4py/analysis.py` & `pm4py-2.7.5/pm4py/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 __doc__ = """
 """
 
-from typing import List, Optional, Tuple, Dict, Union, Generator
+from typing import List, Optional, Tuple, Dict, Union, Generator, Set
 
 from pm4py.objects.log.obj import Trace, EventLog, EventStream
 from pm4py.objects.conversion.log import converter as log_converter
 from pm4py.utils import __event_log_deprecation_warning
 from pm4py.objects.petri_net.obj import PetriNet, Marking
 from pm4py.utils import get_properties, constants, pandas_utils
 from pm4py.util.pandas_utils import check_is_pandas_dataframe, check_pandas_dataframe_columns
@@ -424,7 +424,26 @@
 
         net, im, fm = pm4py.read_pnml('model.pnml')
         net = pm4py.reduce_petri_net_implicit_places(net, im, fm)
     """
     from pm4py.objects.petri_net.utils import murata
     return murata.apply_reduction(net, im, fm)
 
+
+def get_enabled_transitions(net: PetriNet, marking: Marking) -> Set[PetriNet.Transition]:
+    """
+    Gets the transitions enabled in a given marking
+
+    :param net: Petri net
+    :param marking: marking
+    :rtype: ``Set[PetriNet.Transition]``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        net, im, fm = pm4py.read_pnml('tests/input_data/running-example.pnml')
+        # gets the transitions enabled in the initial marking
+        enabled_transitions = pm4py.get_enabled_transitions(net, im)
+    """
+    from pm4py.objects.petri_net import semantics
+    return semantics.enabled_transitions(net, marking)
```

### Comparing `pm4py-2.7.4/pm4py/cli.py` & `pm4py-2.7.5/pm4py/cli.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/conformance.py` & `pm4py-2.7.5/pm4py/conformance.py`

 * *Files 3% similar despite different names*

```diff
@@ -232,15 +232,15 @@
     from pm4py.algo.evaluation.replay_fitness import algorithm as replay_fitness
     result = replay_fitness.apply(log, petri_net, initial_marking, final_marking,
                                 variant=replay_fitness.Variants.TOKEN_BASED, parameters=properties)
 
     return result
 
 
-def fitness_alignments(log: Union[EventLog, pd.DataFrame], petri_net: PetriNet, initial_marking: Marking, final_marking: Marking, multi_processing: bool = constants.ENABLE_MULTIPROCESSING_DEFAULT, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> \
+def fitness_alignments(log: Union[EventLog, pd.DataFrame], petri_net: PetriNet, initial_marking: Marking, final_marking: Marking, multi_processing: bool = constants.ENABLE_MULTIPROCESSING_DEFAULT, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name", variant_str : Optional[str] = None) -> \
         Dict[str, float]:
     """
     Calculates the fitness using alignments
 
     Alignment-based replay aims to find one of the best alignment between the trace and the model. For each trace, the output of an alignment is a list of couples where the first element is an event (of the trace) or » and the second element is a transition (of the model) or ». For each couple, the following classification could be provided:
 
     - Sync move: the classification of the event corresponds to the transition label; in this case, both the trace and the model advance in the same way during the replay.
@@ -257,14 +257,15 @@
     :param petri_net: petri net
     :param initial_marking: initial marking
     :param final_marking: final marking
     :param multi_processing: boolean value that enables the multiprocessing
     :param activity_key: attribute to be used for the activity
     :param timestamp_key: attribute to be used for the timestamp
     :param case_id_key: attribute to be used as case identifier
+    :param variant_str: variant specification
     :rtype: ``Dict[str, float]``
 
     .. code-block:: python3
 
         import pm4py
 
         net, im, fm = pm4py.discover_petri_net_inductive(dataframe, activity_key='concept:name', case_id_key='case:concept:name', timestamp_key='time:timestamp')
@@ -276,15 +277,15 @@
     if check_is_pandas_dataframe(log):
         check_pandas_dataframe_columns(log, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
 
     from pm4py.algo.evaluation.replay_fitness import algorithm as replay_fitness
     parameters = get_properties(log, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
     parameters["multiprocessing"] = multi_processing
     result = replay_fitness.apply(log, petri_net, initial_marking, final_marking,
-                                variant=replay_fitness.Variants.ALIGNMENT_BASED, parameters=parameters)
+                                variant=replay_fitness.Variants.ALIGNMENT_BASED, align_variant=variant_str, parameters=parameters)
 
     return result
 
 
 def precision_token_based_replay(log: Union[EventLog, pd.DataFrame], petri_net: PetriNet, initial_marking: Marking,
                                  final_marking: Marking, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> float:
     """
@@ -379,14 +380,50 @@
     result = precision_evaluator.apply(log, petri_net, initial_marking, final_marking,
                                      variant=precision_evaluator.Variants.ALIGN_ETCONFORMANCE,
                                      parameters=parameters)
 
     return result
 
 
+def replay_prefix_tbr(prefix: List[str], net: PetriNet, im: Marking, fm: Marking, activity_key: str = "concept:name") -> Marking:
+    """
+    Replays a prefix (list of activities) on a given accepting Petri net, using Token-Based Replay.
+
+    :param prefix: list of activities
+    :param net: Petri net
+    :param im: initial marking
+    :param fm: final marking
+    :param activity_key: attribute to be used as activity
+    :rtype:  ``Marking``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        net, im, fm = pm4py.read_pnml('tests/input_data/running-example.pnml')
+        marking = pm4py.replay_prefix_tbr(['register request', 'check ticket'], net, im, fm)
+    """
+    purpose_log = EventLog()
+    trace = Trace()
+    for act in prefix:
+        trace.append(Event({activity_key: act}))
+    purpose_log.append(trace)
+
+    from pm4py.algo.conformance.tokenreplay.variants import token_replay
+    parameters_tr = {
+        token_replay.Parameters.CONSIDER_REMAINING_IN_FITNESS: False,
+        token_replay.Parameters.TRY_TO_REACH_FINAL_MARKING_THROUGH_HIDDEN: False,
+        token_replay.Parameters.STOP_IMMEDIATELY_UNFIT: True,
+        token_replay.Parameters.WALK_THROUGH_HIDDEN_TRANS: True,
+        token_replay.Parameters.ACTIVITY_KEY: activity_key
+    }
+    res = token_replay.apply(purpose_log, net, im, fm, parameters=parameters_tr)[0]
+    return res["reached_marking"]
+
+
 @deprecation.deprecated(deprecated_in="2.3.0", removed_in="3.0.0", details="conformance checking using footprints will not be exposed in a future release")
 def __convert_to_fp(*args) -> Union[List[Dict[str, Any]], Dict[str, Any]]:
     """
     Internal method to convert the provided event log / process model argument
     to footprints (using footprints discovery)
 
     :param args: event log / process model
```

### Comparing `pm4py-2.7.4/pm4py/connectors.py` & `pm4py-2.7.5/pm4py/connectors.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/convert.py` & `pm4py-2.7.5/pm4py/convert.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/discovery.py` & `pm4py-2.7.5/pm4py/discovery.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/filtering.py` & `pm4py-2.7.5/pm4py/filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/hof.py` & `pm4py-2.7.5/pm4py/hof.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/meta.py` & `pm4py-2.7.5/pm4py/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 __name__ = 'pm4py'
-VERSION = '2.7.4'
+VERSION = '2.7.5'
 __version__ = VERSION
 __doc__ = 'Process mining for Python'
 __author__ = 'Fraunhofer Institute for Applied Technology'
 __author_email__ = 'pm4py@fit.fraunhofer.de'
 __maintainer__ = 'Fraunhofer Institute for Applied Technology'
 __maintainer_email__ = "pm4py@fit.fraunhofer.de"
```

### Comparing `pm4py-2.7.4/pm4py/ml.py` & `pm4py-2.7.5/pm4py/ml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/__init__.py` & `pm4py-2.7.5/pm4py/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/exporter/exporter.py` & `pm4py-2.7.5/pm4py/objects/bpmn/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/exporter/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/exporter/variants/etree.py` & `pm4py-2.7.5/pm4py/objects/bpmn/exporter/variants/etree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/importer/importer.py` & `pm4py-2.7.5/pm4py/objects/bpmn/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/importer/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/importer/variants/lxml.py` & `pm4py-2.7.5/pm4py/objects/bpmn/importer/variants/lxml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/layout/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/layout/layouter.py` & `pm4py-2.7.5/pm4py/objects/bpmn/layout/layouter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/layout/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/layout/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/layout/variants/graphviz.py` & `pm4py-2.7.5/pm4py/objects/bpmn/layout/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/obj.py` & `pm4py-2.7.5/pm4py/objects/bpmn/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/semantics.py` & `pm4py-2.7.5/pm4py/objects/bpmn/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/util/__init__.py` & `pm4py-2.7.5/pm4py/objects/bpmn/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/util/bpmn_utils.py` & `pm4py-2.7.5/pm4py/objects/bpmn/util/bpmn_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/util/reduction.py` & `pm4py-2.7.5/pm4py/objects/bpmn/util/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/bpmn/util/sorting.py` & `pm4py-2.7.5/pm4py/objects/bpmn/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/bpmn/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/bpmn/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/bpmn/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/bpmn/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/bpmn/variants/to_petri_net.py` & `pm4py-2.7.5/pm4py/objects/conversion/bpmn/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/dfg/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/dfg/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/dfg/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py` & `pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/to_petri_net_activity_defines_place.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py` & `pm4py-2.7.5/pm4py/objects/conversion/dfg/variants/to_petri_net_invisibles_no_duplicates.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py` & `pm4py-2.7.5/pm4py/objects/conversion/heuristics_net/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/constants.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/df_to_event_log_1v.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/df_to_event_log_nv.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_data_frame.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_data_frame.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_event_log.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_event_log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_event_stream.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/log/variants/to_nx.py` & `pm4py-2.7.5/pm4py/objects/conversion/log/variants/to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/ocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/ocel/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/ocel/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py` & `pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/ocel_features_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py` & `pm4py-2.7.5/pm4py/objects/conversion/ocel/variants/ocel_to_nx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_bpmn.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_petri_net.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_petri_net.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py` & `pm4py-2.7.5/pm4py/objects/conversion/process_tree/variants/to_petri_net_transition_bordered.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/wf_net/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/wf_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/wf_net/converter.py` & `pm4py-2.7.5/pm4py/objects/conversion/wf_net/converter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/to_bpmn.py` & `pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/to_bpmn.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/conversion/wf_net/variants/to_process_tree.py` & `pm4py-2.7.5/pm4py/objects/conversion/wf_net/variants/to_process_tree.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/exporter/exporter.py` & `pm4py-2.7.5/pm4py/objects/dfg/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/exporter/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/exporter/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/dfg/exporter/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/filtering/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/filtering/dfg_filtering.py` & `pm4py-2.7.5/pm4py/objects/dfg/filtering/dfg_filtering.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/importer/importer.py` & `pm4py-2.7.5/pm4py/objects/dfg/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/importer/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/importer/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/dfg/importer/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/obj.py` & `pm4py-2.7.5/pm4py/objects/dfg/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/retrieval/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/retrieval/log.py` & `pm4py-2.7.5/pm4py/objects/dfg/retrieval/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/retrieval/pandas.py` & `pm4py-2.7.5/pm4py/objects/dfg/retrieval/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/util.py` & `pm4py-2.7.5/pm4py/objects/dfg/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/utils/__init__.py` & `pm4py-2.7.5/pm4py/objects/dfg/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/dfg/utils/dfg_utils.py` & `pm4py-2.7.5/pm4py/objects/dfg/utils/dfg_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/heuristics_net/__init__.py` & `pm4py-2.7.5/pm4py/objects/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/heuristics_net/defaults.py` & `pm4py-2.7.5/pm4py/objects/heuristics_net/defaults.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/heuristics_net/edge.py` & `pm4py-2.7.5/pm4py/objects/heuristics_net/edge.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/heuristics_net/node.py` & `pm4py-2.7.5/pm4py/objects/heuristics_net/node.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/heuristics_net/obj.py` & `pm4py-2.7.5/pm4py/objects/heuristics_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/exporter.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/util/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/util/compression.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/util/compression.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/etree_xes_exp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/exporter/xes/variants/line_by_line.py` & `pm4py-2.7.5/pm4py/objects/log/exporter/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/importer.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/chunk_regex.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/chunk_regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse_20.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse_20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/iterparse_mem_compressed.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/importer/xes/variants/line_by_line.py` & `pm4py-2.7.5/pm4py/objects/log/importer/xes/variants/line_by_line.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/obj.py` & `pm4py-2.7.5/pm4py/objects/log/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/__init__.py` & `pm4py-2.7.5/pm4py/objects/log/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/artificial.py` & `pm4py-2.7.5/pm4py/objects/log/util/artificial.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/basic_filter.py` & `pm4py-2.7.5/pm4py/objects/log/util/basic_filter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/dataframe_utils.py` & `pm4py-2.7.5/pm4py/objects/log/util/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/filtering_utils.py` & `pm4py-2.7.5/pm4py/objects/log/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/get_class_representation.py` & `pm4py-2.7.5/pm4py/objects/log/util/get_class_representation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/get_log_encoded.py` & `pm4py-2.7.5/pm4py/objects/log/util/get_log_encoded.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/get_prefixes.py` & `pm4py-2.7.5/pm4py/objects/log/util/get_prefixes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/index_attribute.py` & `pm4py-2.7.5/pm4py/objects/log/util/index_attribute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/insert_classifier.py` & `pm4py-2.7.5/pm4py/objects/log/util/insert_classifier.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/interval_lifecycle.py` & `pm4py-2.7.5/pm4py/objects/log/util/interval_lifecycle.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/log.py` & `pm4py-2.7.5/pm4py/objects/log/util/log.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/log_regex.py` & `pm4py-2.7.5/pm4py/objects/log/util/log_regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/move_attrs_to_trace.py` & `pm4py-2.7.5/pm4py/objects/log/util/move_attrs_to_trace.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/pandas_log_wrapper.py` & `pm4py-2.7.5/pm4py/objects/log/util/pandas_log_wrapper.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/pandas_numpy_variants.py` & `pm4py-2.7.5/pm4py/objects/log/util/pandas_numpy_variants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/sampling.py` & `pm4py-2.7.5/pm4py/objects/log/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/sorting.py` & `pm4py-2.7.5/pm4py/objects/log/util/sorting.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/split_train_test.py` & `pm4py-2.7.5/pm4py/objects/log/util/split_train_test.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/log/util/xes.py` & `pm4py-2.7.5/pm4py/objects/log/util/xes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/constants.py` & `pm4py-2.7.5/pm4py/objects/ocel/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/exporter.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/csv/variants/pandas.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/exporter.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/exporter.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/ocel20.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/sqlite/variants/pandas_exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/util/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/util/clean_dataframes.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/util/clean_dataframes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/exporter.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py` & `pm4py-2.7.5/pm4py/objects/ocel/exporter/xmlocel/variants/ocel20.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,17 @@
     EVENT_TIMESTAMP = constants.PARAM_EVENT_TIMESTAMP
     OBJECT_ID = constants.PARAM_OBJECT_ID
     OBJECT_TYPE = constants.PARAM_OBJECT_TYPE
     QUALIFIER = constants.PARAM_QUALIFIER
     CHANGED_FIELD = constants.PARAM_CHNGD_FIELD
 
 
+RELOBJ_TAG = "object"
+
+
 def apply(ocel: OCEL, target_path: str, parameters: Optional[Dict[Any, Any]] = None):
     if parameters is None:
         parameters = {}
 
     event_id_column = exec_utils.get_param_value(Parameters.EVENT_ID, parameters, ocel.event_id_column)
     event_activity_column = exec_utils.get_param_value(Parameters.EVENT_ACTIVITY, parameters, ocel.event_activity)
     event_timestamp_column = exec_utils.get_param_value(Parameters.EVENT_TIMESTAMP, parameters, ocel.event_timestamp)
@@ -84,16 +87,16 @@
 
     for objid, obj in objects0.items():
         obj = {x: y for x, y in obj.items() if not x.startswith("ocel:") and y is not None and not pd.isna(y)}
         if len(obj) > 0:
             object_changes2[objid] = {}
             object_changes3[objid] = []
             for x, y in obj.items():
-                object_changes2[objid][x] = [(y, "0")]
-                object_changes3[objid].append((x, y, "0"))
+                object_changes2[objid][x] = [(y, "1970-01-01T00:00:00")]
+                object_changes3[objid].append((x, y, "1970-01-01T00:00:00"))
 
     for chng in object_changes0:
         oid = chng[object_id_column]
         if oid not in object_changes1:
             object_changes1[oid] = {}
         if oid not in object_changes2:
             object_changes2[oid] = {}
@@ -146,53 +149,26 @@
 
     objects = etree.SubElement(root, "objects")
     for objid, obj in objects0.items():
         object = etree.SubElement(objects, "object")
         object.set("id", str(objid))
         object.set("type", str(obj[object_type_column]))
 
-        """obj = {x: y for x, y in obj.items() if not x.startswith("ocel:") and y is not None and not pd.isna(y)}
-        object_attributes = etree.SubElement(object, "attributes")
-        object_attributes.set("time", "0")
-        if len(obj) > 0:
-            for k, v in obj.items():
-                object_attribute = etree.SubElement(object_attributes, "attribute")
-                object_attribute.set("name", k)
-                object_attribute.text = str(v)
-        if objid in object_changes1:
-            for timee in object_changes1[objid]:
-                object_attributes = etree.SubElement(object, "attributes")
-                object_attributes.set("time", timee.isoformat())
-                for el in object_changes1[objid][timee]:
-                    object_attribute = etree.SubElement(object_attributes, "attribute")
-                    object_attribute.set("name", el[0])
-                    object_attribute.text = str(el[1])"""
-
-        """object_attributes = etree.SubElement(object, "attributes")
-        if objid in object_changes2:
-            for attr, val in object_changes2[objid].items():
-                object_attribute = etree.SubElement(object_attributes, "attribute")
-                object_attribute.set("name", attr)
-                for tup in val:
-                    object_attrval = etree.SubElement(object_attribute, "value")
-                    object_attrval.set("time", tup[1])
-                    object_attrval.text = tup[0]"""
-
         object_attributes = etree.SubElement(object, "attributes")
         if objid in object_changes3:
             for val in object_changes3[objid]:
                 object_attribute = etree.SubElement(object_attributes, "attribute")
                 object_attribute.set("name", val[0])
                 object_attribute.set("time", val[2])
                 object_attribute.text = str(val[1])
 
         if objid in o2o_dict:
             object_objects = etree.SubElement(object, "objects")
             for i in range(len(o2o_dict[objid][0])):
-                object_object = etree.SubElement(object_objects, "object")
+                object_object = etree.SubElement(object_objects, RELOBJ_TAG)
                 object_object.set("object-id", o2o_dict[objid][0][i])
                 object_object.set("qualifier", o2o_dict[objid][1][i])
 
     events = etree.SubElement(root, "events")
     for evid, eve in events0.items():
         event = etree.SubElement(events, "event")
         event.set("id", str(evid))
@@ -200,15 +176,15 @@
         event.set("time", eve[event_timestamp_column].isoformat())
         event_attributes = etree.SubElement(event, "attributes")
         event_objects = etree.SubElement(event, "objects")
         if evid in relations0_obj_ids:
             this_ids = relations0_obj_ids[evid]
             this_qualifiers = relations0_qualifiers[evid]
             for i in range(len(this_ids)):
-                event_object = etree.SubElement(event_objects, "object")
+                event_object = etree.SubElement(event_objects, RELOBJ_TAG)
                 event_object.set("object-id", str(this_ids[i]))
                 event_object.set("qualifier", str(this_qualifiers[i]))
         eve = {x: y for x, y in eve.items() if not x.startswith("ocel:") and y is not None and not pd.isna(y)}
         if len(eve) > 0:
             for k, v in eve.items():
                 event_attribute = etree.SubElement(event_attributes, "attribute")
                 event_attribute.set("name", k)
```

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/csv/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/csv/importer.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/csv/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/csv/variants/pandas.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/csv/variants/pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/importer.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/jsonocel/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/jsonocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/importer.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/ocel20.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,43 +19,58 @@
 
 from pm4py.objects.ocel import constants
 from pm4py.objects.ocel.obj import OCEL
 from pm4py.util import exec_utils
 import pandas as pd
 from pm4py.objects.ocel.util import ocel_consistency
 from pm4py.objects.ocel.util import filtering_utils
+from pm4py.objects.ocel.validation import ocel20_rel_validation
+import warnings
 
 
 class Parameters(Enum):
     EVENT_ID = constants.PARAM_EVENT_ID
     EVENT_ACTIVITY = constants.PARAM_EVENT_ACTIVITY
     EVENT_TIMESTAMP = constants.PARAM_EVENT_TIMESTAMP
     OBJECT_ID = constants.PARAM_OBJECT_ID
     OBJECT_TYPE = constants.PARAM_OBJECT_TYPE
     INTERNAL_INDEX = constants.PARAM_INTERNAL_INDEX
     QUALIFIER = constants.PARAM_QUALIFIER
     CHANGED_FIELD = constants.PARAM_CHNGD_FIELD
+    VALIDATION = "validation"
+    EXCEPT_IF_INVALID = "except_if_invalid"
 
 
 def apply(file_path: str, parameters: Optional[Dict[Any, Any]] = None):
     if parameters is None:
         parameters = {}
 
     import sqlite3
 
+    validation = exec_utils.get_param_value(Parameters.VALIDATION, parameters, True)
+    except_if_invalid = exec_utils.get_param_value(Parameters.EXCEPT_IF_INVALID, parameters, False)
+
     event_id = exec_utils.get_param_value(Parameters.EVENT_ID, parameters, constants.DEFAULT_EVENT_ID)
     event_activity = exec_utils.get_param_value(Parameters.EVENT_ACTIVITY, parameters, constants.DEFAULT_EVENT_ACTIVITY)
     event_timestamp = exec_utils.get_param_value(Parameters.EVENT_TIMESTAMP, parameters,
                                                  constants.DEFAULT_EVENT_TIMESTAMP)
     object_id = exec_utils.get_param_value(Parameters.OBJECT_ID, parameters, constants.DEFAULT_OBJECT_ID)
     object_type = exec_utils.get_param_value(Parameters.OBJECT_TYPE, parameters, constants.DEFAULT_OBJECT_TYPE)
     internal_index = exec_utils.get_param_value(Parameters.INTERNAL_INDEX, parameters, constants.DEFAULT_INTERNAL_INDEX)
     qualifier_field = exec_utils.get_param_value(Parameters.QUALIFIER, parameters, constants.DEFAULT_QUALIFIER)
     changed_field = exec_utils.get_param_value(Parameters.CHANGED_FIELD, parameters, constants.DEFAULT_CHNGD_FIELD)
 
+    if validation:
+        satisfied, unsatisfied = ocel20_rel_validation.apply(file_path)
+        if unsatisfied:
+            warnings.warn("There are unsatisfied OCEL 2.0 constraints in the given relational database: "+str(unsatisfied))
+
+            if except_if_invalid:
+                raise Exception("OCEL 2.0 validation failed.")
+
     conn = sqlite3.connect(file_path)
 
     EVENTS = pd.read_sql("SELECT * FROM event", conn)
     OBJECTS = pd.read_sql("SELECT * FROM object", conn)
 
     etypes = sorted(list(EVENTS["ocel_type"].unique()))
     otypes = sorted(list(OBJECTS["ocel_type"].unique()))
```

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/sqlite/variants/pandas_importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/importer.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/classic.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py` & `pm4py-2.7.5/pm4py/objects/ocel/importer/xmlocel/variants/ocel20.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                             attribute_name = attribute.get("name")
                             attribute_time = attribute.get("time")
                             try:
                                 attribute_type = object_type_attributes[object_type][attribute_name]
                             except:
                                 attribute_type = "string"
                             attribute_text = parse_xml(attribute.text, attribute_type, date_parser)
-                            if attribute_time == "0":
+                            if attribute_time == "0" or attribute_time == "1970-01-01T00:00:00":
                                 obj_dict[attribute_name] = attribute_text
                             else:
                                 attribute_time = date_parser.apply(attribute_time)
                                 obj_change_dict = {object_id_column: object_id, object_type_column: object_type, attribute_name: attribute_text, changed_field: attribute_name, event_timestamp_column: attribute_time}
                                 object_changes_list.append(obj_change_dict)
 
                 objects_list.append(obj_dict)
```

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/obj.py` & `pm4py-2.7.5/pm4py/objects/ocel/obj.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,12 +117,12 @@
     def __str__(self):
         return str(self.get_summary())
 
     def __repr__(self):
         return str(self.get_summary())
 
     def __copy__(self):
-        return OCEL(self.events, self.objects, self.relations, copy(self.globals), copy(self.parameters), copy(self.o2o), copy(self.e2e))
+        return OCEL(self.events, self.objects, self.relations, copy(self.globals), copy(self.parameters), copy(self.o2o), copy(self.e2e), copy(self.object_changes))
 
     def __deepcopy__(self, memo):
         return OCEL(self.events.copy(), self.objects.copy(), self.relations.copy(), deepcopy(self.globals),
-                    deepcopy(self.parameters), deepcopy(self.o2o), deepcopy(self.e2e))
+                    deepcopy(self.parameters), deepcopy(self.o2o), deepcopy(self.e2e), deepcopy(self.object_changes))
```

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/attributes_names.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/attributes_names.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/convergence_divergence_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/e2o_qualification.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/e2o_qualification.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/ev_att_to_obj_type.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/ev_att_to_obj_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/event_prefix_suffix_per_obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/events_per_object_type.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/events_per_object_type.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/events_per_type_per_activity.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/events_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/explode.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/explode.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/extended_table.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/extended_table.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/filtering_utils.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/filtering_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/flattening.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/flattening.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/log_ocel.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/log_ocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/names_stripping.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/names_stripping.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/objects_per_type_per_activity.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/objects_per_type_per_activity.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/ocel_consistency.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/ocel_consistency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/ocel_iterator.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/ocel_iterator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/parent_children_ref.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/parent_children_ref.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/related_events.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/related_events.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/related_objects.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/related_objects.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/util/sampling.py` & `pm4py-2.7.5/pm4py/objects/ocel/util/sampling.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/validation/__init__.py` & `pm4py-2.7.5/pm4py/objects/ocel/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/validation/jsonocel.py` & `pm4py-2.7.5/pm4py/objects/ocel/validation/jsonocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/ocel/validation/xmlocel.py` & `pm4py-2.7.5/pm4py/objects/ocel/validation/xmlocel.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 import pkgutil
 
 
 def apply(input_path, validation_path, parameters=None):
-    import lxml.etree
-
     if not pkgutil.find_loader("lxml"):
         raise Exception("please install lxml in order to validate an XMLOCEL file.")
 
+    import lxml.etree
+
     if parameters is None:
         parameters = {}
 
     xml_file = lxml.etree.parse(input_path)
     xml_validator = lxml.etree.XMLSchema(file=validation_path)
     is_valid = xml_validator.validate(xml_file)
     return is_valid
```

### Comparing `pm4py-2.7.4/pm4py/objects/org/__init__.py` & `pm4py-2.7.5/pm4py/objects/org/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/org/roles/__init__.py` & `pm4py-2.7.5/pm4py/objects/org/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/org/roles/obj.py` & `pm4py-2.7.5/pm4py/objects/org/roles/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/org/sna/__init__.py` & `pm4py-2.7.5/pm4py/objects/org/sna/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/org/sna/obj.py` & `pm4py-2.7.5/pm4py/objects/org/sna/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/inhibitor_reset/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/data_marking.py` & `pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/data_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/data_petri_nets/semantics.py` & `pm4py-2.7.5/pm4py/objects/petri_net/data_petri_nets/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/exporter/exporter.py` & `pm4py-2.7.5/pm4py/objects/petri_net/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/exporter/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/exporter/variants/pnml.py` & `pm4py-2.7.5/pm4py/objects/petri_net/exporter/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/importer/importer.py` & `pm4py-2.7.5/pm4py/objects/petri_net/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/importer/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/importer/variants/pnml.py` & `pm4py-2.7.5/pm4py/objects/petri_net/importer/variants/pnml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/inhibitor_reset/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/inhibitor_reset/semantics.py` & `pm4py-2.7.5/pm4py/objects/petri_net/inhibitor_reset/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/obj.py` & `pm4py-2.7.5/pm4py/objects/petri_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/properties.py` & `pm4py-2.7.5/pm4py/objects/petri_net/properties.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/saw_net/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/saw_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/saw_net/convert.py` & `pm4py-2.7.5/pm4py/objects/petri_net/saw_net/convert.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/saw_net/obj.py` & `pm4py-2.7.5/pm4py/objects/petri_net/saw_net/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/saw_net/semantics.py` & `pm4py-2.7.5/pm4py/objects/petri_net/saw_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/sem_interface.py` & `pm4py-2.7.5/pm4py/objects/petri_net/sem_interface.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/semantics.py` & `pm4py-2.7.5/pm4py/objects/petri_net/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/stochastic/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/stochastic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/stochastic/obj.py` & `pm4py-2.7.5/pm4py/objects/petri_net/stochastic/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/stochastic/semantics.py` & `pm4py-2.7.5/pm4py/objects/petri_net/stochastic/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/__init__.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/align_utils.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/align_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/check_soundness.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/check_soundness.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/consumption_matrix.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/consumption_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/decomposition.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/decomposition.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/embed_stochastic_map.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/embed_stochastic_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/explore_path.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/explore_path.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/final_marking.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/final_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/incidence_matrix.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/incidence_matrix.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/initial_marking.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/initial_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/murata.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/murata.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/networkx_graph.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/obj_marking.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/obj_marking.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/performance_map.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/petri_utils.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/petri_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/projection.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/projection.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/reachability_graph.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/reachability_graph.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/reduction.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/reduction.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/petri_net/utils/synchronous_product.py` & `pm4py-2.7.5/pm4py/objects/petri_net/utils/synchronous_product.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/exporter/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/exporter/exporter.py` & `pm4py-2.7.5/pm4py/objects/process_tree/exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/exporter/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/exporter/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/exporter/variants/ptml.py` & `pm4py-2.7.5/pm4py/objects/process_tree/exporter/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/importer/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/importer/importer.py` & `pm4py-2.7.5/pm4py/objects/process_tree/importer/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/importer/variants/__init__.py` & `pm4py-2.7.5/pm4py/objects/process_tree/importer/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/importer/variants/ptml.py` & `pm4py-2.7.5/pm4py/objects/process_tree/importer/variants/ptml.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/obj.py` & `pm4py-2.7.5/pm4py/objects/process_tree/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/semantics.py` & `pm4py-2.7.5/pm4py/objects/process_tree/semantics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/state.py` & `pm4py-2.7.5/pm4py/objects/process_tree/state.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/utils/__init__.py` & `pm4py-2.7.5/pm4py/statistics/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/utils/bottomup.py` & `pm4py-2.7.5/pm4py/objects/process_tree/utils/bottomup.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/utils/generic.py` & `pm4py-2.7.5/pm4py/objects/process_tree/utils/generic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/process_tree/utils/regex.py` & `pm4py-2.7.5/pm4py/objects/process_tree/utils/regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/basic_structure.py` & `pm4py-2.7.5/pm4py/objects/random_variables/basic_structure.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/constant0/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/constant0/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/constant0/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/constant0/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/exponential/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/exponential/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/exponential/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/exponential/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/gamma/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/gamma/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/gamma/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/gamma/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/lognormal/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/lognormal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/lognormal/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/lognormal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/normal/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/normal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/normal/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/normal/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/uniform/__init__.py` & `pm4py-2.7.5/pm4py/objects/random_variables/uniform/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/random_variables/uniform/random_variable.py` & `pm4py-2.7.5/pm4py/objects/random_variables/uniform/random_variable.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/stochastic_petri/__init__.py` & `pm4py-2.7.5/pm4py/objects/stochastic_petri/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/stochastic_petri/ctmc.py` & `pm4py-2.7.5/pm4py/objects/stochastic_petri/ctmc.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/stochastic_petri/tangible_reachability.py` & `pm4py-2.7.5/pm4py/objects/stochastic_petri/tangible_reachability.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/stochastic_petri/utils.py` & `pm4py-2.7.5/pm4py/objects/stochastic_petri/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/transition_system/__init__.py` & `pm4py-2.7.5/pm4py/objects/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/transition_system/constants.py` & `pm4py-2.7.5/pm4py/objects/transition_system/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/transition_system/obj.py` & `pm4py-2.7.5/pm4py/objects/transition_system/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/transition_system/utils.py` & `pm4py-2.7.5/pm4py/objects/transition_system/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/trie/__init__.py` & `pm4py-2.7.5/pm4py/objects/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/objects/trie/obj.py` & `pm4py-2.7.5/pm4py/objects/trie/obj.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/ocel.py` & `pm4py-2.7.5/pm4py/ocel.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/openai.py` & `pm4py-2.7.5/pm4py/llm.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,22 +12,48 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 
 import pandas as pd
-from pm4py.objects.log.obj import EventLog, EventStream
-from typing import Union
+from pm4py.objects.log.obj import EventLog, EventStream, Trace
+from typing import Union, Optional
 from pm4py.utils import get_properties, constants
 from pm4py.utils import __event_log_deprecation_warning
 from pm4py.objects.ocel.obj import OCEL
 from pm4py.objects.petri_net.obj import PetriNet, Marking
 
 
+def openai_query(prompt: str, api_key: Optional[str] = None, openai_model: Optional[str] = None) -> str:
+    """
+    Executes the provided prompt, obtaining the answer from the OpenAI APIs.
+
+    :param prompt: prompt that should be executed
+    :param api_key: OpenAI API key
+    :param openai_model: OpenAI model to be used (default: gpt-3.5-turbo)
+    :rtype: ``str``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        resp = pm4py.llm.openai_query('what is the result of 3+3?', api_key="sk-382393", openai_model="gpt-3.5-turbo")
+        print(resp)
+    """
+    parameters = {}
+    if api_key is not None:
+        parameters["api_key"] = api_key
+    if openai_model is not None:
+        parameters["openai_model"] = openai_model
+
+    from pm4py.algo.querying.llm.connectors import openai as perform_query
+    return perform_query.apply(prompt, parameters=parameters)
+
+
 def abstract_dfg(log_obj: Union[pd.DataFrame, EventLog, EventStream], max_len: int = constants.OPENAI_MAX_LEN, include_performance: bool = True, relative_frequency: bool = False, response_header: bool = True, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> str:
     """
     Obtains the DFG abstraction of a traditional event log
 
     :param log_obj: log object
     :param max_len: maximum length of the (string) abstraction
     :param include_performance: (boolean) includes the performance of the paths in the abstraction
@@ -39,27 +65,27 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes")
-        print(pm4py.openai.abstract_dfg(log))
+        print(pm4py.llm.abstract_dfg(log))
     """
     if type(log_obj) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
     __event_log_deprecation_warning(log_obj)
 
     parameters = get_properties(
         log_obj, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
     parameters["max_len"] = max_len
     parameters["include_performance"] = include_performance
     parameters["relative_frequency"] = relative_frequency
     parameters["response_header"] = response_header
 
-    from pm4py.algo.querying.openai import log_to_dfg_descr
+    from pm4py.algo.querying.llm.abstractions import log_to_dfg_descr
     return log_to_dfg_descr.apply(log_obj, parameters=parameters)
 
 
 def abstract_variants(log_obj: Union[pd.DataFrame, EventLog, EventStream], max_len: int = constants.OPENAI_MAX_LEN, include_performance: bool = True, relative_frequency: bool = False, response_header: bool = True, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> str:
     """
     Obtains the variants abstraction of a traditional event log
 
@@ -74,27 +100,27 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes")
-        print(pm4py.openai.abstract_variants(log))
+        print(pm4py.llm.abstract_variants(log))
     """
     if type(log_obj) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
     __event_log_deprecation_warning(log_obj)
 
     parameters = get_properties(
         log_obj, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
     parameters["max_len"] = max_len
     parameters["include_performance"] = include_performance
     parameters["relative_frequency"] = relative_frequency
     parameters["response_header"] = response_header
 
-    from pm4py.algo.querying.openai import log_to_variants_descr
+    from pm4py.algo.querying.llm.abstractions import log_to_variants_descr
     return log_to_variants_descr.apply(log_obj, parameters=parameters)
 
 
 def abstract_ocel(ocel: OCEL, include_timestamps: bool = True) -> str:
     """
     Obtains the abstraction of an object-centric event log, including the list of events and the objects of the OCEL
 
@@ -103,15 +129,15 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         ocel = pm4py.read_ocel("tests/input_data/ocel/example_log.jsonocel")
-        print(pm4py.openai.abstract_ocel(ocel))
+        print(pm4py.llm.abstract_ocel(ocel))
     """
     parameters = {}
     parameters["include_timestamps"] = include_timestamps
 
     from pm4py.algo.transformation.ocel.description import algorithm as ocel_description
     return ocel_description.apply(ocel, parameters=parameters)
 
@@ -128,22 +154,22 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         ocel = pm4py.read_ocel("tests/input_data/ocel/example_log.jsonocel")
-        print(pm4py.openai.abstract_ocel_ocdfg(ocel))
+        print(pm4py.llm.abstract_ocel_ocdfg(ocel))
     """
     parameters = {}
     parameters["include_header"] = include_header
     parameters["include_timestamps"] = include_timestamps
     parameters["max_len"] = max_len
 
-    from pm4py.algo.querying.openai import ocel_ocdfg_descr
+    from pm4py.algo.querying.llm.abstractions import ocel_ocdfg_descr
     return ocel_ocdfg_descr.apply(ocel, parameters=parameters)
 
 
 def abstract_ocel_features(ocel: OCEL, obj_type: str, include_header: bool = True, max_len: int = constants.OPENAI_MAX_LEN) -> str:
     """
     Obtains the abstraction of an object-centric event log, representing in text the features and their values.
 
@@ -154,21 +180,21 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         ocel = pm4py.read_ocel("tests/input_data/ocel/example_log.jsonocel")
-        print(pm4py.openai.abstract_ocel_ocdfg(ocel))
+        print(pm4py.llm.abstract_ocel_ocdfg(ocel))
     """
     parameters = {}
     parameters["include_header"] = include_header
     parameters["max_len"] = max_len
 
-    from pm4py.algo.querying.openai import ocel_fea_descr
+    from pm4py.algo.querying.llm.abstractions import ocel_fea_descr
     return ocel_fea_descr.apply(ocel, obj_type, parameters=parameters)
 
 
 def abstract_event_stream(log_obj: Union[pd.DataFrame, EventLog, EventStream], max_len: int = constants.OPENAI_MAX_LEN, response_header: bool = True, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> str:
     """
     Obtains the event stream abstraction of a traditional event log
 
@@ -181,25 +207,25 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes")
-        print(pm4py.openai.abstract_event_stream(log))
+        print(pm4py.llm.abstract_event_stream(log))
     """
     if type(log_obj) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
     __event_log_deprecation_warning(log_obj)
 
     parameters = get_properties(
         log_obj, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
     parameters["max_len"] = max_len
     parameters["response_header"] = response_header
 
-    from pm4py.algo.querying.openai import stream_to_descr
+    from pm4py.algo.querying.llm.abstractions import stream_to_descr
     return stream_to_descr.apply(log_obj, parameters=parameters)
 
 
 def abstract_petri_net(net: PetriNet, im: Marking, fm: Marking, response_header: bool = True) -> str:
     """
     Obtain an abstraction of a Petri net
 
@@ -210,20 +236,20 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         net, im, fm = pm4py.read_pnml('tests/input_data/running-example.pnml')
-        print(pm4py.openai.abstract_petri_net(net, im, fm))
+        print(pm4py.llm.abstract_petri_net(net, im, fm))
     """
     parameters = {}
     parameters["response_header"] = response_header
 
-    from pm4py.algo.querying.openai import net_to_descr
+    from pm4py.algo.querying.llm.abstractions import net_to_descr
     return net_to_descr.apply(net, im, fm, parameters=parameters)
 
 
 def abstract_log_attributes(log_obj: Union[pd.DataFrame, EventLog, EventStream], max_len: int = constants.OPENAI_MAX_LEN, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> str:
     """
     Abstracts the attributes of a log (reporting their name, their type, and the top values)
 
@@ -235,18 +261,102 @@
     :rtype: ``str``
 
     .. code-block:: python3
 
         import pm4py
 
         log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes")
-        print(pm4py.openai.abstract_log_attributes(log))
+        print(pm4py.llm.abstract_log_attributes(log))
     """
     if type(log_obj) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
     __event_log_deprecation_warning(log_obj)
 
     parameters = get_properties(
         log_obj, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
     parameters["max_len"] = max_len
 
-    from pm4py.algo.querying.openai import log_to_cols_descr
+    from pm4py.algo.querying.llm.abstractions import log_to_cols_descr
     return log_to_cols_descr.apply(log_obj, parameters=parameters)
+
+
+def abstract_log_features(log_obj: Union[pd.DataFrame, EventLog, EventStream], max_len: int = constants.OPENAI_MAX_LEN, include_header: bool = True, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name") -> str:
+    """
+    Abstracts the machine learning features obtained from a log (reporting the top features until the desired length is obtained)
+
+    :param log_obj: log object
+    :param max_len: maximum length of the (string) abstraction
+    :param activity_key: the column to be used as activity
+    :param timestamp_key: the column to be used as timestamp
+    :param case_id_key: the column to be used as case identifier
+    :rtype: ``str``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes")
+        print(pm4py.llm.abstract_log_features(log))
+    """
+    if type(log_obj) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
+    __event_log_deprecation_warning(log_obj)
+
+    parameters = get_properties(
+        log_obj, activity_key=activity_key, timestamp_key=timestamp_key, case_id_key=case_id_key)
+    parameters["max_len"] = max_len
+    parameters["include_header"] = include_header
+
+    from pm4py.algo.querying.llm.abstractions import log_to_fea_descr
+    return log_to_fea_descr.apply(log_obj, parameters=parameters)
+
+
+def abstract_case(case: Trace, include_case_attributes: bool = True, include_event_attributes: bool = True, include_timestamp: bool = True, include_header: bool = True, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp") -> str:
+    """
+    Textually abstracts a case
+
+    :param case: case object
+    :param include_case_attributes: (boolean) include or not the attributes at the case level
+    :param include_event_attributes: (boolean) include or not the attributes at the event level
+    :param include_timestamp: (boolean) include or not the event timestamp in the abstraction
+    :param include_header: (boolean) includes the header of the response
+    :param activity_key: the column to be used as activity
+    :param timestamp_key: the column to be used as timestamp
+    :rtype: ``str``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes", return_legacy_log_object=True)
+        print(pm4py.llm.abstract_case(log[0]))
+    """
+    parameters = {}
+    parameters["include_case_attributes"] = include_case_attributes
+    parameters["include_event_attributes"] = include_event_attributes
+    parameters["include_timestamp"] = include_timestamp
+    parameters["include_header"] = include_header
+    parameters[constants.PARAMETER_CONSTANT_ACTIVITY_KEY] = activity_key
+    parameters[constants.PARAMETER_CONSTANT_TIMESTAMP_KEY] = timestamp_key
+
+    from pm4py.algo.querying.llm.abstractions import case_to_descr
+    return case_to_descr.apply(case, parameters=parameters)
+
+
+def abstract_log_skeleton(log_skeleton, include_header: bool = True) -> str:
+    """
+    Textually abstracts a log skeleton process model
+
+    :param log_skeleton: log skeleton
+    :param include_header: (boolean) includes the header of the response
+    :rtype: ``str``
+
+    .. code-block:: python3
+
+        import pm4py
+
+        log = pm4py.read_xes("tests/input_data/roadtraffic100traces.xes", return_legacy_log_object=True)
+        log_ske = pm4py.discover_log_skeleton(log)
+        print(pm4py.llm.abstract_log_skeleton(log_ske))
+    """
+    parameters = {}
+
+    from pm4py.algo.querying.llm.abstractions import logske_to_descr
+    return logske_to_descr.apply(log_skeleton, parameters=parameters)
```

### Comparing `pm4py-2.7.4/pm4py/org.py` & `pm4py-2.7.5/pm4py/org.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/privacy.py` & `pm4py-2.7.5/pm4py/privacy.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/read.py` & `pm4py-2.7.5/pm4py/read.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/sim.py` & `pm4py-2.7.5/pm4py/sim.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/__init__.py` & `pm4py-2.7.5/pm4py/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/__init__.py` & `pm4py-2.7.5/pm4py/statistics/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/common/__init__.py` & `pm4py-2.7.5/pm4py/statistics/attributes/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/common/get.py` & `pm4py-2.7.5/pm4py/statistics/attributes/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/attributes/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/log/get.py` & `pm4py-2.7.5/pm4py/statistics/attributes/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/log/select.py` & `pm4py-2.7.5/pm4py/statistics/attributes/log/select.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/attributes/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/attributes/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/attributes/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/concurrent_activities/__init__.py` & `pm4py-2.7.5/pm4py/statistics/concurrent_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/concurrent_activities/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/concurrent_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/concurrent_activities/log/get.py` & `pm4py-2.7.5/pm4py/statistics/concurrent_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/concurrent_activities/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/concurrent_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/concurrent_activities/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/concurrent_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/__init__.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/common/__init__.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/common/get.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/log/get.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/end_activities/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/end_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/eventually_follows/__init__.py` & `pm4py-2.7.5/pm4py/statistics/eventually_follows/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/eventually_follows/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/eventually_follows/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/eventually_follows/log/get.py` & `pm4py-2.7.5/pm4py/statistics/eventually_follows/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/eventually_follows/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/eventually_follows/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/eventually_follows/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/eventually_follows/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/__init__.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/act_ot_dependent.py` & `pm4py-2.7.5/pm4py/statistics/ocel/act_ot_dependent.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/act_utils.py` & `pm4py-2.7.5/pm4py/statistics/ocel/act_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/edge_metrics.py` & `pm4py-2.7.5/pm4py/statistics/ocel/edge_metrics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/objects_ot_count.py` & `pm4py-2.7.5/pm4py/statistics/ocel/objects_ot_count.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/ocel/ot_activities.py` & `pm4py-2.7.5/pm4py/statistics/ocel/ot_activities.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/cases/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/cases/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/cases/log/get.py` & `pm4py-2.7.5/pm4py/statistics/overlap/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/cases/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/cases/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/overlap/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/interval_events/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/interval_events/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/interval_events/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/interval_events/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/interval_events/log/get.py` & `pm4py-2.7.5/pm4py/statistics/overlap/interval_events/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/interval_events/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/interval_events/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/interval_events/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/overlap/interval_events/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/utils/__init__.py` & `pm4py-2.7.5/pm4py/statistics/overlap/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/overlap/utils/compute.py` & `pm4py-2.7.5/pm4py/statistics/overlap/utils/compute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/__init__.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/algorithm.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/__init__.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/post.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/pre.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/log/variants/prepost.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/log/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/algorithm.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/__init__.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/post.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/post.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/pre.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/pre.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/passed_time/pandas/variants/prepost.py` & `pm4py-2.7.5/pm4py/statistics/passed_time/pandas/variants/prepost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/cases/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/cases/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/cases/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/cases/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/cases/log/get.py` & `pm4py-2.7.5/pm4py/statistics/rework/cases/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/cases/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/cases/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/cases/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/rework/cases/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/log/get.py` & `pm4py-2.7.5/pm4py/statistics/rework/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/rework/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/rework/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/rework/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/sojourn_time/__init__.py` & `pm4py-2.7.5/pm4py/statistics/sojourn_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/sojourn_time/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/sojourn_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/sojourn_time/log/get.py` & `pm4py-2.7.5/pm4py/statistics/sojourn_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/sojourn_time/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/sojourn_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/sojourn_time/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/sojourn_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/__init__.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/common/__init__.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/common/get.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/common/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/log/get.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/start_activities/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/start_activities/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/log/get.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/util/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/cycle_time/util/compute.py` & `pm4py-2.7.5/pm4py/statistics/traces/cycle_time/util/compute.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/common/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/common/case_duration.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/common/case_duration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/log/case_arrival.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/log/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/log/case_statistics.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/log/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/case_arrival.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/case_arrival.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/traces/generic/pandas/case_statistics.py` & `pm4py-2.7.5/pm4py/statistics/traces/generic/pandas/case_statistics.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/util/__init__.py` & `pm4py-2.7.5/pm4py/statistics/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/util/times_bipartite_matching.py` & `pm4py-2.7.5/pm4py/statistics/util/times_bipartite_matching.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/variants/__init__.py` & `pm4py-2.7.5/pm4py/statistics/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/variants/log/__init__.py` & `pm4py-2.7.5/pm4py/statistics/variants/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/variants/log/get.py` & `pm4py-2.7.5/pm4py/statistics/variants/log/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/variants/pandas/__init__.py` & `pm4py-2.7.5/pm4py/statistics/variants/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/statistics/variants/pandas/get.py` & `pm4py-2.7.5/pm4py/statistics/variants/pandas/get.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/stats.py` & `pm4py-2.7.5/pm4py/stats.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/__init__.py` & `pm4py-2.7.5/pm4py/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/algorithm.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/footprints/variants/classic.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/footprints/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/algorithm.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/tbr/variants/classic.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/tbr/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/algorithm.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/conformance/temporal/variants/classic.py` & `pm4py-2.7.5/pm4py/streaming/algo/conformance/temporal/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/discovery/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/algorithm.py` & `pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/algorithm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/discovery/dfg/variants/frequency.py` & `pm4py-2.7.5/pm4py/streaming/algo/discovery/dfg/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/algo/interface.py` & `pm4py-2.7.5/pm4py/streaming/algo/interface.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/conversion/__init__.py` & `pm4py-2.7.5/pm4py/streaming/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/conversion/from_pandas.py` & `pm4py-2.7.5/pm4py/streaming/conversion/from_pandas.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/conversion/ocel_flatts_distributor.py` & `pm4py-2.7.5/pm4py/streaming/conversion/ocel_flatts_distributor.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/__init__.py` & `pm4py-2.7.5/pm4py/streaming/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/csv/__init__.py` & `pm4py-2.7.5/pm4py/streaming/importer/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/csv/importer.py` & `pm4py-2.7.5/pm4py/streaming/importer/csv/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/csv/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/importer/csv/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/csv/variants/csv_event_stream.py` & `pm4py-2.7.5/pm4py/streaming/importer/csv/variants/csv_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/xes/__init__.py` & `pm4py-2.7.5/pm4py/streaming/importer/xes/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/xes/importer.py` & `pm4py-2.7.5/pm4py/streaming/importer/xes/importer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/xes/variants/__init__.py` & `pm4py-2.7.5/pm4py/streaming/importer/xes/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/xes/variants/xes_event_stream.py` & `pm4py-2.7.5/pm4py/streaming/importer/xes/variants/xes_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/importer/xes/variants/xes_trace_stream.py` & `pm4py-2.7.5/pm4py/streaming/importer/xes/variants/xes_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/stream/__init__.py` & `pm4py-2.7.5/pm4py/streaming/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/stream/live_event_stream.py` & `pm4py-2.7.5/pm4py/streaming/stream/live_event_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/stream/live_trace_stream.py` & `pm4py-2.7.5/pm4py/streaming/stream/live_trace_stream.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/__init__.py` & `pm4py-2.7.5/pm4py/streaming/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/__init__.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/generator.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/generator.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/versions/__init__.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/versions/classic.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/versions/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/versions/redis.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/versions/redis.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/dictio/versions/thread_safe.py` & `pm4py-2.7.5/pm4py/streaming/util/dictio/versions/thread_safe.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/event_stream_printer.py` & `pm4py-2.7.5/pm4py/streaming/util/event_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/streaming/util/trace_stream_printer.py` & `pm4py-2.7.5/pm4py/streaming/util/trace_stream_printer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/__init__.py` & `pm4py-2.7.5/pm4py/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/business_hours.py` & `pm4py-2.7.5/pm4py/util/business_hours.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/colors.py` & `pm4py-2.7.5/pm4py/util/colors.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/compression/__init__.py` & `pm4py-2.7.5/pm4py/util/compression/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/compression/dtypes.py` & `pm4py-2.7.5/pm4py/util/compression/dtypes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/compression/util.py` & `pm4py-2.7.5/pm4py/util/compression/util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/constants.py` & `pm4py-2.7.5/pm4py/util/constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/__init__.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/parser.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/parser.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/variants/__init__.py` & `pm4py-2.7.5/pm4py/util/lp/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/variants/cs8601.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/variants/cs8601.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/variants/dummy.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/variants/dummy.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/dt_parsing/variants/strpfromiso.py` & `pm4py-2.7.5/pm4py/util/dt_parsing/variants/strpfromiso.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/exec_utils.py` & `pm4py-2.7.5/pm4py/util/exec_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/__init__.py` & `pm4py-2.7.5/pm4py/util/lp/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/solver.py` & `pm4py-2.7.5/pm4py/util/lp/solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/util/__init__.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/__init__.py` & `pm4py-2.7.5/pm4py/util/lp/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver.py` & `pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align.py` & `pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py` & `pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align_arm.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py` & `pm4py-2.7.5/pm4py/util/lp/variants/cvxopt_solver_custom_align_ilp.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/ortools_solver.py` & `pm4py-2.7.5/pm4py/util/lp/variants/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/pulp_solver.py` & `pm4py-2.7.5/pm4py/util/lp/variants/pulp_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/lp/variants/scipy_solver.py` & `pm4py-2.7.5/pm4py/util/lp/variants/scipy_solver.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/pandas_utils.py` & `pm4py-2.7.5/pm4py/util/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/points_subset.py` & `pm4py-2.7.5/pm4py/util/points_subset.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/regex.py` & `pm4py-2.7.5/pm4py/util/regex.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/string_distance.py` & `pm4py-2.7.5/pm4py/util/string_distance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/typing.py` & `pm4py-2.7.5/pm4py/util/typing.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/variants_util.py` & `pm4py-2.7.5/pm4py/util/variants_util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/vis_utils.py` & `pm4py-2.7.5/pm4py/util/vis_utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/util/xes_constants.py` & `pm4py-2.7.5/pm4py/util/xes_constants.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/utils.py` & `pm4py-2.7.5/pm4py/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,21 @@
         if xes_constants.DEFAULT_TIMESTAMP_KEY in df.columns:
             del df[xes_constants.DEFAULT_TIMESTAMP_KEY]
         df[xes_constants.DEFAULT_TIMESTAMP_KEY] = df[timestamp_key]
     # makes sure that the timestamps column are of timestamp type
     df = dataframe_utils.convert_timestamp_columns_in_df(df, timest_format=timest_format)
     # drop NaN(s) in the main columns (case ID, activity, timestamp) to ensure functioning of the
     # algorithms
+    prev_length = len(df)
     df = df.dropna(subset={constants.CASE_CONCEPT_NAME, xes_constants.DEFAULT_NAME_KEY,
                            xes_constants.DEFAULT_TIMESTAMP_KEY}, how="any")
+
+    if len(df) < prev_length:
+        warnings.warn("Some rows of the Pandas data frame have been removed because of empty case IDs, activity labels, or timestamps to ensure the correct functioning of PM4Py's algorithms.")
+
     # make sure the case ID column is of string type
     df[constants.CASE_CONCEPT_NAME] = df[constants.CASE_CONCEPT_NAME].astype("string")
     # make sure the activity column is of string type
     df[xes_constants.DEFAULT_NAME_KEY] = df[xes_constants.DEFAULT_NAME_KEY].astype("string")
     # set an index column
     df = pandas_utils.insert_index(df, INDEX_COLUMN, copy_dataframe=False)
     # sorts the dataframe
@@ -372,15 +377,15 @@
             activitiess.append(act)
             timestamps.append(datetime.datetime.fromtimestamp(this_timest))
             this_timest = this_timest + 1
 
     return pd.DataFrame({case_id_key: cases, activity_key: activitiess, timestamp_key: timestamps})
 
 
-def project_on_event_attribute(log: Union[EventLog, pd.DataFrame], attribute_key=xes_constants.DEFAULT_NAME_KEY) -> \
+def project_on_event_attribute(log: Union[EventLog, pd.DataFrame], attribute_key=xes_constants.DEFAULT_NAME_KEY, case_id_key=None) -> \
 List[List[str]]:
     """
     Project the event log on a specified event attribute. The result is a list, containing a list for each case:
     all the cases are transformed to list of values for the specified attribute.
 
     Example:
 
@@ -391,14 +396,15 @@
     ['register request', 'examine thoroughly', 'check ticket', 'decide', 'reject request'],
     ['register request', 'examine casually', 'check ticket', 'decide', 'pay compensation'],
     ['register request', 'examine casually', 'check ticket', 'decide', 'reinitiate request', 'check ticket', 'examine casually', 'decide', 'reinitiate request', 'examine casually', 'check ticket', 'decide', 'reject request'],
     ['register request', 'check ticket', 'examine thoroughly', 'decide', 'reject request']]
 
     :param log: Event log / Pandas dataframe
     :param attribute_key: The attribute to be used
+    :param case_id_key: The attribute to be used as case identifier
     :rtype: ``List[List[str]]``
 
     .. code-block:: python3
 
         import pm4py
 
         list_list_activities = pm4py.project_on_event_attribute(dataframe, 'concept:name')
@@ -406,15 +412,18 @@
     if type(log) not in [pd.DataFrame, EventLog, EventStream]: raise Exception("the method can be applied only to a traditional event log!")
     __event_log_deprecation_warning(log)
 
     output = []
     if check_is_pandas_dataframe(log):
         check_pandas_dataframe_columns(log)
         from pm4py.streaming.conversion import from_pandas
-        it = from_pandas.apply(log, parameters={from_pandas.Parameters.ACTIVITY_KEY: attribute_key})
+        parameters = {from_pandas.Parameters.ACTIVITY_KEY: attribute_key}
+        if case_id_key is not None:
+            parameters[from_pandas.Parameters.CASE_ID_KEY] = case_id_key
+        it = from_pandas.apply(log, parameters=parameters)
         for trace in it:
             output.append([x[xes_constants.DEFAULT_NAME_KEY] if xes_constants.DEFAULT_NAME_KEY is not None else None for x in trace])
     else:
         for trace in log:
             output.append([x[attribute_key] if attribute_key is not None else None for x in trace])
     return output
```

### Comparing `pm4py-2.7.4/pm4py/vis.py` & `pm4py-2.7.5/pm4py/vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
 __doc__ = """
 The ``pm4py.vis`` module contains the visualizations offered in ``pm4py``
 """
 
 import os
+import sys
 from typing import Optional
 from typing import Union, List, Dict, Any, Tuple, Set
 
 import pandas as pd
 
 from pm4py.objects.bpmn.obj import BPMN
 from pm4py.objects.heuristics_net.obj import HeuristicsNet
@@ -38,63 +39,65 @@
 from pm4py.util import constants
 
 import deprecation
 
 
 def view_petri_net(petri_net: PetriNet, initial_marking: Optional[Marking] = None,
                    final_marking: Optional[Marking] = None, format: str = constants.DEFAULT_FORMAT_GVIZ_VIEW, bgcolor: str = "white",
-                   decorations: Dict[Any, Any] = None):
+                   decorations: Dict[Any, Any] = None, debug: bool = False):
     """
     Views a (composite) Petri net
 
     :param petri_net: Petri net
     :param initial_marking: Initial marking
     :param final_marking: Final marking
     :param format: Format of the output picture (if html is provided, GraphvizJS is used to render the visualization in an HTML page)
     :param bgcolor: Background color of the visualization (default: white)
     :param decorations: Decorations (color, label) associated to the elements of the Petri net
+    :param debug: Boolean enabling/disabling the debug mode (show place and transition's names)
 
     .. code-block:: python3
 
         import pm4py
 
         net, im, fm = pm4py.discover_petri_net_inductive(dataframe, activity_key='concept:name', case_id_key='case:concept:name', timestamp_key='time:timestamp')
         pm4py.view_petri_net(net, im, fm, format='svg')
     """
     format = str(format).lower()
     from pm4py.visualization.petri_net import visualizer as pn_visualizer
     gviz = pn_visualizer.apply(petri_net, initial_marking, final_marking,
-                               parameters={pn_visualizer.Variants.WO_DECORATION.value.Parameters.FORMAT: format, "bgcolor": bgcolor, "decorations": decorations})
+                               parameters={pn_visualizer.Variants.WO_DECORATION.value.Parameters.FORMAT: format, "bgcolor": bgcolor, "decorations": decorations, "debug": debug})
     pn_visualizer.view(gviz)
 
 
 def save_vis_petri_net(petri_net: PetriNet, initial_marking: Marking, final_marking: Marking, file_path: str, bgcolor: str = "white",
-                   decorations: Dict[Any, Any] = None):
+                   decorations: Dict[Any, Any] = None, debug: bool = False):
     """
     Saves a Petri net visualization to a file
 
     :param petri_net: Petri net
     :param initial_marking: Initial marking
     :param final_marking: Final marking
     :param file_path: Destination path
     :param bgcolor: Background color of the visualization (default: white)
     :param decorations: Decorations (color, label) associated to the elements of the Petri net
+    :param debug: Boolean enabling/disabling the debug mode (show place and transition's names)
 
     .. code-block:: python3
 
         import pm4py
 
         net, im, fm = pm4py.discover_petri_net_inductive(dataframe, activity_key='concept:name', case_id_key='case:concept:name', timestamp_key='time:timestamp')
         pm4py.save_vis_petri_net(net, im, fm, 'petri_net.png')
     """
     file_path = str(file_path)
     format = os.path.splitext(file_path)[1][1:].lower()
     from pm4py.visualization.petri_net import visualizer as pn_visualizer
     gviz = pn_visualizer.apply(petri_net, initial_marking, final_marking,
-                               parameters={pn_visualizer.Variants.WO_DECORATION.value.Parameters.FORMAT: format, "bgcolor": bgcolor, "decorations": decorations})
+                               parameters={pn_visualizer.Variants.WO_DECORATION.value.Parameters.FORMAT: format, "bgcolor": bgcolor, "decorations": decorations, "debug": debug})
     pn_visualizer.save(gviz, file_path)
 
 
 def view_performance_dfg(dfg: dict, start_activities: dict, end_activities: dict, format: str = constants.DEFAULT_FORMAT_GVIZ_VIEW,
                          aggregation_measure="mean", bgcolor: str = "white"):
     """
     Views a performance DFG
@@ -157,23 +160,24 @@
     parameters[dfg_parameters.END_ACTIVITIES] = end_activities
     parameters[dfg_parameters.AGGREGATION_MEASURE] = aggregation_measure
     parameters["bgcolor"] = bgcolor
     gviz = dfg_perf_visualizer.apply(dfg, parameters=parameters)
     dfg_visualizer.save(gviz, file_path)
 
 
-def view_dfg(dfg: dict, start_activities: dict, end_activities: dict, format: str = constants.DEFAULT_FORMAT_GVIZ_VIEW, bgcolor: str = "white"):
+def view_dfg(dfg: dict, start_activities: dict, end_activities: dict, format: str = constants.DEFAULT_FORMAT_GVIZ_VIEW, bgcolor: str = "white", max_num_edges: int = sys.maxsize):
     """
     Views a (composite) DFG
 
     :param dfg: DFG object
     :param start_activities: Start activities
     :param end_activities: End activities
     :param format: Format of the output picture (if html is provided, GraphvizJS is used to render the visualization in an HTML page)
     :param bgcolor: Background color of the visualization (default: white)
+    :param max_num_edges: maximum number of edges to represent in the graph
 
     .. code-block:: python3
 
         import pm4py
 
         dfg, start_activities, end_activities = pm4py.discover_dfg(dataframe, case_id_key='case:concept:name', activity_key='concept:name', timestamp_key='time:timestamp')
         pm4py.view_dfg(dfg, start_activities, end_activities, format='svg')
@@ -182,28 +186,30 @@
     from pm4py.visualization.dfg import visualizer as dfg_visualizer
     dfg_parameters = dfg_visualizer.Variants.FREQUENCY.value.Parameters
     parameters = {}
     parameters[dfg_parameters.FORMAT] = format
     parameters[dfg_parameters.START_ACTIVITIES] = start_activities
     parameters[dfg_parameters.END_ACTIVITIES] = end_activities
     parameters["bgcolor"] = bgcolor
+    parameters["maxNoOfEdgesInDiagram"] = max_num_edges
     gviz = dfg_visualizer.apply(dfg, variant=dfg_visualizer.Variants.FREQUENCY,
                                 parameters=parameters)
     dfg_visualizer.view(gviz)
 
 
-def save_vis_dfg(dfg: dict, start_activities: dict, end_activities: dict, file_path: str, bgcolor: str = "white"):
+def save_vis_dfg(dfg: dict, start_activities: dict, end_activities: dict, file_path: str, bgcolor: str = "white", max_num_edges: int = sys.maxsize):
     """
     Saves a DFG visualization to a file
 
     :param dfg: DFG object
     :param start_activities: Start activities
     :param end_activities: End activities
     :param file_path: Destination path
     :param bgcolor: Background color of the visualization (default: white)
+    :param max_num_edges: maximum number of edges to represent in the graph
 
     .. code-block:: python3
 
         import pm4py
 
         dfg, start_activities, end_activities = pm4py.discover_dfg(dataframe, case_id_key='case:concept:name', activity_key='concept:name', timestamp_key='time:timestamp')
         pm4py.save_vis_dfg(dfg, start_activities, end_activities, 'dfg.png')
@@ -213,14 +219,15 @@
     from pm4py.visualization.dfg import visualizer as dfg_visualizer
     dfg_parameters = dfg_visualizer.Variants.FREQUENCY.value.Parameters
     parameters = {}
     parameters[dfg_parameters.FORMAT] = format
     parameters[dfg_parameters.START_ACTIVITIES] = start_activities
     parameters[dfg_parameters.END_ACTIVITIES] = end_activities
     parameters["bgcolor"] = bgcolor
+    parameters["maxNoOfEdgesInDiagram"] = max_num_edges
     gviz = dfg_visualizer.apply(dfg, variant=dfg_visualizer.Variants.FREQUENCY,
                                 parameters=parameters)
     dfg_visualizer.save(gviz, file_path)
 
 
 def view_process_tree(tree: ProcessTree, format: str = constants.DEFAULT_FORMAT_GVIZ_VIEW, bgcolor: str = "white"):
     """
@@ -374,15 +381,14 @@
         log = sorting.sort_timestamp(log, xes_constants.DEFAULT_TIMESTAMP_KEY)
         for index, trace in enumerate(log):
             trace.attributes["@@index"] = index
         attributes = ["time:timestamp", "case:@@index", "concept:name"]
     return log, attributes
 
 
-@deprecation.deprecated(deprecated_in="2.3.0", removed_in="3.0.0", details="the dotted chart visualization will be removed in a future release.")
 def view_dotted_chart(log: Union[EventLog, pd.DataFrame], format: str = "png", attributes=None, bgcolor: str = "white", show_legend: bool = True):
     """
     Displays the dotted chart
 
     The dotted chart is a classic visualization of the events inside an event log across different dimensions. Each event of the event log is corresponding to a point. The dimensions are projected on a graph having:
     - X axis: the values of the first dimension are represented there.
     - Y-axis: the values of the second dimension are represented there.
@@ -427,15 +433,14 @@
     parameters["show_legend"] = show_legend
 
     from pm4py.visualization.dotted_chart import visualizer as dotted_chart_visualizer
     gviz = dotted_chart_visualizer.apply(log, attributes, parameters=parameters)
     dotted_chart_visualizer.view(gviz)
 
 
-@deprecation.deprecated(deprecated_in="2.3.0", removed_in="3.0.0", details="the dotted chart visualization will be removed in a future release.")
 def save_vis_dotted_chart(log: Union[EventLog, pd.DataFrame], file_path: str, attributes=None, bgcolor: str = "white", show_legend: bool = True):
     """
     Saves the visualization of the dotted chart
 
     The dotted chart is a classic visualization of the events inside an event log across different dimensions. Each event of the event log is corresponding to a point. The dimensions are projected on a graph having:
     - X axis: the values of the first dimension are represented there.
     - Y-axis: the values of the second dimension are represented there.
@@ -671,15 +676,14 @@
     format = os.path.splitext(file_path)[1][1:].lower()
     from pm4py.visualization.graphs import visualizer as graphs_visualizer
     graph_vis = graphs_visualizer.apply(graph[0], graph[1], variant=graphs_visualizer.Variants.DATES,
                                         parameters={"format": format})
     graphs_visualizer.save(graph_vis, file_path)
 
 
-@deprecation.deprecated(deprecated_in="2.3.0", removed_in="3.0.0", details="the performance spectrum visualization will be removed in a future release.")
 def view_performance_spectrum(log: Union[EventLog, pd.DataFrame], activities: List[str], format: str = "png", activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name", bgcolor: str = "white"):
     """
     Displays the performance spectrum
 
     The performance spectrum is a novel visualization of the performance of the process of the time elapsed between different activities in the process executions. The performance spectrum has initially been described in:
 
     Denisov, Vadim, et al. "The Performance Spectrum Miner: Visual Analytics for Fine-Grained Performance Analysis of Processes." BPM (Dissertation/Demos/Industry). 2018.
@@ -713,15 +717,14 @@
     perf_spectrum = performance_spectrum.apply(log, activities, parameters=properties)
     from pm4py.visualization.performance_spectrum import visualizer as perf_spectrum_visualizer
     from pm4py.visualization.performance_spectrum.variants import neato
     gviz = perf_spectrum_visualizer.apply(perf_spectrum, parameters={neato.Parameters.FORMAT.value: format, "bgcolor": bgcolor})
     perf_spectrum_visualizer.view(gviz)
 
 
-@deprecation.deprecated(deprecated_in="2.3.0", removed_in="3.0.0", details="the performance spectrum visualization will be removed in a future release.")
 def save_vis_performance_spectrum(log: Union[EventLog, pd.DataFrame], activities: List[str], file_path: str, activity_key: str = "concept:name", timestamp_key: str = "time:timestamp", case_id_key: str = "case:concept:name", bgcolor: str = "white"):
     """
     Saves the visualization of the performance spectrum to a file
 
     The performance spectrum is a novel visualization of the performance of the process of the time elapsed between different activities in the process executions. The performance spectrum has initially been described in:
 
     Denisov, Vadim, et al. "The Performance Spectrum Miner: Visual Analytics for Fine-Grained Performance Analysis of Processes." BPM (Dissertation/Demos/Industry). 2018.
```

### Comparing `pm4py-2.7.4/pm4py/visualization/__init__.py` & `pm4py-2.7.5/pm4py/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/align_table/__init__.py` & `pm4py-2.7.5/pm4py/visualization/align_table/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/align_table/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/align_table/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/align_table/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/align_table/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/align_table/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/align_table/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/bpmn/__init__.py` & `pm4py-2.7.5/pm4py/visualization/bpmn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/bpmn/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/bpmn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/bpmn/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/bpmn/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/bpmn/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/bpmn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/__init__.py` & `pm4py-2.7.5/pm4py/visualization/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/dot_util.py` & `pm4py-2.7.5/pm4py/visualization/common/dot_util.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/gview.py` & `pm4py-2.7.5/pm4py/visualization/common/gview.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/html.py` & `pm4py-2.7.5/pm4py/visualization/common/html.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/save.py` & `pm4py-2.7.5/pm4py/visualization/common/save.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/svg_pos_parser.py` & `pm4py-2.7.5/pm4py/visualization/common/svg_pos_parser.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/utils.py` & `pm4py-2.7.5/pm4py/visualization/common/utils.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/common/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/common/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/__init__.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/util/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/object_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/util/dt_to_string.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/util/dt_to_string.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/decisiontree/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/decisiontree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/__init__.py` & `pm4py-2.7.5/pm4py/visualization/dfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/util/__init__.py` & `pm4py-2.7.5/pm4py/visualization/dfg/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/util/dfg_gviz.py` & `pm4py-2.7.5/pm4py/visualization/dfg/util/dfg_gviz.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,20 +183,18 @@
     dfg_keys = list(dfg.keys())
     for edge in dfg_keys:
         if edge not in dfg_allowed_keys:
             del dfg[edge]
 
     # calculate edges penwidth
     penwidth = assign_penwidth_edges(dfg)
-    activities_in_dfg = set()
+
     activities_count_int = copy(activities_count)
 
-    for edge in dfg:
-        activities_in_dfg.add(edge[0])
-        activities_in_dfg.add(edge[1])
+    activities_in_dfg = set(activities_count)
 
     # assign attributes color
     if measure == "frequency":
         activities_color = get_activities_color(activities_count_int)
     else:
         activities_color = get_activities_color_soj_time(soj_time)
```

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/dfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/variants/cost.py` & `pm4py-2.7.5/pm4py/visualization/dfg/variants/cost.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/variants/frequency.py` & `pm4py-2.7.5/pm4py/visualization/dfg/variants/frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,15 +70,21 @@
     activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes.DEFAULT_NAME_KEY)
     image_format = exec_utils.get_param_value(Parameters.FORMAT, parameters, "png")
     max_no_of_edges_in_diagram = exec_utils.get_param_value(Parameters.MAX_NO_EDGES_IN_DIAGRAM, parameters, 100000)
     start_activities = exec_utils.get_param_value(Parameters.START_ACTIVITIES, parameters, {})
     end_activities = exec_utils.get_param_value(Parameters.END_ACTIVITIES, parameters, {})
     font_size = exec_utils.get_param_value(Parameters.FONT_SIZE, parameters, 12)
     font_size = str(font_size)
-    activities = dfg_utils.get_activities_from_dfg(dfg)
+
+    if start_activities is None:
+        start_activities = dict()
+    if end_activities is None:
+        end_activities = dict()
+    activities = sorted(list(set(dfg_utils.get_activities_from_dfg(dfg)).union(set(start_activities)).union(set(end_activities))))
+
     bgcolor = exec_utils.get_param_value(Parameters.BGCOLOR, parameters, constants.DEFAULT_BGCOLOR)
     stat_locale = exec_utils.get_param_value(Parameters.STAT_LOCALE, parameters, {})
 
     if activities_count is None:
         if log is not None:
             activities_count = attr_get.get_attribute_values(log, activity_key, parameters=parameters)
         else:
```

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/variants/performance.py` & `pm4py-2.7.5/pm4py/visualization/dfg/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dfg/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/dfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dotted_chart/__init__.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,12 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.visualization.dotted_chart import visualizer, variants
-
-import warnings
-
-warnings.warn("The dotted_chart visualizer will be removed in a future release.")
+from pm4py.visualization.petri_net.common import visualize
```

### Comparing `pm4py-2.7.4/pm4py/visualization/dotted_chart/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/dotted_chart/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/dotted_chart/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/dotted_chart/variants/classic.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
     for p in points_list:
         coord_x = corr_dict[0][p[0]]
         coord_y = corr_dict[1][p[1]]
         color = color_dict[p[2]] if color_dict is not None else "blue"
         n_id = "n" + str(uuid.uuid4()).replace("-", "") + "e"
         lines.append(
-            "%s [label=\"\", shape=circle,  width=\"%.10fpx\", height=\"%.10fpx\", pos=\"%.10f,%.10f!\", fontsize=\"6pt\", style=\"filled\", fillcolor=\"%s\"];" % (
+            "%s [label=\"\", shape=circle,  width=\"%.10fpx\", height=\"%.10fpx\", pos=\"%.10f,%.10f!\", fontsize=\"6pt\", style=\"filled\", fillcolor=\"%s\", penwidth=0];" % (
                 n_id, dot_size, dot_size, coord_x * x_length, coord_y * y_length, color))
 
     if color_dict is not None and show_legend:
         lines.append(
             "Legend [label=\"legend (attribute: %s)\", shape=none, width=\"0px\", height=\"0px\", pos=\"0,-%d!\"]" % (
                 attributes[2], 1*layout_ext_multiplier))
         row = -1
```

### Comparing `pm4py-2.7.4/pm4py/visualization/dotted_chart/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/dotted_chart/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/__init__.py` & `pm4py-2.7.5/pm4py/visualization/footprints/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/footprints/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/variants/comparison.py` & `pm4py-2.7.5/pm4py/visualization/footprints/variants/comparison.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/variants/comparison_symmetric.py` & `pm4py-2.7.5/pm4py/visualization/footprints/variants/comparison_symmetric.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/variants/single.py` & `pm4py-2.7.5/pm4py/visualization/footprints/variants/single.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/footprints/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/footprints/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/__init__.py` & `pm4py-2.7.5/pm4py/visualization/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/util/__init__.py` & `pm4py-2.7.5/pm4py/visualization/graphs/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/util/common.py` & `pm4py-2.7.5/pm4py/visualization/graphs/util/common.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/graphs/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/variants/attributes.py` & `pm4py-2.7.5/pm4py/visualization/graphs/variants/attributes.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/variants/barplot.py` & `pm4py-2.7.5/pm4py/visualization/graphs/variants/barplot.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/variants/cases.py` & `pm4py-2.7.5/pm4py/visualization/graphs/variants/cases.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/variants/dates.py` & `pm4py-2.7.5/pm4py/visualization/graphs/variants/dates.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/graphs/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/graphs/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/heuristics_net/__init__.py` & `pm4py-2.7.5/pm4py/visualization/heuristics_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/heuristics_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/heuristics_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py` & `pm4py-2.7.5/pm4py/visualization/heuristics_net/variants/pydotplus_vis.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from pm4py.objects.heuristics_net.obj import HeuristicsNet
 from typing import Optional, Dict, Any, Union, Tuple
 from uuid import uuid4
 
 
 class Parameters(Enum):
     FORMAT = "format"
+    BGCOLOR = "bgcolor"
 
 
 def get_corr_hex(num):
     """
     Gets correspondence between a number
     and an hexadecimal string
 
@@ -133,16 +134,18 @@
     ------------
     graph
         Pydotplus graph
     """
     if parameters is None:
         parameters = {}
 
+    bgcolor = exec_utils.get_param_value(Parameters.BGCOLOR, parameters, constants.DEFAULT_BGCOLOR)
     graph = pydotplus.Dot(strict=True)
-    graph.obj_dict['attributes']['bgcolor'] = constants.DEFAULT_BGCOLOR
+    graph.obj_dict['attributes']['bgcolor'] = bgcolor
+    graph.set_bgcolor(bgcolor)
 
     corr_nodes = {}
     corr_nodes_names = {}
     is_frequency = False
 
     start_end_nodes_set = set()
```

### Comparing `pm4py-2.7.4/pm4py/visualization/heuristics_net/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/heuristics_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/network_analysis/__init__.py` & `pm4py-2.7.5/pm4py/visualization/network_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/network_analysis/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/network_analysis/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/network_analysis/variants/frequency.py` & `pm4py-2.7.5/pm4py/visualization/network_analysis/variants/frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/network_analysis/variants/performance.py` & `pm4py-2.7.5/pm4py/visualization/network_analysis/variants/performance.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/network_analysis/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/network_analysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/interleavings/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/interleavings/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/interleavings/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/interleavings/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/interleavings/variants/graphviz.py` & `pm4py-2.7.5/pm4py/visualization/ocel/interleavings/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/interleavings/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/ocel/interleavings/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/object_graph/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/object_graph/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/object_graph/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/sna/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,7 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
+from pm4py.visualization.sna import visualizer, variants
```

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/object_graph/variants/graphviz.py` & `pm4py-2.7.5/pm4py/visualization/ocel/object_graph/variants/graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/object_graph/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/ocel/object_graph/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocdfg/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocdfg/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocpn/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocpn/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocpn/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocpn/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocpn/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/ocel/ocpn/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/ocel/ocpn/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/performance_spectrum/__init__.py` & `pm4py-2.7.5/pm4py/visualization/performance_spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/performance_spectrum/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/performance_spectrum/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/performance_spectrum/variants/neato.py` & `pm4py-2.7.5/pm4py/visualization/performance_spectrum/variants/neato.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/performance_spectrum/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/performance_spectrum/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/__init__.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/common/__init__.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/util/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.visualization.petri_net.common import visualize
+from pm4py.visualization.petri_net.util import performance_map, vis_trans_shortest_paths, alignments_decoration
```

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/common/visualize.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/common/visualize.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/util/__init__.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/util/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.visualization.petri_net.util import performance_map, vis_trans_shortest_paths, alignments_decoration
+from pm4py.visualization.transition_system.util import visualize_graphviz
```

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/util/alignments_decoration.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/util/alignments_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/util/performance_map.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/util/performance_map.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/util/vis_trans_shortest_paths.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/alignments.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/alignments.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/greedy_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/greedy_decoration_performance.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/token_decoration_performance.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,21 +10,19 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.algo.discovery.dfg.variants import native, performance
-from pm4py.statistics.attributes.log import get as attr_get
-from pm4py.util import xes_constants as xes
+from pm4py.algo.conformance.tokenreplay import algorithm as token_replay
+from pm4py.statistics.variants.log import get as variants_get
 from pm4py.visualization.petri_net.common import visualize
-from pm4py.visualization.petri_net.util.vis_trans_shortest_paths import get_decorations_from_dfg_spaths_acticount
-from pm4py.visualization.petri_net.util.vis_trans_shortest_paths import get_shortest_paths
-from pm4py.util import exec_utils
+from pm4py.visualization.petri_net.util import performance_map
+from pm4py.util import exec_utils, xes_constants
 from enum import Enum
 from pm4py.util.constants import PARAMETER_CONSTANT_ACTIVITY_KEY, PARAMETER_CONSTANT_TIMESTAMP_KEY
 from pm4py.objects.petri_net.obj import PetriNet, Marking
 from typing import Optional, Dict, Any, Union, Tuple
 from pm4py.objects.log.obj import EventLog, EventStream
 import graphviz
 
@@ -36,85 +34,101 @@
     ACTIVITY_KEY = PARAMETER_CONSTANT_ACTIVITY_KEY
     TIMESTAMP_KEY = PARAMETER_CONSTANT_TIMESTAMP_KEY
     AGGREGATION_MEASURE = "aggregationMeasure"
     FONT_SIZE = "font_size"
     STAT_LOCALE = "stat_locale"
 
 
-def get_decorated_net(net, initial_marking, final_marking, log, parameters=None, variant="frequency"):
+def get_decorations(log, net, initial_marking, final_marking, parameters=None, measure="frequency",
+                    ht_perf_method="last"):
     """
-    Get a decorated net according to the specified variant (decorate Petri net based on DFG)
+    Calculate decorations in order to annotate the Petri net
 
     Parameters
-    ------------
+    -----------
+    log
+        Trace log
     net
         Petri net
     initial_marking
         Initial marking
     final_marking
         Final marking
-    log
-        Log to use to decorate the Petri net
     parameters
-        Algorithm parameters
-    variant
-        Specify if the decoration should take into account the frequency or the performance
+        Parameters associated to the algorithm
+    measure
+        Measure to represent on the process model (frequency/performance)
+    ht_perf_method
+        Method to use in order to annotate hidden transitions (performance value could be put on the last possible
+        point (last) or in the first possible point (first)
 
     Returns
     ------------
-    gviz
-        GraphViz object
+    decorations
+        Decorations to put on the process model
     """
     if parameters is None:
         parameters = {}
 
-    aggregation_measure = exec_utils.get_param_value(Parameters.AGGREGATION_MEASURE, parameters,
-                                                     "sum" if "frequency" in variant else "mean")
-
-    activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes.DEFAULT_NAME_KEY)
+    aggregation_measure = exec_utils.get_param_value(Parameters.AGGREGATION_MEASURE, parameters, None)
+    activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes_constants.DEFAULT_NAME_KEY)
+    timestamp_key = exec_utils.get_param_value(Parameters.TIMESTAMP_KEY, parameters,
+                                               xes_constants.DEFAULT_TIMESTAMP_KEY)
     stat_locale = exec_utils.get_param_value(Parameters.STAT_LOCALE, parameters, {})
 
-    # we find the DFG
-    if variant == "performance":
-        dfg = performance.performance(log, parameters=parameters)
-    else:
-        dfg = native.native(log, parameters=parameters)
-    # we find shortest paths
-    spaths = get_shortest_paths(net)
-    # we find the number of activities occurrences in the log
-    activities_count = attr_get.get_attribute_values(log, activity_key, parameters=parameters)
-    aggregated_statistics = get_decorations_from_dfg_spaths_acticount(net, dfg, spaths,
-                                                                      activities_count,
-                                                                      variant=variant,
-                                                                      aggregation_measure=aggregation_measure,
-                                                                      stat_locale=stat_locale)
+    variants_idx = variants_get.get_variants_from_log_trace_idx(log, parameters=parameters)
+    variants = variants_get.convert_variants_trace_idx_to_trace_obj(log, variants_idx)
 
-    return visualize.apply(net, initial_marking, final_marking, parameters=parameters,
-                           decorations=aggregated_statistics)
+    parameters_tr = {token_replay.Variants.TOKEN_REPLAY.value.Parameters.ACTIVITY_KEY: activity_key,
+                     token_replay.Variants.TOKEN_REPLAY.value.Parameters.VARIANTS: variants}
+
+    # do the replay
+    aligned_traces = token_replay.apply(log, net, initial_marking, final_marking, parameters=parameters_tr)
+
+    # apply petri_reduction technique in order to simplify the Petri net
+    # net = reduction.apply(net, parameters={"aligned_traces": aligned_traces})
+
+    element_statistics = performance_map.single_element_statistics(log, net, initial_marking,
+                                                                   aligned_traces, variants_idx,
+                                                                   activity_key=activity_key,
+                                                                   timestamp_key=timestamp_key,
+                                                                   ht_perf_method=ht_perf_method,
+                                                                   parameters=parameters)
+
+    aggregated_statistics = performance_map.aggregate_statistics(element_statistics, measure=measure,
+                                                                 aggregation_measure=aggregation_measure,
+                                                                 stat_locale=stat_locale)
+
+    return aggregated_statistics
 
 
 def apply(net: PetriNet, initial_marking: Marking, final_marking: Marking, log: EventLog = None, aggregated_statistics=None, parameters: Optional[Dict[Union[str, Parameters], Any]] = None) -> graphviz.Digraph:
     """
-    Apply performance decoration through greedy algorithm (decorate Petri net based on DFG)
+    Apply method for Petri net visualization (it calls the graphviz_visualization
+    method) adding performance representation obtained by token replay
 
     Parameters
-    ------------
+    -----------
     net
         Petri net
     initial_marking
         Initial marking
     final_marking
         Final marking
     log
-        Log to use to decorate the Petri net
+        (Optional) log
     aggregated_statistics
         Dictionary containing the frequency statistics
     parameters
-        Algorithm parameters
+        Algorithm parameters (including the activity key used during the replay, and the timestamp key)
 
     Returns
-    ------------
-    gviz
-        GraphViz object
+    -----------
+    viz
+        Graph object
     """
-    del aggregated_statistics
-    return get_decorated_net(net, initial_marking, final_marking, log, parameters=parameters, variant="performance")
+    if aggregated_statistics is None:
+        if log is not None:
+            aggregated_statistics = get_decorations(log, net, initial_marking, final_marking, parameters=parameters,
+                                                    measure="performance")
+    return visualize.apply(net, initial_marking, final_marking, parameters=parameters,
+                           decorations=aggregated_statistics)
```

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/token_decoration_frequency.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/token_decoration_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/token_decoration_performance.py` & `pm4py-2.7.5/pm4py/visualization/sna/variants/pyvis.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,125 +10,156 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.algo.conformance.tokenreplay import algorithm as token_replay
-from pm4py.statistics.variants.log import get as variants_get
-from pm4py.visualization.petri_net.common import visualize
-from pm4py.visualization.petri_net.util import performance_map
-from pm4py.util import exec_utils, xes_constants
+import shutil
+import tempfile
 from enum import Enum
-from pm4py.util.constants import PARAMETER_CONSTANT_ACTIVITY_KEY, PARAMETER_CONSTANT_TIMESTAMP_KEY
-from pm4py.objects.petri_net.obj import PetriNet, Marking
-from typing import Optional, Dict, Any, Union, Tuple
-from pm4py.objects.log.obj import EventLog, EventStream
-import graphviz
+
+from pm4py.util import exec_utils, vis_utils
+from pm4py.objects.org.sna.obj import SNA
 
 
 class Parameters(Enum):
-    FORMAT = "format"
-    DEBUG = "debug"
-    RANKDIR = "set_rankdir"
-    ACTIVITY_KEY = PARAMETER_CONSTANT_ACTIVITY_KEY
-    TIMESTAMP_KEY = PARAMETER_CONSTANT_TIMESTAMP_KEY
-    AGGREGATION_MEASURE = "aggregationMeasure"
-    FONT_SIZE = "font_size"
-    STAT_LOCALE = "stat_locale"
+    WEIGHT_THRESHOLD = "weight_threshold"
+    IFRAME_WIDTH = "iframe_width"
+    IFRAME_HEIGHT = "iframe_height"
+    LOCAL_JUPYTER_FILE_NAME = "local_jupyter_file_name"
 
 
-def get_decorations(log, net, initial_marking, final_marking, parameters=None, measure="frequency",
-                    ht_perf_method="last"):
+def get_temp_file_name(format):
     """
-    Calculate decorations in order to annotate the Petri net
+    Gets a temporary file name for the image
 
     Parameters
-    -----------
-    log
-        Trace log
-    net
-        Petri net
-    initial_marking
-        Initial marking
-    final_marking
-        Final marking
+    ------------
+    format
+        Format of the target image
+    """
+    filename = tempfile.NamedTemporaryFile(suffix='.' + format)
+
+    return filename.name
+
+
+def apply(sna: SNA, parameters=None):
+    """
+    Perform SNA visualization starting from the Matrix Container object
+    and the Resource-Resource matrix
+
+    Parameters
+    -------------
+    sna
+        Value of the metrics
     parameters
-        Parameters associated to the algorithm
-    measure
-        Measure to represent on the process model (frequency/performance)
-    ht_perf_method
-        Method to use in order to annotate hidden transitions (performance value could be put on the last possible
-        point (last) or in the first possible point (first)
+        Possible parameters of the algorithm, including:
+            - Parameters.WEIGHT_THRESHOLD -> the weight threshold to use in displaying the graph
 
     Returns
-    ------------
-    decorations
-        Decorations to put on the process model
+    -------------
+    temp_file_name
+        Name of a temporary file where the visualization is placed
     """
+    from pyvis.network import Network
+
     if parameters is None:
         parameters = {}
 
-    aggregation_measure = exec_utils.get_param_value(Parameters.AGGREGATION_MEASURE, parameters, None)
-    activity_key = exec_utils.get_param_value(Parameters.ACTIVITY_KEY, parameters, xes_constants.DEFAULT_NAME_KEY)
-    timestamp_key = exec_utils.get_param_value(Parameters.TIMESTAMP_KEY, parameters,
-                                               xes_constants.DEFAULT_TIMESTAMP_KEY)
-    stat_locale = exec_utils.get_param_value(Parameters.STAT_LOCALE, parameters, {})
+    weight_threshold = exec_utils.get_param_value(Parameters.WEIGHT_THRESHOLD, parameters, 0)
+    directed = sna.is_directed
 
-    variants_idx = variants_get.get_variants_from_log_trace_idx(log, parameters=parameters)
-    variants = variants_get.convert_variants_trace_idx_to_trace_obj(log, variants_idx)
+    temp_file_name = get_temp_file_name("html")
 
-    parameters_tr = {token_replay.Variants.TOKEN_REPLAY.value.Parameters.ACTIVITY_KEY: activity_key,
-                     token_replay.Variants.TOKEN_REPLAY.value.Parameters.VARIANTS: variants}
+    got_net = Network(height="750px", width="100%", bgcolor="black", font_color="#3de975", directed=directed)
+    # set the physics layout of the network
+    got_net.barnes_hut()
+
+    for c, w in sna.connections.items():
+        if w >= weight_threshold:
+            src = c[0]  # convert ids to labels
+            dst = c[1]
+
+            # I have to add some options here, there is no parameter
+            highlight = {'border': "#3de975", 'background': "#41e9df"}
+            # color = {'border': "#000000", 'background': "#123456"}
+            got_net.add_node(src, src, title=src, labelHighlightBold=True, color={'highlight': highlight})
+            got_net.add_node(dst, dst, title=dst, labelHighlightBold=True, color={'highlight': highlight})
+            got_net.add_edge(src, dst, value=w, title=w)
+
+    neighbor_map = got_net.get_adj_list()
+
+    # add neighbor data to node hover data
+    for node in got_net.nodes:
+        counter = 0
+        if directed:
+            node["title"] = "<h3>" + node["title"] + " Output Links: </h3>"
+        else:
+            node["title"] = "<h3>" + node["title"] + " Links: </h3>"
+        for neighbor in neighbor_map[node["id"]]:
+            if (counter % 10 == 0):
+                node["title"] += "<br>::: " + neighbor
+            else:
+                node["title"] += " ::: " + neighbor
+            node["value"] = len(neighbor_map[node["id"]])
+            counter += 1
+
+    got_net.show_buttons(filter_=['nodes', 'edges', 'physics'])
+
+    F = open(temp_file_name, "w")
+    try:
+        F.write(got_net.generate_html())
+        F.close()
+    except:
+        # networkx 3.1
+        F.close()
+        got_net.write_html(temp_file_name)
+    
+    return temp_file_name
 
-    # do the replay
-    aligned_traces = token_replay.apply(log, net, initial_marking, final_marking, parameters=parameters_tr)
 
-    # apply petri_reduction technique in order to simplify the Petri net
-    # net = reduction.apply(net, parameters={"aligned_traces": aligned_traces})
-
-    element_statistics = performance_map.single_element_statistics(log, net, initial_marking,
-                                                                   aligned_traces, variants_idx,
-                                                                   activity_key=activity_key,
-                                                                   timestamp_key=timestamp_key,
-                                                                   ht_perf_method=ht_perf_method,
-                                                                   parameters=parameters)
+def view(temp_file_name, parameters=None):
+    """
+    View the SNA visualization on the screen
 
-    aggregated_statistics = performance_map.aggregate_statistics(element_statistics, measure=measure,
-                                                                 aggregation_measure=aggregation_measure,
-                                                                 stat_locale=stat_locale)
+    Parameters
+    -------------
+    temp_file_name
+        Temporary file name
+    parameters
+        Possible parameters of the algorithm
+    """
+    if parameters is None:
+        parameters = {}
 
-    return aggregated_statistics
+    iframe_width = exec_utils.get_param_value(Parameters.IFRAME_WIDTH, parameters, 900)
+    iframe_height = exec_utils.get_param_value(Parameters.IFRAME_HEIGHT, parameters, 600)
+    local_jupyter_file_name = exec_utils.get_param_value(Parameters.LOCAL_JUPYTER_FILE_NAME, parameters, "jupyter_sna_vis.html")
+
+    if vis_utils.check_visualization_inside_jupyter():
+        from IPython.display import IFrame
+        shutil.copyfile(temp_file_name, local_jupyter_file_name)
+        iframe = IFrame(local_jupyter_file_name, width=iframe_width, height=iframe_height)
+        from IPython.display import display
+        return display(iframe)
+    else:
+        vis_utils.open_opsystem_image_viewer(temp_file_name)
 
 
-def apply(net: PetriNet, initial_marking: Marking, final_marking: Marking, log: EventLog = None, aggregated_statistics=None, parameters: Optional[Dict[Union[str, Parameters], Any]] = None) -> graphviz.Digraph:
+def save(temp_file_name, dest_file, parameters=None):
     """
-    Apply method for Petri net visualization (it calls the graphviz_visualization
-    method) adding performance representation obtained by token replay
+    Save the SNA visualization from a temporary file to a well-defined destination file
 
     Parameters
-    -----------
-    net
-        Petri net
-    initial_marking
-        Initial marking
-    final_marking
-        Final marking
-    log
-        (Optional) log
-    aggregated_statistics
-        Dictionary containing the frequency statistics
+    -------------
+    temp_file_name
+        Temporary file name
+    dest_file
+        Destination file
     parameters
-        Algorithm parameters (including the activity key used during the replay, and the timestamp key)
+        Possible parameters of the algorithm
+    """
+    if parameters is None:
+        parameters = {}
 
-    Returns
-    -----------
-    viz
-        Graph object
-    """
-    if aggregated_statistics is None:
-        if log is not None:
-            aggregated_statistics = get_decorations(log, net, initial_marking, final_marking, parameters=parameters,
-                                                    measure="performance")
-    return visualize.apply(net, initial_marking, final_marking, parameters=parameters,
-                           decorations=aggregated_statistics)
+    shutil.copyfile(temp_file_name, dest_file)
```

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/variants/wo_decoration.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/petri_net/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/petri_net/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/__init__.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/variants/frequency_annotation.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/variants/frequency_annotation.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/variants/symbolic.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/variants/symbolic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/variants/wo_decoration.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/variants/wo_decoration.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/process_tree/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/process_tree/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/sna/__init__.py` & `pm4py-2.7.5/pm4py/visualization/dotted_chart/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,8 +10,8 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.visualization.sna import visualizer, variants
+from pm4py.visualization.dotted_chart import visualizer, variants
```

### Comparing `pm4py-2.7.4/pm4py/visualization/sna/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/sna/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/sna/variants/networkx.py` & `pm4py-2.7.5/pm4py/visualization/sna/variants/networkx.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/sna/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/sna/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/__init__.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/util/__init__.py` & `pm4py-2.7.5/pm4py/algo/querying/llm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,8 +10,9 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with PM4Py.  If not, see <https://www.gnu.org/licenses/>.
 '''
-from pm4py.visualization.transition_system.util import visualize_graphviz
+
+from pm4py.algo.querying.llm import abstractions, connectors
```

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/util/visualize_graphviz.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/util/visualize_graphviz.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/variants/trans_frequency.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/variants/trans_frequency.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/variants/view_based.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/variants/view_based.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/transition_system/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/transition_system/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/trie/__init__.py` & `pm4py-2.7.5/pm4py/visualization/trie/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/trie/variants/__init__.py` & `pm4py-2.7.5/pm4py/visualization/trie/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/trie/variants/classic.py` & `pm4py-2.7.5/pm4py/visualization/trie/variants/classic.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/visualization/trie/visualizer.py` & `pm4py-2.7.5/pm4py/visualization/trie/visualizer.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py/write.py` & `pm4py-2.7.5/pm4py/write.py`

 * *Files identical despite different names*

### Comparing `pm4py-2.7.4/pm4py.egg-info/PKG-INFO` & `pm4py-2.7.5/pm4py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pm4py
-Version: 2.7.4
+Version: 2.7.5
 Summary: Process mining for Python
 Home-page: http://www.pm4py.org
 Author: Fraunhofer Institute for Applied Technology
 Author-email: pm4py@fit.fraunhofer.de
 License: GPL 3.0
 Project-URL: Documentation, http://www.pm4py.org
 Project-URL: Source, https://github.com/pm4py/pm4py-source
```

### Comparing `pm4py-2.7.4/pm4py.egg-info/SOURCES.txt` & `pm4py-2.7.5/pm4py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 pm4py/cli.py
 pm4py/conformance.py
 pm4py/connectors.py
 pm4py/convert.py
 pm4py/discovery.py
 pm4py/filtering.py
 pm4py/hof.py
+pm4py/llm.py
 pm4py/meta.py
 pm4py/ml.py
 pm4py/ocel.py
-pm4py/openai.py
 pm4py/org.py
 pm4py/privacy.py
 pm4py/read.py
 pm4py/sim.py
 pm4py/stats.py
 pm4py/utils.py
 pm4py/vis.py
@@ -492,23 +492,28 @@
 pm4py/algo/organizational_mining/sna/variants/log/working_together.py
 pm4py/algo/organizational_mining/sna/variants/pandas/__init__.py
 pm4py/algo/organizational_mining/sna/variants/pandas/handover.py
 pm4py/algo/organizational_mining/sna/variants/pandas/jointactivities.py
 pm4py/algo/organizational_mining/sna/variants/pandas/subcontracting.py
 pm4py/algo/organizational_mining/sna/variants/pandas/working_together.py
 pm4py/algo/querying/__init__.py
-pm4py/algo/querying/openai/__init__.py
-pm4py/algo/querying/openai/log_to_cols_descr.py
-pm4py/algo/querying/openai/log_to_dfg_descr.py
-pm4py/algo/querying/openai/log_to_variants_descr.py
-pm4py/algo/querying/openai/net_to_descr.py
-pm4py/algo/querying/openai/ocel_fea_descr.py
-pm4py/algo/querying/openai/ocel_ocdfg_descr.py
-pm4py/algo/querying/openai/perform_query.py
-pm4py/algo/querying/openai/stream_to_descr.py
+pm4py/algo/querying/llm/__init__.py
+pm4py/algo/querying/llm/abstractions/__init__.py
+pm4py/algo/querying/llm/abstractions/case_to_descr.py
+pm4py/algo/querying/llm/abstractions/log_to_cols_descr.py
+pm4py/algo/querying/llm/abstractions/log_to_dfg_descr.py
+pm4py/algo/querying/llm/abstractions/log_to_fea_descr.py
+pm4py/algo/querying/llm/abstractions/log_to_variants_descr.py
+pm4py/algo/querying/llm/abstractions/logske_to_descr.py
+pm4py/algo/querying/llm/abstractions/net_to_descr.py
+pm4py/algo/querying/llm/abstractions/ocel_fea_descr.py
+pm4py/algo/querying/llm/abstractions/ocel_ocdfg_descr.py
+pm4py/algo/querying/llm/abstractions/stream_to_descr.py
+pm4py/algo/querying/llm/connectors/__init__.py
+pm4py/algo/querying/llm/connectors/openai.py
 pm4py/algo/reduction/__init__.py
 pm4py/algo/reduction/process_tree/__init__.py
 pm4py/algo/reduction/process_tree/reducer.py
 pm4py/algo/reduction/process_tree/variants/__init__.py
 pm4py/algo/reduction/process_tree/variants/tree_tr_based.py
 pm4py/algo/simulation/__init__.py
 pm4py/algo/simulation/montecarlo/__init__.py
@@ -799,14 +804,15 @@
 pm4py/objects/ocel/util/parent_children_ref.py
 pm4py/objects/ocel/util/related_events.py
 pm4py/objects/ocel/util/related_objects.py
 pm4py/objects/ocel/util/rename_objs_ot_tim_lex.py
 pm4py/objects/ocel/util/sampling.py
 pm4py/objects/ocel/validation/__init__.py
 pm4py/objects/ocel/validation/jsonocel.py
+pm4py/objects/ocel/validation/ocel20_rel_validation.py
 pm4py/objects/ocel/validation/xmlocel.py
 pm4py/objects/org/__init__.py
 pm4py/objects/org/roles/__init__.py
 pm4py/objects/org/roles/obj.py
 pm4py/objects/org/sna/__init__.py
 pm4py/objects/org/sna/obj.py
 pm4py/objects/petri_net/__init__.py
```

### Comparing `pm4py-2.7.4/setup.py` & `pm4py-2.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
               'pm4py.algo.analysis.woflan.graphs', 'pm4py.algo.analysis.woflan.graphs.reachability_graph',
               'pm4py.algo.analysis.woflan.graphs.minimal_coverability_graph',
               'pm4py.algo.analysis.woflan.graphs.restricted_coverability_graph',
               'pm4py.algo.analysis.woflan.place_invariants', 'pm4py.algo.analysis.woflan.not_well_handled_pairs',
               'pm4py.algo.analysis.workflow_net', 'pm4py.algo.analysis.workflow_net.variants',
               'pm4py.algo.analysis.marking_equation', 'pm4py.algo.analysis.marking_equation.variants',
               'pm4py.algo.analysis.extended_marking_equation', 'pm4py.algo.analysis.extended_marking_equation.variants',
-              'pm4py.algo.querying', 'pm4py.algo.querying.openai', 'pm4py.algo.discovery', 'pm4py.algo.discovery.dfg',
+              'pm4py.algo.querying', 'pm4py.algo.querying.llm', 'pm4py.algo.querying.llm.connectors',
+              'pm4py.algo.querying.llm.abstractions', 'pm4py.algo.discovery', 'pm4py.algo.discovery.dfg',
               'pm4py.algo.discovery.dfg.utils', 'pm4py.algo.discovery.dfg.adapters',
               'pm4py.algo.discovery.dfg.adapters.pandas', 'pm4py.algo.discovery.dfg.variants',
               'pm4py.algo.discovery.ilp', 'pm4py.algo.discovery.ilp.variants', 'pm4py.algo.discovery.ocel',
               'pm4py.algo.discovery.ocel.ocpn', 'pm4py.algo.discovery.ocel.ocpn.variants',
               'pm4py.algo.discovery.ocel.ocdfg', 'pm4py.algo.discovery.ocel.ocdfg.variants',
               'pm4py.algo.discovery.ocel.saw_nets', 'pm4py.algo.discovery.ocel.saw_nets.variants',
               'pm4py.algo.discovery.ocel.interleavings', 'pm4py.algo.discovery.ocel.interleavings.utils',
```

### Comparing `pm4py-2.7.4/tests/test_cli.py` & `pm4py-2.7.5/tests/test_cli.py`

 * *Files identical despite different names*

