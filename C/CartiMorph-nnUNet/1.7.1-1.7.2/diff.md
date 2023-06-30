# Comparing `tmp/CartiMorph_nnUnet-1.7.1.tar.gz` & `tmp/CartiMorph_nnUNet-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CartiMorph_nnUnet-1.7.1.tar", last modified: Fri Jun 30 06:34:07 2023, max compression
+gzip compressed data, was "CartiMorph_nnUNet-1.7.2.tar", last modified: Fri Jun 30 06:49:02 2023, max compression
```

## Comparing `CartiMorph_nnUnet-1.7.1.tar` & `CartiMorph_nnUNet-1.7.2.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.934918 CartiMorph_nnUnet-1.7.1/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.880089 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/
--rw-r--r--   0 vincent    (501) staff       (20)      462 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/configuration.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.886461 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/
--rw-r--r--   0 vincent    (501) staff       (20)     3901 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py
--rw-r--r--   0 vincent    (501) staff       (20)     3287 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py
--rw-r--r--   0 vincent    (501) staff       (20)     4754 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     4535 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     6634 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py
--rw-r--r--   0 vincent    (501) staff       (20)     6987 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)    20639 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     9159 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task040_KiTS.py
--rw-r--r--   0 vincent    (501) staff       (20)     6075 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task043_BraTS_2019.py
--rw-r--r--   0 vincent    (501) staff       (20)     3462 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task055_SegTHOR.py
--rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task056_VerSe2019.py
--rw-r--r--   0 vincent    (501) staff       (20)     3396 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task056_Verse_normalize_orientation.py
--rw-r--r--   0 vincent    (501) staff       (20)     4263 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task058_ISBI_EM_SEG.py
--rw-r--r--   0 vincent    (501) staff       (20)     4324 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task059_EPFL_EM_MITO_SEG.py
--rw-r--r--   0 vincent    (501) staff       (20)     6124 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task061_CREMI.py
--rw-r--r--   0 vincent    (501) staff       (20)     3238 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task062_NIHPancreas.py
--rw-r--r--   0 vincent    (501) staff       (20)     3026 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task064_KiTS_labelsFixed.py
--rw-r--r--   0 vincent    (501) staff       (20)     3196 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task065_KiTS_NicksLabels.py
--rw-r--r--   0 vincent    (501) staff       (20)     2507 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task069_CovidSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     6317 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task075_Fluo_C3DH_A549_ManAndSim.py
--rw-r--r--   0 vincent    (501) staff       (20)    12105 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task076_Fluo_N3DH_SIM.py
--rw-r--r--   0 vincent    (501) staff       (20)    33438 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task082_BraTS_2020.py
--rw-r--r--   0 vincent    (501) staff       (20)     6403 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task083_VerSe2020.py
--rw-r--r--   0 vincent    (501) staff       (20)    12468 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task089_Fluo-N2DH-SIM.py
--rw-r--r--   0 vincent    (501) staff       (20)    12423 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py
--rw-r--r--   0 vincent    (501) staff       (20)    15009 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task115_COVIDSegChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     6292 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task120_Massachusetts_RoadSegm.py
--rw-r--r--   0 vincent    (501) staff       (20)     2209 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task135_KiTS2021.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     7681 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task154_RibFrac_multi_label.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     7551 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     5603 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task156_RibSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     5366 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task159_MyoPS2020.py
--rw-r--r--   0 vincent    (501) staff       (20)     1616 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task216_Amos2022_task1.py
--rw-r--r--   0 vincent    (501) staff       (20)     1619 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task217_Amos2022_task2.py
--rw-r--r--   0 vincent    (501) staff       (20)     2982 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task218_HC18.py
--rw-r--r--   0 vincent    (501) staff       (20)       55 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3641 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.887823 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3246 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/add_dummy_task_with_mean_over_all_tasks.py
--rw-r--r--   0 vincent    (501) staff       (20)     2024 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py
--rw-r--r--   0 vincent    (501) staff       (20)     1969 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/collect_results_files.py
--rw-r--r--   0 vincent    (501) staff       (20)    18780 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/evaluator.py
--rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/metrics.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.889373 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3483 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py
--rw-r--r--   0 vincent    (501) staff       (20)     7405 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py
--rw-r--r--   0 vincent    (501) staff       (20)    12941 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
--rw-r--r--   0 vincent    (501) staff       (20)    13165 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates.py
--rw-r--r--   0 vincent    (501) staff       (20)     6992 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_StructSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     6565 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_cascade.py
--rw-r--r--   0 vincent    (501) staff       (20)    12141 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_in_one_json.py
--rw-r--r--   0 vincent    (501) staff       (20)     6207 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_with_plans.py
--rw-r--r--   0 vincent    (501) staff       (20)     3938 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/region_based_evaluation.py
--rw-r--r--   0 vincent    (501) staff       (20)     2686 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/surface_dice.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.891913 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/
--rw-r--r--   0 vincent    (501) staff       (20)    11051 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.893638 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6754 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     6688 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     6752 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     1932 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py
--rw-r--r--   0 vincent    (501) staff       (20)     3151 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py
--rw-r--r--   0 vincent    (501) staff       (20)     1337 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py
--rw-r--r--   0 vincent    (501) staff       (20)     2161 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py
--rw-r--r--   0 vincent    (501) staff       (20)     7402 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.894338 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1625 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py
--rw-r--r--   0 vincent    (501) staff       (20)     2016 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1765 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.894793 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7015 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py
--rw-r--r--   0 vincent    (501) staff       (20)     6308 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.895252 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7697 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py
--rw-r--r--   0 vincent    (501) staff       (20)     6766 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.895858 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3624 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py
--rw-r--r--   0 vincent    (501) staff       (20)     1787 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py
--rw-r--r--   0 vincent    (501) staff       (20)    12203 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py
--rw-r--r--   0 vincent    (501) staff       (20)      500 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/change_batch_size.py
--rw-r--r--   0 vincent    (501) staff       (20)    10562 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/common_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     8773 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     5784 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py
--rw-r--r--   0 vincent    (501) staff       (20)    26524 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    10260 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py
--rw-r--r--   0 vincent    (501) staff       (20)     4015 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/nnUNet_convert_decathlon_task.py
--rw-r--r--   0 vincent    (501) staff       (20)    10041 2023-04-05 08:06:36.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.896126 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/old/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/old/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     5224 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/old/old_plan_and_preprocess_task.py
--rw-r--r--   0 vincent    (501) staff       (20)     4189 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/summarize_plans.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.896293 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.896519 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    10497 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py
--rw-r--r--   0 vincent    (501) staff       (20)     9635 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.898250 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.898509 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/amos2022/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/amos2022/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    11488 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/amos2022/inference_code.py
--rw-r--r--   0 vincent    (501) staff       (20)     2631 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/change_trainer.py
--rw-r--r--   0 vincent    (501) staff       (20)     6300 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/ensemble_predictions.py
--rw-r--r--   0 vincent    (501) staff       (20)    44882 2023-05-01 15:47:02.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/predict.py
--rw-r--r--   0 vincent    (501) staff       (20)    13856 2023-05-01 15:47:01.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/predict_simple.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.898918 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    14181 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/collect_pretrained_models.py
--rw-r--r--   0 vincent    (501) staff       (20)    23045 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/download_pretrained_model.py
--rw-r--r--   0 vincent    (501) staff       (20)    12220 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/segmentation_export.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.900991 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.901947 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    12558 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/conv_blocks.py
--rw-r--r--   0 vincent    (501) staff       (20)     1547 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/feature_response_normalization.py
--rw-r--r--   0 vincent    (501) staff       (20)     1051 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py
--rw-r--r--   0 vincent    (501) staff       (20)      730 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/mish.py
--rw-r--r--   0 vincent    (501) staff       (20)    21046 2023-05-02 11:15:11.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     6839 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_UNet_DP.py
--rw-r--r--   0 vincent    (501) staff       (20)    20014 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    27608 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_preact_residual_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    25056 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_residual_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/initialization.py
--rw-r--r--   0 vincent    (501) staff       (20)    44012 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/neural_network.py
--rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/paths.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.902722 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    19122 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/connected_components.py
--rw-r--r--   0 vincent    (501) staff       (20)     3162 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_all_for_paper.py
--rw-r--r--   0 vincent    (501) staff       (20)     4849 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py
--rw-r--r--   0 vincent    (501) staff       (20)     2729 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing_simple.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.903530 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/cropping.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.903829 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/custom_preprocessors/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/custom_preprocessors/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3475 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py
--rw-r--r--   0 vincent    (501) staff       (20)    48208 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/preprocessing.py
--rw-r--r--   0 vincent    (501) staff       (20)    12201 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/sanity_checks.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.905070 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3818 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/default_configuration.py
--rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/load_pretrained_weights.py
--rw-r--r--   0 vincent    (501) staff       (20)    11797 2023-04-06 04:03:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training.py
--rw-r--r--   0 vincent    (501) staff       (20)    11803 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training_DDP.py
--rw-r--r--   0 vincent    (501) staff       (20)    11809 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training_DP.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.905506 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.905913 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/cascade_stuff/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6237 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.907704 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
--rw-r--r--   0 vincent    (501) staff       (20)    11100 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py
--rw-r--r--   0 vincent    (501) staff       (20)    11280 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py
--rw-r--r--   0 vincent    (501) staff       (20)    12621 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     5012 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_noDA.py
--rw-r--r--   0 vincent    (501) staff       (20)    12938 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
--rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
--rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.908029 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/dataloading/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/dataloading/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    33671 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.908400 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/learning_rate/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/learning_rate/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.909340 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/
--rw-r--r--   0 vincent    (501) staff       (20)     1364 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
--rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
--rw-r--r--   0 vincent    (501) staff       (20)    13960 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7125 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/model_restore.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.911658 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.911828 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.912348 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    21314 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py
--rw-r--r--   0 vincent    (501) staff       (20)    14415 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.912681 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/__init__.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     2662 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    31382 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/network_trainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    39860 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    16064 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
--rw-r--r--   0 vincent    (501) staff       (20)    22667 2023-05-02 11:04:46.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
--rw-r--r--   0 vincent    (501) staff       (20)    19613 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
--rw-r--r--   0 vincent    (501) staff       (20)    34510 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DDP.py
--rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DP.py
--rw-r--r--   0 vincent    (501) staff       (20)     1225 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_fp32.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.913425 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.917889 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2271 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py
--rw-r--r--   0 vincent    (501) staff       (20)     2214 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py
--rw-r--r--   0 vincent    (501) staff       (20)     2473 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2430 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2379 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2829 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py
--rw-r--r--   0 vincent    (501) staff       (20)     2221 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py
--rw-r--r--   0 vincent    (501) staff       (20)     2228 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py
--rw-r--r--   0 vincent    (501) staff       (20)     2256 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py
--rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2180 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py
--rw-r--r--   0 vincent    (501) staff       (20)     2258 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py
--rw-r--r--   0 vincent    (501) staff       (20)     2285 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py
--rw-r--r--   0 vincent    (501) staff       (20)     6082 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     6085 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2155 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py
--rw-r--r--   0 vincent    (501) staff       (20)     1582 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py
--rw-r--r--   0 vincent    (501) staff       (20)    19820 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py
--rw-r--r--   0 vincent    (501) staff       (20)     2727 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2288 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py
--rw-r--r--   0 vincent    (501) staff       (20)     2318 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py
--rw-r--r--   0 vincent    (501) staff       (20)     8834 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py
--rw-r--r--   0 vincent    (501) staff       (20)     6236 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.918454 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    14098 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py
--rw-r--r--   0 vincent    (501) staff       (20)     6509 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.919338 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4283 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py
--rw-r--r--   0 vincent    (501) staff       (20)     1321 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py
--rw-r--r--   0 vincent    (501) staff       (20)     1324 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py
--rw-r--r--   0 vincent    (501) staff       (20)     1363 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.919664 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2527 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.921186 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1182 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py
--rw-r--r--   0 vincent    (501) staff       (20)     9841 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py
--rw-r--r--   0 vincent    (501) staff       (20)    20353 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py
--rw-r--r--   0 vincent    (501) staff       (20)      976 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py
--rw-r--r--   0 vincent    (501) staff       (20)     7727 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     7811 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     2321 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.924085 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1180 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py
--rw-r--r--   0 vincent    (501) staff       (20)     1181 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py
--rw-r--r--   0 vincent    (501) staff       (20)     1276 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py
--rw-r--r--   0 vincent    (501) staff       (20)     1331 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py
--rw-r--r--   0 vincent    (501) staff       (20)     1936 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py
--rw-r--r--   0 vincent    (501) staff       (20)     1352 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py
--rw-r--r--   0 vincent    (501) staff       (20)     1382 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py
--rw-r--r--   0 vincent    (501) staff       (20)     1743 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     1462 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py
--rw-r--r--   0 vincent    (501) staff       (20)     1943 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py
--rw-r--r--   0 vincent    (501) staff       (20)     1514 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py
--rw-r--r--   0 vincent    (501) staff       (20)     1469 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py
--rw-r--r--   0 vincent    (501) staff       (20)     2667 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.924738 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     9982 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py
--rw-r--r--   0 vincent    (501) staff       (20)     1304 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py
--rw-r--r--   0 vincent    (501) staff       (20)     4489 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.929087 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1245 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py
--rw-r--r--   0 vincent    (501) staff       (20)     2899 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py
--rw-r--r--   0 vincent    (501) staff       (20)     1246 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py
--rw-r--r--   0 vincent    (501) staff       (20)     2707 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py
--rw-r--r--   0 vincent    (501) staff       (20)     1808 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py
--rw-r--r--   0 vincent    (501) staff       (20)     1950 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1610 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py
--rw-r--r--   0 vincent    (501) staff       (20)     3693 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py
--rw-r--r--   0 vincent    (501) staff       (20)     1206 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py
--rw-r--r--   0 vincent    (501) staff       (20)     1192 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py
--rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py
--rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py
--rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py
--rw-r--r--   0 vincent    (501) staff       (20)     1947 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py
--rw-r--r--   0 vincent    (501) staff       (20)     1756 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.929416 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3472 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.929742 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/optimizer/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/optimizer/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/optimizer/ranger.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.933540 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3172 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/distributed.py
--rw-r--r--   0 vincent    (501) staff       (20)     4533 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/file_conversions.py
--rw-r--r--   0 vincent    (501) staff       (20)     1130 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/file_endings.py
--rw-r--r--   0 vincent    (501) staff       (20)     1810 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/folder_names.py
--rw-r--r--   0 vincent    (501) staff       (20)     4564 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/image_reorientation.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/nd_softmax.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/one_hot_encoding.py
--rw-r--r--   0 vincent    (501) staff       (20)     8434 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/overlay_plots.py
--rw-r--r--   0 vincent    (501) staff       (20)      794 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/random_stuff.py
--rw-r--r--   0 vincent    (501) staff       (20)     1554 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/recursive_delete_npz.py
--rw-r--r--   0 vincent    (501) staff       (20)     1770 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py
--rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
--rw-r--r--   0 vincent    (501) staff       (20)      908 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/sitk_stuff.py
--rw-r--r--   0 vincent    (501) staff       (20)     3514 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
--rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/tensor_utilities.py
--rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/to_torch.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:34:07.934536 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)    22209 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)     1627 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)      151 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       18 2023-06-30 06:34:07.000000 CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUnet-1.7.1/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 06:34:07.934757 CartiMorph_nnUnet-1.7.1/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      699 2023-06-30 06:30:41.000000 CartiMorph_nnUnet-1.7.1/README.md
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 06:34:07.934973 CartiMorph_nnUnet-1.7.1/setup.cfg
--rwxr-xr-x   0 vincent    (501) staff       (20)     3034 2023-06-30 06:33:46.000000 CartiMorph_nnUnet-1.7.1/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.730042 CartiMorph_nnUNet-1.7.2/
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.663042 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/
+-rw-r--r--   0 vincent    (501) staff       (20)      462 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/configuration.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.671960 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/
+-rw-r--r--   0 vincent    (501) staff       (20)     3901 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3287 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4754 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4535 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6634 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6987 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py
+-rw-r--r--   0 vincent    (501) staff       (20)    20639 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9159 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task040_KiTS.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6075 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task043_BraTS_2019.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3462 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task055_SegTHOR.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task056_VerSe2019.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3396 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task056_Verse_normalize_orientation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4263 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task058_ISBI_EM_SEG.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4324 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task059_EPFL_EM_MITO_SEG.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6124 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task061_CREMI.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3238 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task062_NIHPancreas.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3026 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task064_KiTS_labelsFixed.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3196 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task065_KiTS_NicksLabels.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2507 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task069_CovidSeg.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6317 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task075_Fluo_C3DH_A549_ManAndSim.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12105 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task076_Fluo_N3DH_SIM.py
+-rw-r--r--   0 vincent    (501) staff       (20)    33438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task082_BraTS_2020.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6403 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task083_VerSe2020.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12468 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task089_Fluo-N2DH-SIM.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12423 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py
+-rw-r--r--   0 vincent    (501) staff       (20)    15009 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task115_COVIDSegChallenge.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6292 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task120_Massachusetts_RoadSegm.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2209 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task135_KiTS2021.py
+-rwxr-xr-x   0 vincent    (501) staff       (20)     7681 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task154_RibFrac_multi_label.py
+-rwxr-xr-x   0 vincent    (501) staff       (20)     7551 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py
+-rwxr-xr-x   0 vincent    (501) staff       (20)     5603 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task156_RibSeg.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5366 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task159_MyoPS2020.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1616 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task216_Amos2022_task1.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1619 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task217_Amos2022_task2.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2982 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task218_HC18.py
+-rw-r--r--   0 vincent    (501) staff       (20)       55 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3641 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/utils.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.673689 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3246 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/add_dummy_task_with_mean_over_all_tasks.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2024 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1969 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/collect_results_files.py
+-rw-r--r--   0 vincent    (501) staff       (20)    18780 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/evaluator.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/metrics.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.676088 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3483 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7405 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12941 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13165 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6992 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_StructSeg.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6565 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_cascade.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12141 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_in_one_json.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6207 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_with_plans.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3938 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/region_based_evaluation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2686 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/surface_dice.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.680237 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/
+-rw-r--r--   0 vincent    (501) staff       (20)    11051 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.681711 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6754 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6688 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6752 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1932 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3151 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1337 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2161 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7402 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.682432 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1625 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2016 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1765 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.683240 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7015 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6308 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.683707 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7697 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6766 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.686122 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1787 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12203 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py
+-rw-r--r--   0 vincent    (501) staff       (20)      500 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/change_batch_size.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10562 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/common_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8773 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5784 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py
+-rw-r--r--   0 vincent    (501) staff       (20)    26524 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10260 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4015 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/nnUNet_convert_decathlon_task.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10041 2023-04-05 08:06:36.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.686400 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/old/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/old/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5224 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/old/old_plan_and_preprocess_task.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4189 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/summarize_plans.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.686559 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.686777 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10497 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9635 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/utils.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.689035 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.689387 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/amos2022/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/amos2022/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11488 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/amos2022/inference_code.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2631 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/change_trainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6300 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/ensemble_predictions.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44882 2023-05-01 15:47:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/predict.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13856 2023-05-01 15:47:01.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/predict_simple.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.689914 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    14181 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/collect_pretrained_models.py
+-rw-r--r--   0 vincent    (501) staff       (20)    23045 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/download_pretrained_model.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12220 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/segmentation_export.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.692134 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.693045 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12558 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/conv_blocks.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1547 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/feature_response_normalization.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1051 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py
+-rw-r--r--   0 vincent    (501) staff       (20)      730 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/mish.py
+-rw-r--r--   0 vincent    (501) staff       (20)    21046 2023-05-02 11:15:11.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6839 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_UNet_DP.py
+-rw-r--r--   0 vincent    (501) staff       (20)    20014 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    27608 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_preact_residual_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    25056 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_residual_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/initialization.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44012 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/neural_network.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/paths.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.693791 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19122 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/connected_components.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3162 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_all_for_paper.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4849 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2729 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing_simple.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.694860 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/cropping.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.695121 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/custom_preprocessors/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/custom_preprocessors/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3475 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py
+-rw-r--r--   0 vincent    (501) staff       (20)    48208 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/preprocessing.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12201 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/sanity_checks.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.696674 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3818 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/default_configuration.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/load_pretrained_weights.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11797 2023-04-06 04:03:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11803 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training_DDP.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11809 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training_DP.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.697081 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.697455 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/cascade_stuff/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6237 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.698894 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11100 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11280 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12621 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)     5012 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_noDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12938 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.699192 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/dataloading/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/dataloading/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    33671 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.699527 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/learning_rate/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/learning_rate/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.700434 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/
+-rw-r--r--   0 vincent    (501) staff       (20)     1364 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13960 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7125 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/model_restore.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.703618 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.703829 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.704843 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    21314 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py
+-rw-r--r--   0 vincent    (501) staff       (20)    14415 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.705184 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/__init__.py
+-rwxr-xr-x   0 vincent    (501) staff       (20)     2662 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    31382 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/network_trainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    39860 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    16064 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
+-rw-r--r--   0 vincent    (501) staff       (20)    22667 2023-05-02 11:04:46.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19613 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
+-rw-r--r--   0 vincent    (501) staff       (20)    34510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DDP.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DP.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1225 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_fp32.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.705999 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.711715 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2271 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2214 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2473 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2430 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2379 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2829 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2221 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2228 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2256 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2180 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2258 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2285 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6082 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6085 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2155 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1582 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19820 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2727 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2288 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2318 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8834 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6236 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.712281 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    14098 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6509 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.713352 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4283 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1321 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1324 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1363 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.713827 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2527 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.717332 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1182 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py
+-rw-r--r--   0 vincent    (501) staff       (20)    20353 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py
+-rw-r--r--   0 vincent    (501) staff       (20)      976 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7727 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7811 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2321 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.721451 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1180 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1181 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1276 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1331 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1936 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1352 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1382 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1743 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1462 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1943 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1514 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1469 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2667 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.722054 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9982 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1304 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4489 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.726092 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1245 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2899 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1246 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2707 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1808 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1950 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1610 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3693 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1206 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1192 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1947 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1756 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.726395 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3472 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.726673 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/optimizer/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/optimizer/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/optimizer/ranger.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.729650 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3172 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/distributed.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4533 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/file_conversions.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1130 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/file_endings.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1810 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/folder_names.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4564 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/image_reorientation.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/nd_softmax.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/one_hot_encoding.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8434 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/overlay_plots.py
+-rw-r--r--   0 vincent    (501) staff       (20)      794 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/random_stuff.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1554 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/recursive_delete_npz.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1770 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
+-rw-r--r--   0 vincent    (501) staff       (20)      908 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/sitk_stuff.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3514 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/tensor_utilities.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/to_torch.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 06:49:02.663947 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)    22209 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)     1627 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      151 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       18 2023-06-30 06:49:02.000000 CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUNet-1.7.2/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 06:49:02.729881 CartiMorph_nnUNet-1.7.2/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      696 2023-06-30 06:47:33.000000 CartiMorph_nnUNet-1.7.2/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 06:49:02.730090 CartiMorph_nnUNet-1.7.2/setup.cfg
+-rwxr-xr-x   0 vincent    (501) staff       (20)     3034 2023-06-30 06:48:11.000000 CartiMorph_nnUNet-1.7.2/setup.py
```

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task040_KiTS.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task040_KiTS.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task043_BraTS_2019.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task043_BraTS_2019.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task055_SegTHOR.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task055_SegTHOR.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task056_VerSe2019.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task056_VerSe2019.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task056_Verse_normalize_orientation.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task056_Verse_normalize_orientation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task058_ISBI_EM_SEG.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task058_ISBI_EM_SEG.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task059_EPFL_EM_MITO_SEG.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task059_EPFL_EM_MITO_SEG.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task061_CREMI.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task061_CREMI.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task062_NIHPancreas.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task062_NIHPancreas.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task064_KiTS_labelsFixed.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task064_KiTS_labelsFixed.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task065_KiTS_NicksLabels.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task065_KiTS_NicksLabels.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task069_CovidSeg.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task069_CovidSeg.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task075_Fluo_C3DH_A549_ManAndSim.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task075_Fluo_C3DH_A549_ManAndSim.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task076_Fluo_N3DH_SIM.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task076_Fluo_N3DH_SIM.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task082_BraTS_2020.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task082_BraTS_2020.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task083_VerSe2020.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task083_VerSe2020.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task089_Fluo-N2DH-SIM.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task089_Fluo-N2DH-SIM.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task115_COVIDSegChallenge.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task115_COVIDSegChallenge.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task120_Massachusetts_RoadSegm.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task120_Massachusetts_RoadSegm.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task135_KiTS2021.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task135_KiTS2021.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task154_RibFrac_multi_label.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task154_RibFrac_multi_label.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task156_RibSeg.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task156_RibSeg.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task159_MyoPS2020.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task159_MyoPS2020.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task216_Amos2022_task1.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task216_Amos2022_task1.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task217_Amos2022_task2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task217_Amos2022_task2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/Task218_HC18.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/Task218_HC18.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/dataset_conversion/utils.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/dataset_conversion/utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/add_dummy_task_with_mean_over_all_tasks.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/add_dummy_task_with_mean_over_all_tasks.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/collect_results_files.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/collect_results_files.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/evaluator.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/metrics.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_StructSeg.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_StructSeg.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_cascade.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_cascade.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_in_one_json.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_in_one_json.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_with_plans.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_with_plans.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/region_based_evaluation.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/region_based_evaluation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/evaluation/surface_dice.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/evaluation/surface_dice.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/common_utils.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/common_utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/nnUNet_convert_decathlon_task.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/nnUNet_convert_decathlon_task.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/old/old_plan_and_preprocess_task.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/old/old_plan_and_preprocess_task.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/summarize_plans.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/summarize_plans.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/experiment_planning/utils.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/experiment_planning/utils.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/amos2022/inference_code.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/amos2022/inference_code.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/change_trainer.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/change_trainer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/ensemble_predictions.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/ensemble_predictions.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/predict.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/predict.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/predict_simple.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/predict_simple.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/collect_pretrained_models.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/collect_pretrained_models.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/pretrained_models/download_pretrained_model.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/pretrained_models/download_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/inference/segmentation_export.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/inference/segmentation_export.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/conv_blocks.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/conv_blocks.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/feature_response_normalization.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/feature_response_normalization.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/custom_modules/mish.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/custom_modules/mish.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_UNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_UNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_UNet_DP.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_UNet_DP.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_UNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_UNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_preact_residual_UNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_preact_residual_UNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/generic_modular_residual_UNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/generic_modular_residual_UNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/initialization.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/initialization.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/network_architecture/neural_network.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/network_architecture/neural_network.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/paths.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/paths.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/connected_components.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/connected_components.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_all_for_paper.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_all_for_paper.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing_simple.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing_simple.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/cropping.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/cropping.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/preprocessing.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/preprocessing/sanity_checks.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/preprocessing/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/default_configuration.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/default_configuration.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/load_pretrained_weights.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/load_pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training_DDP.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training_DDP.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/run/run_training_DP.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/run/run_training_DP.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_noDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_noDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/downsampling.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/downsampling.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/dataloading/dataset_loading.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/dataloading/dataset_loading.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/learning_rate/poly_lr.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/learning_rate/poly_lr.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/dice_loss.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/dice_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/loss_functions/focal_loss.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/loss_functions/focal_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/model_restore.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/model_restore.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/network_trainer.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/network_trainer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DDP.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DDP.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DP.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DP.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_fp32.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_fp32.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/training/optimizer/ranger.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/training/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/distributed.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/file_conversions.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/file_conversions.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/file_endings.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/file_endings.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/folder_names.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/folder_names.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/image_reorientation.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/image_reorientation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/nd_softmax.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/nd_softmax.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/one_hot_encoding.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/one_hot_encoding.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/overlay_plots.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/overlay_plots.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/random_stuff.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/random_stuff.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/recursive_delete_npz.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/recursive_delete_npz.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/set_n_proc_DA.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/set_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/sitk_stuff.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/sitk_stuff.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/task_name_id_conversion.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/task_name_id_conversion.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/tensor_utilities.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/tensor_utilities.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUNet/utilities/to_torch.py` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet/utilities/to_torch.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/SOURCES.txt` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 LICENSE
 README.md
 setup.py
 CartiMorph_nnUNet/__init__.py
 CartiMorph_nnUNet/configuration.py
 CartiMorph_nnUNet/paths.py
+CartiMorph_nnUNet.egg-info/PKG-INFO
+CartiMorph_nnUNet.egg-info/SOURCES.txt
+CartiMorph_nnUNet.egg-info/dependency_links.txt
+CartiMorph_nnUNet.egg-info/entry_points.txt
+CartiMorph_nnUNet.egg-info/requires.txt
+CartiMorph_nnUNet.egg-info/top_level.txt
 CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py
 CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py
 CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py
 CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py
 CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py
 CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py
 CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py
@@ -273,14 +279,8 @@
 CartiMorph_nnUNet/utilities/random_stuff.py
 CartiMorph_nnUNet/utilities/recursive_delete_npz.py
 CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py
 CartiMorph_nnUNet/utilities/set_n_proc_DA.py
 CartiMorph_nnUNet/utilities/sitk_stuff.py
 CartiMorph_nnUNet/utilities/task_name_id_conversion.py
 CartiMorph_nnUNet/utilities/tensor_utilities.py
-CartiMorph_nnUNet/utilities/to_torch.py
-CartiMorph_nnUnet.egg-info/PKG-INFO
-CartiMorph_nnUnet.egg-info/SOURCES.txt
-CartiMorph_nnUnet.egg-info/dependency_links.txt
-CartiMorph_nnUnet.egg-info/entry_points.txt
-CartiMorph_nnUnet.egg-info/requires.txt
-CartiMorph_nnUnet.egg-info/top_level.txt
+CartiMorph_nnUNet/utilities/to_torch.py
```

### Comparing `CartiMorph_nnUnet-1.7.1/CartiMorph_nnUnet.egg-info/entry_points.txt` & `CartiMorph_nnUNet-1.7.2/CartiMorph_nnUNet.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/LICENSE` & `CartiMorph_nnUNet-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUnet-1.7.1/README.md` & `CartiMorph_nnUNet-1.7.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 A work based on [nnUNet](https://github.com/MIC-DKFZ/nnUNet)
 
 
 
 ## Installation
 
 ```python
-python -m pip install CartiMorph-nnUnet==1.7.0
+python -m pip install CartiMorph-nnUnet==1.7.1
 ```
 
 check the installation with
 
 ```python
-python -c "import CartiMorph-nnUnet as nnUnet; print(nnUnet.__version__)"  
+python -c "import CartiMorph_nnUNet as nnUnet; print(nnUnet.__file__)"  
 ```
 
 successful installation should return `0.5`
```

### Comparing `CartiMorph_nnUnet-1.7.1/setup.py` & `CartiMorph_nnUNet-1.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
-setup(name='CartiMorph_nnUnet',
+setup(name='CartiMorph_nnUNet',
       packages=find_namespace_packages(include=["CartiMorph_nnUNet", "CartiMorph_nnUNet.*"]),
-      version='1.7.1',
+      version='1.7.2',
       description='nnU-Net with minor revisions tailored for the CartiMorph framework.',
       url='https://github.com/YongchengYAO/CartiMorph-nnUNet',
       author='Yongcheng Yao, Chinese University of Hong Kong',
       license='Apache License Version 2.0, January 2004',
       install_requires=[
             "torch>1.10.0",
             "tqdm",
```

