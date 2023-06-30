# Comparing `tmp/CartiMorph_nnUNet-1.7.3.tar.gz` & `tmp/CartiMorph_nnUNet-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CartiMorph_nnUNet-1.7.3.tar", last modified: Fri Jun 30 07:10:05 2023, max compression
+gzip compressed data, was "CartiMorph_nnUNet-1.7.4.tar", last modified: Fri Jun 30 09:18:11 2023, max compression
```

## Comparing `CartiMorph_nnUNet-1.7.3.tar` & `CartiMorph_nnUNet-1.7.4.tar`

### file list

```diff
@@ -1,334 +1,106 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.513669 CartiMorph_nnUNet-1.7.3/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.457036 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/
--rw-r--r--   0 vincent    (501) staff       (20)      617 2023-06-30 07:01:28.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/configuration.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.465261 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/
--rw-r--r--   0 vincent    (501) staff       (20)     3901 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task017_BeyondCranialVaultAbdominalOrganSegmentation.py
--rw-r--r--   0 vincent    (501) staff       (20)     3287 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task024_Promise2012.py
--rw-r--r--   0 vincent    (501) staff       (20)     4754 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task027_AutomaticCardiacDetectionChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     4535 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task029_LiverTumorSegmentationChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     6634 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task032_BraTS_2018.py
--rw-r--r--   0 vincent    (501) staff       (20)     6987 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task035_ISBI_MSLesionSegmentationChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)    20639 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task037_038_Chaos_Challenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     9159 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task040_KiTS.py
--rw-r--r--   0 vincent    (501) staff       (20)     6075 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task043_BraTS_2019.py
--rw-r--r--   0 vincent    (501) staff       (20)     3462 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task055_SegTHOR.py
--rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task056_VerSe2019.py
--rw-r--r--   0 vincent    (501) staff       (20)     3396 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task056_Verse_normalize_orientation.py
--rw-r--r--   0 vincent    (501) staff       (20)     4263 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task058_ISBI_EM_SEG.py
--rw-r--r--   0 vincent    (501) staff       (20)     4324 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task059_EPFL_EM_MITO_SEG.py
--rw-r--r--   0 vincent    (501) staff       (20)     6124 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task061_CREMI.py
--rw-r--r--   0 vincent    (501) staff       (20)     3238 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task062_NIHPancreas.py
--rw-r--r--   0 vincent    (501) staff       (20)     3026 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task064_KiTS_labelsFixed.py
--rw-r--r--   0 vincent    (501) staff       (20)     3196 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task065_KiTS_NicksLabels.py
--rw-r--r--   0 vincent    (501) staff       (20)     2507 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task069_CovidSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     6317 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task075_Fluo_C3DH_A549_ManAndSim.py
--rw-r--r--   0 vincent    (501) staff       (20)    12105 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task076_Fluo_N3DH_SIM.py
--rw-r--r--   0 vincent    (501) staff       (20)    33438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task082_BraTS_2020.py
--rw-r--r--   0 vincent    (501) staff       (20)     6403 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task083_VerSe2020.py
--rw-r--r--   0 vincent    (501) staff       (20)    12468 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task089_Fluo-N2DH-SIM.py
--rw-r--r--   0 vincent    (501) staff       (20)    12423 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py
--rw-r--r--   0 vincent    (501) staff       (20)    15009 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task115_COVIDSegChallenge.py
--rw-r--r--   0 vincent    (501) staff       (20)     6292 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task120_Massachusetts_RoadSegm.py
--rw-r--r--   0 vincent    (501) staff       (20)     2209 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task135_KiTS2021.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     7681 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task154_RibFrac_multi_label.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     7551 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     5603 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task156_RibSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     5366 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task159_MyoPS2020.py
--rw-r--r--   0 vincent    (501) staff       (20)     1616 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task216_Amos2022_task1.py
--rw-r--r--   0 vincent    (501) staff       (20)     1619 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task217_Amos2022_task2.py
--rw-r--r--   0 vincent    (501) staff       (20)     2982 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task218_HC18.py
--rw-r--r--   0 vincent    (501) staff       (20)       55 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3641 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.466664 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3246 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/add_dummy_task_with_mean_over_all_tasks.py
--rw-r--r--   0 vincent    (501) staff       (20)     2024 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py
--rw-r--r--   0 vincent    (501) staff       (20)     1969 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/collect_results_files.py
--rw-r--r--   0 vincent    (501) staff       (20)    18780 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/evaluator.py
--rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/metrics.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.468195 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3483 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/collect_all_fold0_results_and_summarize_in_one_csv.py
--rw-r--r--   0 vincent    (501) staff       (20)     7405 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/ensemble.py
--rw-r--r--   0 vincent    (501) staff       (20)    12941 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/figure_out_what_to_submit.py
--rw-r--r--   0 vincent    (501) staff       (20)    13165 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates.py
--rw-r--r--   0 vincent    (501) staff       (20)     6992 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_StructSeg.py
--rw-r--r--   0 vincent    (501) staff       (20)     6565 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/rank_candidates_cascade.py
--rw-r--r--   0 vincent    (501) staff       (20)    12141 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_in_one_json.py
--rw-r--r--   0 vincent    (501) staff       (20)     6207 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/model_selection/summarize_results_with_plans.py
--rw-r--r--   0 vincent    (501) staff       (20)     3938 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/region_based_evaluation.py
--rw-r--r--   0 vincent    (501) staff       (20)     2686 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/surface_dice.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.471039 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/
--rw-r--r--   0 vincent    (501) staff       (20)    11051 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.472809 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6754 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_11GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     6688 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_16GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     6752 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_32GB.py
--rw-r--r--   0 vincent    (501) staff       (20)     1932 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v21_3convperstage.py
--rw-r--r--   0 vincent    (501) staff       (20)     3151 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v22.py
--rw-r--r--   0 vincent    (501) staff       (20)     1337 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_baseline_3DUNet_v23.py
--rw-r--r--   0 vincent    (501) staff       (20)     2161 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_pretrained.py
--rw-r--r--   0 vincent    (501) staff       (20)     7402 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/experiment_planner_residual_3DUNet_v21.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.473508 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1625 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_2DUNet_v21_RGB_scaleto_0_1.py
--rw-r--r--   0 vincent    (501) staff       (20)     2016 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_CT2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1765 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/normalization/experiment_planner_3DUNet_nonCT.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.474021 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7015 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_mm.py
--rw-r--r--   0 vincent    (501) staff       (20)     6308 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/patch_size/experiment_planner_3DUNet_isotropic_in_voxels.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.474567 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     7697 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_allConv3x3.py
--rw-r--r--   0 vincent    (501) staff       (20)     6766 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/pooling_and_convs/experiment_planner_baseline_3DUNet_poolBasedOnSpacing.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.475277 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_targetSpacingForAnisoAxis.py
--rw-r--r--   0 vincent    (501) staff       (20)     1787 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_customTargetSpacing_2x2x2.py
--rw-r--r--   0 vincent    (501) staff       (20)    12203 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/alternative_experiment_planning/target_spacing/experiment_planner_baseline_3DUNet_v21_noResampling.py
--rw-r--r--   0 vincent    (501) staff       (20)      500 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/change_batch_size.py
--rw-r--r--   0 vincent    (501) staff       (20)    10562 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/common_utils.py
--rw-r--r--   0 vincent    (501) staff       (20)     8773 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     5784 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet_v21.py
--rw-r--r--   0 vincent    (501) staff       (20)    26524 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    10260 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet_v21.py
--rw-r--r--   0 vincent    (501) staff       (20)     4015 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/nnUNet_convert_decathlon_task.py
--rw-r--r--   0 vincent    (501) staff       (20)    10041 2023-04-05 08:06:36.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.475606 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/old/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/old/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     5224 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/old/old_plan_and_preprocess_task.py
--rw-r--r--   0 vincent    (501) staff       (20)     4189 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/summarize_plans.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.475824 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/task_specific_planner/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/task_specific_planner/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.476059 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    10497 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/task_specific_planner/amos2022/residual_bfnnunet_planner.py
--rw-r--r--   0 vincent    (501) staff       (20)     9635 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/utils.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.479679 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.479967 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/amos2022/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/amos2022/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    11488 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/amos2022/inference_code.py
--rw-r--r--   0 vincent    (501) staff       (20)     2631 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/change_trainer.py
--rw-r--r--   0 vincent    (501) staff       (20)     6300 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/ensemble_predictions.py
--rw-r--r--   0 vincent    (501) staff       (20)    44882 2023-05-01 15:47:02.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/predict.py
--rw-r--r--   0 vincent    (501) staff       (20)    13856 2023-05-01 15:47:01.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/predict_simple.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.480435 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/pretrained_models/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/pretrained_models/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    14181 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/pretrained_models/collect_pretrained_models.py
--rw-r--r--   0 vincent    (501) staff       (20)    23045 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/pretrained_models/download_pretrained_model.py
--rw-r--r--   0 vincent    (501) staff       (20)    12220 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/segmentation_export.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.482951 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.483845 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    12558 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/conv_blocks.py
--rw-r--r--   0 vincent    (501) staff       (20)     1547 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/feature_response_normalization.py
--rw-r--r--   0 vincent    (501) staff       (20)     1051 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py
--rw-r--r--   0 vincent    (501) staff       (20)      730 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/mish.py
--rw-r--r--   0 vincent    (501) staff       (20)    21046 2023-05-02 11:15:11.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     6839 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_UNet_DP.py
--rw-r--r--   0 vincent    (501) staff       (20)    20014 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_modular_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    27608 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_modular_preact_residual_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)    25056 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_modular_residual_UNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/initialization.py
--rw-r--r--   0 vincent    (501) staff       (20)    44012 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/neural_network.py
--rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/paths.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.484643 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    19122 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/connected_components.py
--rw-r--r--   0 vincent    (501) staff       (20)     3162 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/consolidate_all_for_paper.py
--rw-r--r--   0 vincent    (501) staff       (20)     4849 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing.py
--rw-r--r--   0 vincent    (501) staff       (20)     2729 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/consolidate_postprocessing_simple.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.485474 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/cropping.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.485747 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/custom_preprocessors/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/custom_preprocessors/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3475 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/custom_preprocessors/preprocessor_scale_RGB_to_0_1.py
--rw-r--r--   0 vincent    (501) staff       (20)    48208 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/preprocessing.py
--rw-r--r--   0 vincent    (501) staff       (20)    12201 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/sanity_checks.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.486826 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3818 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/default_configuration.py
--rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/load_pretrained_weights.py
--rw-r--r--   0 vincent    (501) staff       (20)    11797 2023-04-06 04:03:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/run_training.py
--rw-r--r--   0 vincent    (501) staff       (20)    11803 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/run_training_DDP.py
--rw-r--r--   0 vincent    (501) staff       (20)    11809 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/run_training_DP.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.487227 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.487625 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/cascade_stuff/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6237 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.489091 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
--rw-r--r--   0 vincent    (501) staff       (20)    11100 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py
--rw-r--r--   0 vincent    (501) staff       (20)    11280 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py
--rw-r--r--   0 vincent    (501) staff       (20)    12621 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     5012 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_noDA.py
--rw-r--r--   0 vincent    (501) staff       (20)    12938 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
--rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
--rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.489390 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/dataloading/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/dataloading/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    33671 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.489716 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/learning_rate/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/learning_rate/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.490601 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/
--rw-r--r--   0 vincent    (501) staff       (20)     1364 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
--rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
--rw-r--r--   0 vincent    (501) staff       (20)    13960 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
--rw-r--r--   0 vincent    (501) staff       (20)     7125 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/model_restore.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.492901 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.493087 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.494357 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    21314 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py
--rw-r--r--   0 vincent    (501) staff       (20)    14415 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.494728 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/__init__.py
--rwxr-xr-x   0 vincent    (501) staff       (20)     2662 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/MMS/nnUNetTrainerV2_MMS.py
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    31382 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/network_trainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    39860 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
--rw-r--r--   0 vincent    (501) staff       (20)    16064 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
--rw-r--r--   0 vincent    (501) staff       (20)    22667 2023-05-02 11:04:46.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
--rw-r--r--   0 vincent    (501) staff       (20)    19613 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
--rw-r--r--   0 vincent    (501) staff       (20)    34510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DDP.py
--rw-r--r--   0 vincent    (501) staff       (20)    11638 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_DP.py
--rw-r--r--   0 vincent    (501) staff       (20)     1225 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_fp32.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.495522 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/__init__.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.500135 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2271 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage.py
--rw-r--r--   0 vincent    (501) staff       (20)     2214 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_3ConvPerStage_samefilters.py
--rw-r--r--   0 vincent    (501) staff       (20)     2473 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_BN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2430 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_FRN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2379 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GN.py
--rw-r--r--   0 vincent    (501) staff       (20)     2829 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_GeLU.py
--rw-r--r--   0 vincent    (501) staff       (20)     2221 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_LReLU_slope_2en1.py
--rw-r--r--   0 vincent    (501) staff       (20)     2228 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_Mish.py
--rw-r--r--   0 vincent    (501) staff       (20)     2256 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization.py
--rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_NoNormalization_lr1en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2180 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU.py
--rw-r--r--   0 vincent    (501) staff       (20)     2258 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_biasInSegOutput.py
--rw-r--r--   0 vincent    (501) staff       (20)     2285 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ReLU_convReLUIN.py
--rw-r--r--   0 vincent    (501) staff       (20)     6082 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet.py
--rw-r--r--   0 vincent    (501) staff       (20)     6085 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2155 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_DA3_BN.py
--rw-r--r--   0 vincent    (501) staff       (20)     1582 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit.py
--rw-r--r--   0 vincent    (501) staff       (20)    19820 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_ResencUNet_SimonsInit_DA5.py
--rw-r--r--   0 vincent    (501) staff       (20)     2727 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_allConv3x3.py
--rw-r--r--   0 vincent    (501) staff       (20)     2288 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_biasInSegOutput.py
--rw-r--r--   0 vincent    (501) staff       (20)     2318 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_lReLU_convlReLUIN.py
--rw-r--r--   0 vincent    (501) staff       (20)     8834 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_noDeepSupervision.py
--rw-r--r--   0 vincent    (501) staff       (20)     6236 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/architectural_variants/nnUNetTrainerV2_softDeepSupervision.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.500631 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)    14098 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_2epochs.py
--rw-r--r--   0 vincent    (501) staff       (20)     6509 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/benchmarking/nnUNetTrainerV2_dummyLoad.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.501510 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     4283 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_DAVariants.py
--rw-r--r--   0 vincent    (501) staff       (20)     1321 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_lowerLR.py
--rw-r--r--   0 vincent    (501) staff       (20)     1324 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter.py
--rw-r--r--   0 vincent    (501) staff       (20)     1363 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/cascade/nnUNetTrainerV2CascadeFullRes_shorter_lowerLR.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.501828 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     2527 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/copies/nnUNetTrainerV2_copies.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.503298 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1182 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py
--rw-r--r--   0 vincent    (501) staff       (20)     9841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA3.py
--rw-r--r--   0 vincent    (501) staff       (20)    20353 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA5.py
--rw-r--r--   0 vincent    (501) staff       (20)      976 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py
--rw-r--r--   0 vincent    (501) staff       (20)     7727 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_insaneDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     7811 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noDA.py
--rw-r--r--   0 vincent    (501) staff       (20)     2321 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_noMirroring.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.505786 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1180 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceBD.py
--rw-r--r--   0 vincent    (501) staff       (20)     1181 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_ForceSD.py
--rw-r--r--   0 vincent    (501) staff       (20)     1276 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py
--rw-r--r--   0 vincent    (501) staff       (20)     1331 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CEGDL.py
--rw-r--r--   0 vincent    (501) staff       (20)     1936 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice.py
--rw-r--r--   0 vincent    (501) staff       (20)     1352 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py
--rw-r--r--   0 vincent    (501) staff       (20)     1382 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceTopK10.py
--rw-r--r--   0 vincent    (501) staff       (20)     1743 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_lr1en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     1462 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_Dice_squared.py
--rw-r--r--   0 vincent    (501) staff       (20)     1943 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_MCC.py
--rw-r--r--   0 vincent    (501) staff       (20)     1514 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_TopK10.py
--rw-r--r--   0 vincent    (501) staff       (20)     1469 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_focalLoss.py
--rw-r--r--   0 vincent    (501) staff       (20)     2667 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_graduallyTransitionFromCEToDice.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.506166 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     9982 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/miscellaneous/nnUNetTrainerV2_fullEvals.py
--rw-r--r--   0 vincent    (501) staff       (20)     1304 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerCE.py
--rw-r--r--   0 vincent    (501) staff       (20)     4489 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/nnUNetTrainerNoDA.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.509671 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     1245 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam.py
--rw-r--r--   0 vincent    (501) staff       (20)     2899 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_ReduceOnPlateau.py
--rw-r--r--   0 vincent    (501) staff       (20)     1246 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Adam_lr_3en4.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr1en2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en3.py
--rw-r--r--   0 vincent    (501) staff       (20)     1493 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_Ranger_lr3en4.py
--rw-r--r--   0 vincent    (501) staff       (20)     2707 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_ReduceOnPlateau.py
--rw-r--r--   0 vincent    (501) staff       (20)     1808 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule.py
--rw-r--r--   0 vincent    (501) staff       (20)     1950 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_fixedSchedule2.py
--rw-r--r--   0 vincent    (501) staff       (20)     1610 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_SGD_lrs.py
--rw-r--r--   0 vincent    (501) staff       (20)     3693 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_cycleAtEnd.py
--rw-r--r--   0 vincent    (501) staff       (20)     1206 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_fp16.py
--rw-r--r--   0 vincent    (501) staff       (20)     1192 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09.py
--rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum095.py
--rw-r--r--   0 vincent    (501) staff       (20)     1194 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum098.py
--rw-r--r--   0 vincent    (501) staff       (20)     1293 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_momentum09in2D.py
--rw-r--r--   0 vincent    (501) staff       (20)     1947 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_reduceMomentumDuringTraining.py
--rw-r--r--   0 vincent    (501) staff       (20)     1756 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/optimizer_and_lr/nnUNetTrainerV2_warmup.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.510027 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3472 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/resampling/nnUNetTrainerV2_resample33.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.510354 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/optimizer/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/optimizer/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/optimizer/ranger.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.513231 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/
--rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)     3172 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/distributed.py
--rw-r--r--   0 vincent    (501) staff       (20)     4533 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/file_conversions.py
--rw-r--r--   0 vincent    (501) staff       (20)     1130 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/file_endings.py
--rw-r--r--   0 vincent    (501) staff       (20)     1810 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/folder_names.py
--rw-r--r--   0 vincent    (501) staff       (20)     4564 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/image_reorientation.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/nd_softmax.py
--rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/one_hot_encoding.py
--rw-r--r--   0 vincent    (501) staff       (20)     8434 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/overlay_plots.py
--rw-r--r--   0 vincent    (501) staff       (20)      794 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/random_stuff.py
--rw-r--r--   0 vincent    (501) staff       (20)     1554 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/recursive_delete_npz.py
--rw-r--r--   0 vincent    (501) staff       (20)     1770 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py
--rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
--rw-r--r--   0 vincent    (501) staff       (20)      908 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/sitk_stuff.py
--rw-r--r--   0 vincent    (501) staff       (20)     3514 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
--rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/tensor_utilities.py
--rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/to_torch.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 07:10:05.457823 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)    22209 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)     2023 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)      151 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/requires.txt
--rw-r--r--   0 vincent    (501) staff       (20)       18 2023-06-30 07:10:05.000000 CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet.egg-info/top_level.txt
--rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUNet-1.7.3/LICENSE
--rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 07:10:05.513504 CartiMorph_nnUNet-1.7.3/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      640 2023-06-30 07:07:38.000000 CartiMorph_nnUNet-1.7.3/README.md
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 07:10:05.513717 CartiMorph_nnUNet-1.7.3/setup.cfg
--rwxr-xr-x   0 vincent    (501) staff       (20)     3430 2023-06-30 07:09:24.000000 CartiMorph_nnUNet-1.7.3/setup.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.198587 CartiMorph_nnUNet-1.7.4/
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.182705 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/
+-rw-r--r--   0 vincent    (501) staff       (20)      617 2023-06-30 09:17:56.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      257 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/configuration.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.184746 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    18791 2023-06-30 08:19:24.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/evaluator.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13031 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/metrics.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.186095 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/
+-rw-r--r--   0 vincent    (501) staff       (20)    11084 2023-06-30 08:07:52.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10573 2023-06-30 08:09:29.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/common_utils.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8872 2023-06-30 08:16:19.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    26645 2023-06-30 08:15:35.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)    10184 2023-06-30 08:17:41.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9703 2023-06-30 08:08:55.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/utils.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.186828 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44937 2023-06-30 08:05:12.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/predict.py
+-rw-r--r--   0 vincent    (501) staff       (20)    13889 2023-06-30 07:22:30.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/predict_simple.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12231 2023-06-30 08:35:08.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/segmentation_export.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.187477 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    21079 2023-06-30 08:12:26.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/generic_UNet.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1673 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/initialization.py
+-rw-r--r--   0 vincent    (501) staff       (20)    44034 2023-06-30 08:13:21.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/neural_network.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2949 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/paths.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.187801 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/postprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/postprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19155 2023-06-30 08:35:41.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/postprocessing/connected_components.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.188816 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8571 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/cropping.py
+-rw-r--r--   0 vincent    (501) staff       (20)    48230 2023-06-30 08:16:03.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/preprocessing.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12212 2023-06-30 08:17:17.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/sanity_checks.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.189473 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3884 2023-06-30 07:56:39.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/default_configuration.py
+-rw-r--r--   0 vincent    (501) staff       (20)     2504 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/load_pretrained_weights.py
+-rw-r--r--   0 vincent    (501) staff       (20)    11918 2023-06-30 08:04:26.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/run_training.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.189756 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/__init__.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.190056 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/cascade_stuff/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/cascade_stuff/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6325 2023-06-30 07:59:12.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.191112 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4841 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12665 2023-06-30 08:47:23.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py
+-rw-r--r--   0 vincent    (501) staff       (20)    12993 2023-06-30 08:38:21.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4137 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/downsampling.py
+-rw-r--r--   0 vincent    (501) staff       (20)     9029 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.191416 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/dataloading/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/dataloading/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    33693 2023-06-30 08:37:03.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/dataloading/dataset_loading.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.191789 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/learning_rate/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/learning_rate/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      807 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/learning_rate/poly_lr.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.192705 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/
+-rw-r--r--   0 vincent    (501) staff       (20)     1375 2023-06-30 08:39:27.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      438 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/crossentropy.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1679 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py
+-rw-r--r--   0 vincent    (501) staff       (20)    14004 2023-06-30 08:40:47.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/dice_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7847 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/focal_loss.py
+-rw-r--r--   0 vincent    (501) staff       (20)     7202 2023-06-30 08:14:47.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/model_restore.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.193908 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)    31404 2023-06-30 08:41:20.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/network_trainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    40059 2023-06-30 08:00:59.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py
+-rw-r--r--   0 vincent    (501) staff       (20)    16163 2023-06-30 08:01:58.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py
+-rw-r--r--   0 vincent    (501) staff       (20)    22788 2023-06-30 08:49:46.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py
+-rw-r--r--   0 vincent    (501) staff       (20)    19734 2023-06-30 08:02:22.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.194217 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/optimizer/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/optimizer/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     6465 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/optimizer/ranger.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.198062 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/
+-rw-r--r--   0 vincent    (501) staff       (20)       54 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3172 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/distributed.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4533 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/file_conversions.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1130 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/file_endings.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1810 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/folder_names.py
+-rw-r--r--   0 vincent    (501) staff       (20)     4564 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/image_reorientation.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-05-01 14:25:34.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/nd_softmax.py
+-rw-r--r--   0 vincent    (501) staff       (20)      990 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/one_hot_encoding.py
+-rw-r--r--   0 vincent    (501) staff       (20)     8434 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/overlay_plots.py
+-rw-r--r--   0 vincent    (501) staff       (20)      794 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/random_stuff.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1554 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/recursive_delete_npz.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1770 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1510 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/set_n_proc_DA.py
+-rw-r--r--   0 vincent    (501) staff       (20)      908 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/sitk_stuff.py
+-rw-r--r--   0 vincent    (501) staff       (20)     3525 2023-06-30 08:04:03.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/task_name_id_conversion.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1624 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/tensor_utilities.py
+-rw-r--r--   0 vincent    (501) staff       (20)     1175 2023-02-05 08:08:10.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/to_torch.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-06-30 09:18:11.183817 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)     4212 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      270 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)      151 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/requires.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       18 2023-06-30 09:18:11.000000 CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet.egg-info/top_level.txt
+-rw-r--r--   0 vincent    (501) staff       (20)    11357 2023-06-30 06:10:04.000000 CartiMorph_nnUNet-1.7.4/LICENSE
+-rw-r--r--   0 vincent    (501) staff       (20)      434 2023-06-30 09:18:11.198440 CartiMorph_nnUNet-1.7.4/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      640 2023-06-30 07:07:38.000000 CartiMorph_nnUNet-1.7.4/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-06-30 09:18:11.198635 CartiMorph_nnUNet-1.7.4/setup.cfg
+-rwxr-xr-x   0 vincent    (501) staff       (20)     1421 2023-06-30 09:17:44.000000 CartiMorph_nnUNet-1.7.4/setup.py
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/__init__.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# set version
-__version__ = '1.7.3'
-
 from __future__ import absolute_import
 
 print("\n\nThis is a modified version of nnU-Net (1.7.0) tailored for the CartiMorph framework (https://github.com/YongchengYAO/CartiMorph).")
 print("\nIf you are using CartiMorph, please cite the paper:")
 print("\n[paper-holder]")
 
 print("\n\nPlease cite the following paper when using nnUNet:\nIsensee, F., Jaeger, P.F., Kohl, S.A.A. et al. "
       "\"nnU-Net: a self-configuring method for deep learning-based biomedical image segmentation.\" "
       "Nat Methods (2020). https://doi.org/10.1038/s41592-020-01008-z\n\n")
 
-from . import *
+from . import *
+
+# set version
+__version__ = '1.7.4'
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task114_heart_MNMs.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/sanity_checks.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,255 +8,267 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import shutil
-from collections import OrderedDict
 
+from multiprocessing import Pool
+
+import SimpleITK as sitk
+import nibabel as nib
 import numpy as np
-import pandas as pd
 from batchgenerators.utilities.file_and_folder_operations import *
-from numpy.random.mtrand import RandomState
+from CartiMorph_nnUNet.configuration import default_num_threads
+
 
-from nnunet.experiment_planning.common_utils import split_4d_nifti
+def verify_all_same_orientation(folder):
+    """
+    This should run after cropping
+    :param folder:
+    :return:
+    """
+    nii_files = subfiles(folder, suffix=".nii.gz", join=True)
+    orientations = []
+    for n in nii_files:
+        img = nib.load(n)
+        affine = img.affine
+        orientation = nib.aff2axcodes(affine)
+        orientations.append(orientation)
+    # now we need to check whether they are all the same
+    orientations = np.array(orientations)
+    unique_orientations = np.unique(orientations, axis=0)
+    all_same = len(unique_orientations) == 1
+    return all_same, unique_orientations
+
+
+def verify_same_geometry(img_1: sitk.Image, img_2: sitk.Image):
+    ori1, spacing1, direction1, size1 = img_1.GetOrigin(), img_1.GetSpacing(), img_1.GetDirection(), img_1.GetSize()
+    ori2, spacing2, direction2, size2 = img_2.GetOrigin(), img_2.GetSpacing(), img_2.GetDirection(), img_2.GetSize()
+
+    same_ori = np.all(np.isclose(ori1, ori2))
+    if not same_ori:
+        print("the origin does not match between the images:")
+        print(ori1)
+        print(ori2)
+
+    same_spac = np.all(np.isclose(spacing1, spacing2))
+    if not same_spac:
+        print("the spacing does not match between the images")
+        print(spacing1)
+        print(spacing2)
+
+    same_dir = np.all(np.isclose(direction1, direction2))
+    if not same_dir:
+        print("the direction does not match between the images")
+        print(direction1)
+        print(direction2)
+
+    same_size = np.all(np.isclose(size1, size2))
+    if not same_size:
+        print("the size does not match between the images")
+        print(size1)
+        print(size2)
+
+    if same_ori and same_spac and same_dir and same_size:
+        return True
+    else:
+        return False
 
 
-def get_mnms_data(data_root):
-    files_raw = []
-    files_gt = []
-    for r, dirs, files in os.walk(data_root):
-        for f in files:
-            if f.endswith('nii.gz'):
-                file_path = os.path.join(r, f)
-                if '_gt' in f:
-                    files_gt.append(file_path)
-                else:
-                    files_raw.append(file_path)
-    return files_raw, files_gt
-
-
-def generate_filename_for_nnunet(pat_id, ts, pat_folder=None, add_zeros=False, vendor=None, centre=None, mode='mnms',
-                                 data_format='nii.gz'):
-    if not vendor or not centre:
-        if add_zeros:
-            filename = "{}_{}_0000.{}".format(pat_id, str(ts).zfill(4), data_format)
-        else:
-            filename = "{}_{}.{}".format(pat_id, str(ts).zfill(4), data_format)
+def verify_contains_only_expected_labels(itk_img: str, valid_labels: (tuple, list)):
+    img_npy = sitk.GetArrayFromImage(sitk.ReadImage(itk_img))
+    uniques = np.unique(img_npy)
+    invalid_uniques = [i for i in uniques if i not in valid_labels]
+    if len(invalid_uniques) == 0:
+        r = True
     else:
-        if mode == 'mnms':
-            if add_zeros:
-                filename = "{}_{}_{}_{}_0000.{}".format(pat_id, str(ts).zfill(4), vendor, centre, data_format)
-            else:
-                filename = "{}_{}_{}_{}.{}".format(pat_id, str(ts).zfill(4), vendor, centre, data_format)
-        else:
-            if add_zeros:
-                filename = "{}_{}_{}_{}_0000.{}".format(vendor, centre, pat_id, str(ts).zfill(4), data_format)
-            else:
-                filename = "{}_{}_{}_{}.{}".format(vendor, centre, pat_id, str(ts).zfill(4), data_format)
-
-    if pat_folder:
-        filename = os.path.join(pat_folder, filename)
-    return filename
-
-
-def select_annotated_frames_mms(data_folder, out_folder, add_zeros=False, is_gt=False,
-                                df_path="/media/full/tera2/data/challenges/mms/Training-corrected_original/M&Ms Dataset Information.xlsx",
-                                mode='mnms',):
-    table = pd.read_excel(df_path, index_col='External code')
-
-    for idx in table.index:
-        ed = table.loc[idx, 'ED']
-        es = table.loc[idx, 'ES']
-        vendor = table.loc[idx, 'Vendor']
-        centre = table.loc[idx, 'Centre']
-
-        if vendor != "C": # vendor C is for test data
-
-            # this step is needed in case of M&Ms data to adjust it to the nnUNet frame work
-            # generate old filename (w/o vendor and centre)
-            if is_gt:
-                add_to_name = 'sa_gt'
-            else:
-                add_to_name = 'sa'
-            filename_ed_original = os.path.join(
-                data_folder, "{}_{}_{}.nii.gz".format(idx, add_to_name, str(ed).zfill(4)))
-            filename_es_original = os.path.join(
-                data_folder, "{}_{}_{}.nii.gz".format(idx, add_to_name, str(es).zfill(4)))
-
-            # generate new filename with vendor and centre
-            filename_ed = generate_filename_for_nnunet(pat_id=idx, ts=ed, pat_folder=out_folder,
-                                                       vendor=vendor, centre=centre, add_zeros=add_zeros, mode=mode)
-            filename_es = generate_filename_for_nnunet(pat_id=idx, ts=es, pat_folder=out_folder,
-                                                       vendor=vendor, centre=centre, add_zeros=add_zeros, mode=mode)
-
-            shutil.copy(filename_ed_original, filename_ed)
-            shutil.copy(filename_es_original, filename_es)
-
-
-def create_custom_splits_for_experiments(task_path):
-    data_keys = [i[:-4] for i in
-                 subfiles(os.path.join(task_path, "nnUNetData_plans_v2.1_2D_stage0"),
-                          join=False, suffix='npz')]
-    existing_splits = os.path.join(task_path, "splits_final.pkl")
-
-    splits = load_pickle(existing_splits)
-    splits = splits[:5]  # discard old changes
-
-    unique_a_only = np.unique([i.split('_')[0] for i in data_keys if i.find('_A_') != -1])
-    unique_b_only = np.unique([i.split('_')[0] for i in data_keys if i.find('_B_') != -1])
-
-    num_train_a = int(np.round(0.8 * len(unique_a_only)))
-    num_train_b = int(np.round(0.8 * len(unique_b_only)))
-
-    p = RandomState(1234)
-    idx_a_train = p.choice(len(unique_a_only), num_train_a, replace=False)
-    idx_b_train = p.choice(len(unique_b_only), num_train_b, replace=False)
-
-    identifiers_a_train = [unique_a_only[i] for i in idx_a_train]
-    identifiers_b_train = [unique_b_only[i] for i in idx_b_train]
-
-    identifiers_a_val = [i for i in unique_a_only if i not in identifiers_a_train]
-    identifiers_b_val = [i for i in unique_b_only if i not in identifiers_b_train]
-
-    # fold 5 will be train on a and eval on val sets of a and b
-    splits.append({'train': [i for i in data_keys if i.split("_")[0] in identifiers_a_train],
-                   'val': [i for i in data_keys if i.split("_")[0] in identifiers_a_val] + [i for i in data_keys if
-                                                                                            i.split("_")[
-                                                                                                0] in identifiers_b_val]})
-
-    # fold 6 will be train on b and eval on val sets of a and b
-    splits.append({'train': [i for i in data_keys if i.split("_")[0] in identifiers_b_train],
-                   'val': [i for i in data_keys if i.split("_")[0] in identifiers_a_val] + [i for i in data_keys if
-                                                                                            i.split("_")[
-                                                                                                0] in identifiers_b_val]})
-
-    # fold 7 train on both, eval on both
-    splits.append({'train': [i for i in data_keys if i.split("_")[0] in identifiers_b_train] + [i for i in data_keys if i.split("_")[0] in identifiers_a_train],
-                   'val': [i for i in data_keys if i.split("_")[0] in identifiers_a_val] + [i for i in data_keys if
-                                                                                            i.split("_")[
-                                                                                                0] in identifiers_b_val]})
-    save_pickle(splits, existing_splits)
+        r = False
+    return r, invalid_uniques
+
+
+def verify_dataset_integrity(folder):
+    """
+    folder needs the imagesTr, imagesTs and labelsTr subfolders. There also needs to be a dataset.json
+    checks if all training cases and labels are present
+    checks if all test cases (if any) are present
+    for each case, checks whether all modalities apre present
+    for each case, checks whether the pixel grids are aligned
+    checks whether the labels really only contain values they should
+    :param folder:
+    :return:
+    """
+    assert isfile(join(folder, "dataset.json")), "There needs to be a dataset.json file in folder, folder=%s" % folder
+    assert isdir(join(folder, "imagesTr")), "There needs to be a imagesTr subfolder in folder, folder=%s" % folder
+    assert isdir(join(folder, "labelsTr")), "There needs to be a labelsTr subfolder in folder, folder=%s" % folder
+    dataset = load_json(join(folder, "dataset.json"))
+    training_cases = dataset['training']
+    num_modalities = len(dataset['modality'].keys())
+    test_cases = dataset['test']
+    expected_train_identifiers = [i['image'].split("/")[-1][:-7] for i in training_cases]
+    expected_test_identifiers = [i.split("/")[-1][:-7] for i in test_cases]
+
+    ## check training set
+    nii_files_in_imagesTr = subfiles((join(folder, "imagesTr")), suffix=".nii.gz", join=False)
+    nii_files_in_labelsTr = subfiles((join(folder, "labelsTr")), suffix=".nii.gz", join=False)
+
+    label_files = []
+    geometries_OK = True
+    has_nan = False
+
+    # check all cases
+    if len(expected_train_identifiers) != len(np.unique(expected_train_identifiers)): raise RuntimeError("found duplicate training cases in dataset.json")
+
+    print("Verifying training set")
+    for c in expected_train_identifiers:
+        print("checking case", c)
+        # check if all files are present
+        expected_label_file = join(folder, "labelsTr", c + ".nii.gz")
+        label_files.append(expected_label_file)
+        expected_image_files = [join(folder, "imagesTr", c + "_%04.0d.nii.gz" % i) for i in range(num_modalities)]
+        assert isfile(expected_label_file), "could not find label file for case %s. Expected file: \n%s" % (
+            c, expected_label_file)
+        assert all([isfile(i) for i in
+                    expected_image_files]), "some image files are missing for case %s. Expected files:\n %s" % (
+            c, expected_image_files)
+
+        # verify that all modalities and the label have the same shape and geometry.
+        label_itk = sitk.ReadImage(expected_label_file)
+
+        nans_in_seg = np.any(np.isnan(sitk.GetArrayFromImage(label_itk)))
+        has_nan = has_nan | nans_in_seg
+        if nans_in_seg:
+            print("There are NAN values in segmentation %s" % expected_label_file)
+
+        images_itk = [sitk.ReadImage(i) for i in expected_image_files]
+        for i, img in enumerate(images_itk):
+            nans_in_image = np.any(np.isnan(sitk.GetArrayFromImage(img)))
+            has_nan = has_nan | nans_in_image
+            same_geometry = verify_same_geometry(img, label_itk)
+            if not same_geometry:
+                geometries_OK = False
+                print("The geometry of the image %s does not match the geometry of the label file. The pixel arrays "
+                      "will not be aligned and nnU-Net cannot use this data. Please make sure your image modalities "
+                      "are coregistered and have the same geometry as the label" % expected_image_files[0][:-12])
+            if nans_in_image:
+                print("There are NAN values in image %s" % expected_image_files[i])
+
+        # now remove checked files from the lists nii_files_in_imagesTr and nii_files_in_labelsTr
+        for i in expected_image_files:
+            nii_files_in_imagesTr.remove(os.path.basename(i))
+        nii_files_in_labelsTr.remove(os.path.basename(expected_label_file))
+
+    # check for stragglers
+    assert len(
+        nii_files_in_imagesTr) == 0, "there are training cases in imagesTr that are not listed in dataset.json: %s" % nii_files_in_imagesTr
+    assert len(
+        nii_files_in_labelsTr) == 0, "there are training cases in labelsTr that are not listed in dataset.json: %s" % nii_files_in_labelsTr
+
+    # verify that only properly declared values are present in the labels
+    print("Verifying label values")
+    expected_labels = list(int(i) for i in dataset['labels'].keys())
+    expected_labels.sort()
+
+    # check if labels are in consecutive order
+    assert expected_labels[0] == 0, 'The first label must be 0 and maps to the background'
+    labels_valid_consecutive = np.ediff1d(expected_labels) == 1
+    assert all(labels_valid_consecutive), f'Labels must be in consecutive order (0, 1, 2, ...). The labels {np.array(expected_labels)[1:][~labels_valid_consecutive]} do not satisfy this restriction'
+
+    p = Pool(default_num_threads)
+    results = p.starmap(verify_contains_only_expected_labels, zip(label_files, [expected_labels] * len(label_files)))
+    p.close()
+    p.join()
+
+    fail = False
+    print("Expected label values are", expected_labels)
+    for i, r in enumerate(results):
+        if not r[0]:
+            print("Unexpected labels found in file %s. Found these unexpected values (they should not be there) %s" % (
+                label_files[i], r[1]))
+            fail = True
+
+    if fail:
+        raise AssertionError(
+            "Found unexpected labels in the training dataset. Please correct that or adjust your dataset.json accordingly")
+    else:
+        print("Labels OK")
+
+    # check test set, but only if there actually is a test set
+    if len(expected_test_identifiers) > 0:
+        print("Verifying test set")
+        nii_files_in_imagesTs = subfiles((join(folder, "imagesTs")), suffix=".nii.gz", join=False)
+
+        for c in expected_test_identifiers:
+            # check if all files are present
+            expected_image_files = [join(folder, "imagesTs", c + "_%04.0d.nii.gz" % i) for i in range(num_modalities)]
+            assert all([isfile(i) for i in
+                        expected_image_files]), "some image files are missing for case %s. Expected files:\n %s" % (
+                c, expected_image_files)
+
+            # verify that all modalities and the label have the same geometry. We use the affine for this
+            if num_modalities > 1:
+                images_itk = [sitk.ReadImage(i) for i in expected_image_files]
+                reference_img = images_itk[0]
+
+                for i, img in enumerate(images_itk[1:]):
+                    assert verify_same_geometry(img, reference_img), "The modalities of the image %s do not seem to be " \
+                                                                     "registered. Please coregister your modalities." % (
+                                                                         expected_image_files[i])
+
+            # now remove checked files from the lists nii_files_in_imagesTr and nii_files_in_labelsTr
+            for i in expected_image_files:
+                nii_files_in_imagesTs.remove(os.path.basename(i))
+        assert len(
+            nii_files_in_imagesTs) == 0, "there are training cases in imagesTs that are not listed in dataset.json: %s" % nii_files_in_imagesTr
+
+    all_same, unique_orientations = verify_all_same_orientation(join(folder, "imagesTr"))
+    if not all_same:
+        print(
+            "WARNING: Not all images in the dataset have the same axis ordering. We very strongly recommend you correct that by reorienting the data. fslreorient2std should do the trick")
+    # save unique orientations to dataset.json
+    if not geometries_OK:
+        raise Warning("GEOMETRY MISMATCH FOUND! CHECK THE TEXT OUTPUT! This does not cause an error at this point  but you should definitely check whether your geometries are alright!")
+    else:
+        print("Dataset OK")
+
+    if has_nan:
+        raise RuntimeError("Some images have nan values in them. This will break the training. See text output above to see which ones")
+
+
+def reorient_to_RAS(img_fname: str, output_fname: str = None):
+    img = nib.load(img_fname)
+    canonical_img = nib.as_closest_canonical(img)
+    if output_fname is None:
+        output_fname = img_fname
+    nib.save(canonical_img, output_fname)
 
 
 if __name__ == "__main__":
-    # this script will split 4d data from the M&Ms data set into 3d images for both, raw images and gt annotations.
-    # after this script you will be able to start a training on the M&Ms data.
-    # use this script as inspiration in case other data than M&Ms data is use for training.
-    #
-    # check also the comments at the END of the script for instructions on how to run the actual training after this
-    # script
-    #
-
-    # define a task ID for your experiment (I have choosen 114)
-    task_name = "Task679_heart_mnms"
-    # this is where the downloaded data from the M&Ms challenge shall be placed
-    raw_data_dir = "/media/full/tera2/data"
-    # set path to official ***M&Ms Dataset Information.xlsx*** file
-    df_path = "/media/full/tera2/data/challenges/mms/Training-corrected_original/M&Ms Dataset Information.xlsx"
-    # don't make changes here
-    folder_imagesTr = "imagesTr"
-    train_dir = os.path.join(raw_data_dir, task_name, folder_imagesTr)
-
-    # this is where our your splitted files WITH annotation will be stored. Dont make changes here. Otherwise nnUNet
-    # might have problems finding the training data later during the training process
-    out_dir = os.path.join(os.environ.get('nnUNet_raw_data_base'), 'nnUNet_raw_data', task_name)
-
-    files_raw, files_gt = get_mnms_data(data_root=train_dir)
-
-    filesTs, _ = get_mnms_data(data_root=train_dir)
-
-    split_path_raw_all_ts = os.path.join(raw_data_dir, task_name, "splitted_all_timesteps", folder_imagesTr,
-                                         "split_raw_images")
-    split_path_gt_all_ts = os.path.join(raw_data_dir, task_name, "splitted_all_timesteps", folder_imagesTr,
-                                        "split_annotation")
-    maybe_mkdir_p(split_path_raw_all_ts)
-    maybe_mkdir_p(split_path_gt_all_ts)
-
-    # for fast splitting of many patients use the following lines
-    # however keep in mind that these lines cause problems for some users.
-    # If problems occur use the code for loops below
-    # print("splitting raw 4d images into 3d images")
-    # split_4d_for_all_pat(files_raw, split_path_raw)
-    # print("splitting ground truth 4d into 3d files")
-    # split_4d_for_all_pat(files_gt, split_path_gt_all_ts)
-
-    print("splitting raw 4d images into 3d images")
-    for f in files_raw:
-        print("splitting {}".format(f))
-        split_4d_nifti(f, split_path_raw_all_ts)
-    print("splitting ground truth 4d into 3d files")
-    for gt in files_gt:
-        split_4d_nifti(gt, split_path_gt_all_ts)
-        print("splitting {}".format(gt))
-
-    print("prepared data will be saved at: {}".format(out_dir))
-    maybe_mkdir_p(join(out_dir, "imagesTr"))
-    maybe_mkdir_p(join(out_dir, "labelsTr"))
-
-    imagesTr_path = os.path.join(out_dir, "imagesTr")
-    labelsTr_path = os.path.join(out_dir, "labelsTr")
-    # only a small fraction of all timestep in the cardiac cycle possess gt annotation. These timestep will now be
-    # selected
-    select_annotated_frames_mms(split_path_raw_all_ts, imagesTr_path, add_zeros=True, is_gt=False, df_path=df_path)
-    select_annotated_frames_mms(split_path_gt_all_ts, labelsTr_path, add_zeros=False, is_gt=True, df_path=df_path)
-
-    labelsTr = subfiles(labelsTr_path)
-
-    # create a json file that will be needed by nnUNet to initiate the preprocessing process
-    json_dict = OrderedDict()
-    json_dict['name'] = "M&Ms"
-    json_dict['description'] = "short axis cardiac cine MRI segmentation"
-    json_dict['tensorImageSize'] = "4D"
-    json_dict['reference'] = "Campello, Victor M et al. “Multi-Centre, Multi-Vendor and Multi-Disease Cardiac " \
-                             "Segmentation: The M&Ms Challenge.” IEEE transactions on " \
-                             "medical imaging vol. 40,12 (2021): 3543-3554. doi:10.1109/TMI.2021.3090082"
-    json_dict['licence'] = "see M&Ms challenge"
-    json_dict['release'] = "0.0"
-    json_dict['modality'] = {
-        "0": "MRI",
-    }
-    # labels differ for ACDC challenge
-    json_dict['labels'] = {
-        "0": "background",
-        "1": "LVBP",
-        "2": "LVM",
-        "3": "RV"
-    }
-    json_dict['numTraining'] = len(labelsTr)
-    json_dict['numTest'] = 0
-    json_dict['training'] = [{'image': "./imagesTr/%s" % i.split("/")[-1],
-                              "label": "./labelsTr/%s" % i.split("/")[-1]} for i in labelsTr]
-    json_dict['test'] = []
-
-    save_json(json_dict, os.path.join(out_dir, "dataset.json"))
-
-    #
-    # now the data is ready to be preprocessed by the nnUNet
-    # the following steps are only needed if you want to reproduce the exact results from the MMS challenge
-    #
-
-
-    # then preprocess data and plan training.
-    # run in terminal
-    # nnUNet_plan_and_preprocess -t 114 --verify_dataset_integrity # for 2d
-    # nnUNet_plan_and_preprocess -t 114 --verify_dataset_integrity -pl3d ExperimentPlannerTargetSpacingForAnisoAxis # for 3d
-
-    # start training and stop it immediately to get a split.pkl file
-    # nnUNet_train 2d nnUNetTrainerV2_MMS 114 0
-
-    #
-    # then create custom splits as used for the final M&Ms submission
-    #
-
-    # in this file comment everything except for the following line
-    # create_custom_splits_for_experiments(out_dir)
-
-    # then start training with
-    #
-    # nnUNet_train 3d_fullres nnUNetTrainerV2_MMS Task114_heart_mnms -p nnUNetPlanstargetSpacingForAnisoAxis 0 # for 3d and fold 0
-    # and
-    # nnUNet_train 2d nnUNetTrainerV2_MMS Task114_heart_mnms 0 # for 2d and fold 0
+    # investigate geometry issues
+    import SimpleITK as sitk
+
+    # load image
+    gt_itk = sitk.ReadImage(
+        "/media/fabian/Results/nnUNet/3d_fullres/Task064_KiTS_labelsFixed/nnUNetTrainerV2__nnUNetPlansv2.1/gt_niftis/case_00085.nii.gz")
+
+    # get numpy array
+    pred_npy = sitk.GetArrayFromImage(gt_itk)
+
+    # create new image from numpy array
+    prek_itk_new = sitk.GetImageFromArray(pred_npy)
+    # copy geometry
+    prek_itk_new.CopyInformation(gt_itk)
+    # prek_itk_new = copy_geometry(prek_itk_new, gt_itk)
+
+    # save
+    sitk.WriteImage(prek_itk_new, "test.mnc")
+
+    # load images in nib
+    gt = nib.load(
+        "/media/fabian/Results/nnUNet/3d_fullres/Task064_KiTS_labelsFixed/nnUNetTrainerV2__nnUNetPlansv2.1/gt_niftis/case_00085.nii.gz")
+    pred_nib = nib.load("test.mnc")
 
+    new_img_sitk = sitk.ReadImage("test.mnc")
 
+    np1 = sitk.GetArrayFromImage(gt_itk)
+    np2 = sitk.GetArrayFromImage(prek_itk_new)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/dataset_conversion/Task155_RibFrac_binary.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/overlay_plots.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,174 +1,204 @@
-import SimpleITK as sitk
-from natsort import natsorted
+#    Copyright 2020 Division of Medical Image Computing, German Cancer Research Center (DKFZ), Heidelberg, Germany
+#
+#    Licensed under the Apache License, Version 2.0 (the "License");
+#    you may not use this file except in compliance with the License.
+#    You may obtain a copy of the License at
+#
+#        http://www.apache.org/licenses/LICENSE-2.0
+#
+#    Unless required by applicable law or agreed to in writing, software
+#    distributed under the License is distributed on an "AS IS" BASIS,
+#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#    See the License for the specific language governing permissions and
+#    limitations under the License.
+from multiprocessing.pool import Pool
+
 import numpy as np
-from pathlib import Path
-import pandas as pd
-from collections import defaultdict
-from shutil import copyfile
-import os
-from os.path import join
-from tqdm import tqdm
-import gc
-import multiprocessing as mp
-from nnunet.dataset_conversion.utils import generate_dataset_json
-from functools import partial
-
-
-def preprocess_dataset(dataset_load_path, dataset_save_path, pool):
-    train_image_load_path = join(dataset_load_path, "imagesTr")
-    train_mask_load_path = join(dataset_load_path, "labelsTr")
-    test_image_load_path = join(dataset_load_path, "imagesTs")
-
-    ribfrac_train_info_1_path = join(dataset_load_path, "ribfrac-train-info-1.csv")
-    ribfrac_train_info_2_path = join(dataset_load_path, "ribfrac-train-info-2.csv")
-    ribfrac_val_info_path = join(dataset_load_path, "ribfrac-val-info.csv")
-
-    train_image_save_path = join(dataset_save_path, "imagesTr")
-    train_mask_save_path = join(dataset_save_path, "labelsTr")
-    test_image_save_path = join(dataset_save_path, "imagesTs")
-    Path(train_image_save_path).mkdir(parents=True, exist_ok=True)
-    Path(train_mask_save_path).mkdir(parents=True, exist_ok=True)
-    Path(test_image_save_path).mkdir(parents=True, exist_ok=True)
-
-    meta_data = preprocess_csv(ribfrac_train_info_1_path, ribfrac_train_info_2_path, ribfrac_val_info_path)
-    preprocess_train(train_image_load_path, train_mask_load_path, meta_data, dataset_save_path, pool)
-    preprocess_test(test_image_load_path, dataset_save_path)
-
-
-def preprocess_csv(ribfrac_train_info_1_path, ribfrac_train_info_2_path, ribfrac_val_info_path):
-    print("Processing csv...")
-    meta_data = defaultdict(list)
-    for csv_path in [ribfrac_train_info_1_path, ribfrac_train_info_2_path, ribfrac_val_info_path]:
-        df = pd.read_csv(csv_path)
-        for index, row in df.iterrows():
-            name = row["public_id"]
-            instance = row["label_id"]
-            class_label = row["label_code"]
-            meta_data[name].append({"instance": instance, "class_label": class_label})
-    print("Finished csv processing.")
-    return meta_data
-
-
-def preprocess_train(image_path, mask_path, meta_data, save_path, pool):
-    print("Processing train data...")
-    pool.map(partial(preprocess_train_single, image_path=image_path, mask_path=mask_path, meta_data=meta_data, save_path=save_path), meta_data.keys())
-    print("Finished processing train data.")
-
-
-def preprocess_train_single(name, image_path, mask_path, meta_data, save_path):
-    id = int(name[7:])
-    image, _, _, _ = load_image(join(image_path, name + "-image.nii.gz"), return_meta=True, is_seg=False)
-    instance_seg_mask, spacing, _, _ = load_image(join(mask_path, name + "-label.nii.gz"), return_meta=True, is_seg=True)
-    semantic_seg_mask = np.zeros_like(instance_seg_mask, dtype=int)
-    for entry in meta_data[name]:
-        class_label = entry["class_label"]
-        if class_label > 0:
-            class_label = 1
-        semantic_seg_mask[instance_seg_mask == entry["instance"]] = class_label
-    save_image(join(save_path, "imagesTr/RibFrac_" + str(id).zfill(4) + "_0000.nii.gz"), image, spacing=spacing, is_seg=False)
-    save_image(join(save_path, "labelsTr/RibFrac_" + str(id).zfill(4) + ".nii.gz"), semantic_seg_mask, spacing=spacing, is_seg=True)
-
-
-def preprocess_test(load_test_image_dir, save_path):
-    print("Processing test data...")
-    filenames = load_filenames(load_test_image_dir)
-    for filename in tqdm(filenames):
-        id = int(os.path.basename(filename)[8:-13])
-        copyfile(filename, join(save_path, "imagesTs/RibFrac_" + str(id).zfill(4) + "_0000.nii.gz"))
-    print("Finished processing test data.")
-
-
-def load_filenames(img_dir, extensions=None):
-    _img_dir = fix_path(img_dir)
-    img_filenames = []
-
-    for file in os.listdir(_img_dir):
-        if extensions is None or file.endswith(extensions):
-            img_filenames.append(_img_dir + file)
-    img_filenames = np.asarray(img_filenames)
-    img_filenames = natsorted(img_filenames)
-
-    return img_filenames
-
-
-def fix_path(path):
-    if path[-1] != "/":
-        path += "/"
-    return path
-
-
-def load_image(filepath, return_meta=False, is_seg=False):
-    image = sitk.ReadImage(filepath)
-    image_np = sitk.GetArrayFromImage(image)
-
-    if is_seg:
-        image_np = np.rint(image_np)
-        image_np = image_np.astype(np.int8)  # In special cases segmentations can contain negative labels, so no np.uint8
+import SimpleITK as sitk
+from nnunet.utilities.task_name_id_conversion import convert_task_name_to_id, convert_id_to_task_name
+from batchgenerators.utilities.file_and_folder_operations import *
+from nnunet.paths import *
+
+color_cycle = (
+    "000000",
+    "4363d8",
+    "f58231",
+    "3cb44b",
+    "e6194B",
+    "911eb4",
+    "ffe119",
+    "bfef45",
+    "42d4f4",
+    "f032e6",
+    "000075",
+    "9A6324",
+    "808000",
+    "800000",
+    "469990",
+)
+
+
+def hex_to_rgb(hex: str):
+    assert len(hex) == 6
+    return tuple(int(hex[i:i + 2], 16) for i in (0, 2, 4))
+
+
+def generate_overlay(input_image: np.ndarray, segmentation: np.ndarray, mapping: dict = None, color_cycle=color_cycle,
+                     overlay_intensity=0.6):
+    """
+    image must be a color image, so last dimension must be 3. if image is grayscale, tile it first!
+    Segmentation must be label map of same shape as image (w/o color channels)
+    mapping can be label_id -> idx_in_cycle or None
+
+    returned image is scaled to [0, 255]!!!
+    """
+    # assert len(image.shape) == len(segmentation.shape)
+    # assert all([i == j for i, j in zip(image.shape, segmentation.shape)])
+
+    # create a copy of image
+    image = np.copy(input_image)
+
+    if len(image.shape) == 2:
+        image = np.tile(image[:, :, None], (1, 1, 3))
+    elif len(image.shape) == 3:
+        assert image.shape[2] == 3, 'if 3d image is given the last dimension must be the color channels ' \
+                                    '(3 channels). Only 2D images are supported'
+
+    else:
+        raise RuntimeError("unexpected image shape. only 2D images and 2D images with color channels (color in "
+                           "last dimension) are supported")
+
+    # rescale image to [0, 255]
+    image = image - image.min()
+    image = image / image.max() * 255
+
+    # create output
+
+    if mapping is None:
+        uniques = np.unique(segmentation)
+        mapping = {i: c for c, i in enumerate(uniques)}
+
+    for l in mapping.keys():
+        image[segmentation == l] += overlay_intensity * np.array(hex_to_rgb(color_cycle[mapping[l]]))
+
+    # rescale result to [0, 255]
+    image = image / image.max() * 255
+    return image.astype(np.uint8)
+
+
+def plot_overlay(image_file: str, segmentation_file: str, output_file: str, overlay_intensity: float = 0.6):
+    import matplotlib.pyplot as plt
+
+    image = sitk.GetArrayFromImage(sitk.ReadImage(image_file))
+    seg = sitk.GetArrayFromImage(sitk.ReadImage(segmentation_file))
+    assert all([i == j for i, j in zip(image.shape, seg.shape)]), "image and seg do not have the same shape: %s, %s" % (
+        image_file, segmentation_file)
+
+    assert len(image.shape) == 3, 'only 3D images/segs are supported'
+
+    fg_mask = seg != 0
+    fg_per_slice = fg_mask.sum((1, 2))
+    selected_slice = np.argmax(fg_per_slice)
+
+    overlay = generate_overlay(image[selected_slice], seg[selected_slice], overlay_intensity=overlay_intensity)
+
+    plt.imsave(output_file, overlay)
 
-    if not return_meta:
-        return image_np
+
+def plot_overlay_preprocessed(case_file: str, output_file: str, overlay_intensity: float = 0.6, modality_index=0):
+    import matplotlib.pyplot as plt
+    data = np.load(case_file)['data']
+
+    assert modality_index < (data.shape[0] - 1), 'This dataset only supports modality index up to %d' % (data.shape[0] - 2)
+
+    image = data[modality_index]
+    seg = data[-1]
+    seg[seg < 0] = 0
+
+    fg_mask = seg > 0
+    fg_per_slice = fg_mask.sum((1, 2))
+    selected_slice = np.argmax(fg_per_slice)
+
+    overlay = generate_overlay(image[selected_slice], seg[selected_slice], overlay_intensity=overlay_intensity)
+
+    plt.imsave(output_file, overlay)
+
+
+def multiprocessing_plot_overlay(list_of_image_files, list_of_seg_files, list_of_output_files, overlay_intensity,
+                                 num_processes=8):
+    p = Pool(num_processes)
+    r = p.starmap_async(plot_overlay, zip(
+        list_of_image_files, list_of_seg_files, list_of_output_files, [overlay_intensity] * len(list_of_output_files)
+    ))
+    r.get()
+    p.close()
+    p.join()
+
+
+def multiprocessing_plot_overlay_preprocessed(list_of_case_files, list_of_output_files, overlay_intensity,
+                                 num_processes=8, modality_index=0):
+    p = Pool(num_processes)
+    r = p.starmap_async(plot_overlay_preprocessed, zip(
+        list_of_case_files, list_of_output_files, [overlay_intensity] * len(list_of_output_files),
+        [modality_index] * len(list_of_output_files)
+    ))
+    r.get()
+    p.close()
+    p.join()
+
+
+def generate_overlays_for_task(task_name_or_id, output_folder, num_processes=8, modality_idx=0, use_preprocessed=True,
+                               data_identifier=default_data_identifier):
+    if isinstance(task_name_or_id, str):
+        if not task_name_or_id.startswith("Task"):
+            task_name_or_id = int(task_name_or_id)
+            task_name = convert_id_to_task_name(task_name_or_id)
+        else:
+            task_name = task_name_or_id
     else:
-        spacing = image.GetSpacing()
-        keys = image.GetMetaDataKeys()
-        header = {key:image.GetMetaData(key) for key in keys}
-        affine = None  # How do I get the affine transform with SimpleITK? With NiBabel it is just image.affine
-        return image_np, spacing, affine, header
-
-
-def save_image(filename, image, spacing=None, affine=None, header=None, is_seg=False, mp_pool=None, free_mem=False):
-    if is_seg:
-        image = np.rint(image)
-        image = image.astype(np.int8)  # In special cases segmentations can contain negative labels, so no np.uint8
-
-    image = sitk.GetImageFromArray(image)
-
-    if header is not None:
-        [image.SetMetaData(key, header[key]) for key in header.keys()]
-
-    if spacing is not None:
-        image.SetSpacing(spacing)
-
-    if affine is not None:
-        pass  # How do I set the affine transform with SimpleITK? With NiBabel it is just nib.Nifti1Image(img, affine=affine, header=header)
-
-    if mp_pool is None:
-        sitk.WriteImage(image, filename)
-        if free_mem:
-            del image
-            gc.collect()
+        task_name = convert_id_to_task_name(int(task_name_or_id))
+
+    if not use_preprocessed:
+        folder = join(nnUNet_raw_data, task_name)
+
+        identifiers = [i[:-7] for i in subfiles(join(folder, 'labelsTr'), suffix='.nii.gz', join=False)]
+
+        image_files = [join(folder, 'imagesTr', i + "_%04.0d.nii.gz" % modality_idx) for i in identifiers]
+        seg_files = [join(folder, 'labelsTr', i + ".nii.gz") for i in identifiers]
+
+        assert all([isfile(i) for i in image_files])
+        assert all([isfile(i) for i in seg_files])
+
+        maybe_mkdir_p(output_folder)
+        output_files = [join(output_folder, i + '.png') for i in identifiers]
+        multiprocessing_plot_overlay(image_files, seg_files, output_files, 0.6, num_processes)
     else:
-        mp_pool.apply_async(_save, args=(filename, image, free_mem,))
-        if free_mem:
-            del image
-            gc.collect()
-
-
-def _save(filename, image, free_mem):
-    sitk.WriteImage(image, filename)
-    if free_mem:
-        del image
-        gc.collect()
-
-
-if __name__ == "__main__":
-    # Note: Due to a bug in SimpleITK 2.1.x a version of SimpleITK < 2.1.0 is required for loading images. Further, we can't copy the images and masks, but have to load them and resample both to the same spacing.
-    # Conversion instructions:
-    # 1. All sets, parts and CSVs need to be downloaded from https://ribfrac.grand-challenge.org/dataset/
-    # 2. Unzip ribfrac-train-images-1.zip (will be unzipped as Part1) and ribfrac-train-images-2.zip (will be unzipped as Part2), move content from Part2 to Part1 and rename the folder to imagesTr
-    # 3. Unzip ribfrac-train-labels-1.zip (will be unzipped as Part1) and ribfrac-train-labels-2.zip (will be unzipped as Part2), move content from Part2 to Part1 and rename the folder to labelsTr
-    # 4. Unzip ribfrac-val-images.zip and add content to imagesTr, repeat with ribfrac-val-labels.zip
-    # 5. Unzip ribfrac-test-images.zip and rename it to imagesTs
-
-    pool = mp.Pool(processes=20)
-
-    dataset_load_path = "/home/k539i/Documents/network_drives/E132-Projekte/Projects/2021_Gotkowski_RibFrac_RibSeg/original/RibFrac/"
-    dataset_save_path = "/home/k539i/Documents/network_drives/E132-Projekte/Projects/2021_Gotkowski_RibFrac_RibSeg/preprocessed/Task155_RibFrac_binary/"
-    preprocess_dataset(dataset_load_path, dataset_save_path, pool)
-
-    print("Still saving images in background...")
-    pool.close()
-    pool.join()
-    print("All tasks finished.")
+        folder = join(preprocessing_output_dir, task_name)
+        if not isdir(folder): raise RuntimeError("run preprocessing for that task first")
+        matching_folders = subdirs(folder, prefix=data_identifier + "_stage")
+        if len(matching_folders) == 0: "run preprocessing for that task first (use default experiment planner!)"
+        matching_folders.sort()
+        folder = matching_folders[-1]
+        identifiers = [i[:-4] for i in subfiles(folder, suffix='.npz', join=False)]
+        maybe_mkdir_p(output_folder)
+        output_files = [join(output_folder, i + '.png') for i in identifiers]
+        image_files = [join(folder, i + ".npz") for i in identifiers]
+        maybe_mkdir_p(output_folder)
+        multiprocessing_plot_overlay_preprocessed(image_files, output_files, overlay_intensity=0.6,
+                                                  num_processes=num_processes, modality_index=modality_idx)
+
+
+def entry_point_generate_overlay():
+    import argparse
+    parser = argparse.ArgumentParser("Plots png overlays of the slice with the most foreground. Note that this "
+                                     "disregards spacing information!")
+    parser.add_argument('-t', type=str, help="task name or task ID", required=True)
+    parser.add_argument('-o', type=str, help="output folder", required=True)
+    parser.add_argument('-num_processes', type=int, default=8, required=False, help="number of processes used. Default: 8")
+    parser.add_argument('-modality_idx', type=int, default=0, required=False,
+                        help="modality index used (0 = _0000.nii.gz). Default: 0")
+    parser.add_argument('--use_raw', action='store_true', required=False, help="if set then we use raw data. else "
+                                                                               "we use preprocessed")
+    args = parser.parse_args()
 
-    labels = {0: "background", 1: "fracture"}
-    generate_dataset_json(join(dataset_save_path, 'dataset.json'), join(dataset_save_path, "imagesTr"), None, ('CT',), labels, "Task155_RibFrac_binary")
+    generate_overlays_for_task(args.t, args.o, args.num_processes, args.modality_idx, use_preprocessed=not args.use_raw)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/add_mean_dice_to_json.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/tensor_utilities.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,44 +8,47 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import json
 import numpy as np
-from batchgenerators.utilities.file_and_folder_operations import subfiles
-from collections import OrderedDict
+import torch
+from torch import nn
+
+
+def sum_tensor(inp, axes, keepdim=False):
+    axes = np.unique(axes).astype(int)
+    if keepdim:
+        for ax in axes:
+            inp = inp.sum(int(ax), keepdim=True)
+    else:
+        for ax in sorted(axes, reverse=True):
+            inp = inp.sum(int(ax))
+    return inp
+
+
+def mean_tensor(inp, axes, keepdim=False):
+    axes = np.unique(axes).astype(int)
+    if keepdim:
+        for ax in axes:
+            inp = inp.mean(int(ax), keepdim=True)
+    else:
+        for ax in sorted(axes, reverse=True):
+            inp = inp.mean(int(ax))
+    return inp
+
+
+def flip(x, dim):
+    """
+    flips the tensor at dimension dim (mirroring!)
+    :param x:
+    :param dim:
+    :return:
+    """
+    indices = [slice(None)] * x.dim()
+    indices[dim] = torch.arange(x.size(dim) - 1, -1, -1,
+                                dtype=torch.long, device=x.device)
+    return x[tuple(indices)]
 
 
-def foreground_mean(filename):
-    with open(filename, 'r') as f:
-        res = json.load(f)
-    class_ids = np.array([int(i) for i in res['results']['mean'].keys() if (i != 'mean')])
-    class_ids = class_ids[class_ids != 0]
-    class_ids = class_ids[class_ids != -1]
-    class_ids = class_ids[class_ids != 99]
-
-    tmp = res['results']['mean'].get('99')
-    if tmp is not None:
-        _ = res['results']['mean'].pop('99')
-
-    metrics = res['results']['mean']['1'].keys()
-    res['results']['mean']["mean"] = OrderedDict()
-    for m in metrics:
-        foreground_values = [res['results']['mean'][str(i)][m] for i in class_ids]
-        res['results']['mean']["mean"][m] = np.nanmean(foreground_values)
-    with open(filename, 'w') as f:
-        json.dump(res, f, indent=4, sort_keys=True)
-
-
-def run_in_folder(folder):
-    json_files = subfiles(folder, True, None, ".json", True)
-    json_files = [i for i in json_files if not i.split("/")[-1].startswith(".") and not i.endswith("_globalMean.json")] # stupid mac
-    for j in json_files:
-        foreground_mean(j)
-
-
-if __name__ == "__main__":
-    folder = "/media/fabian/Results/nnUNetOutput_final/summary_jsons"
-    run_in_folder(folder)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/evaluator.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import json
 import hashlib
 from datetime import datetime
 from multiprocessing.pool import Pool
 import numpy as np
 import pandas as pd
 import SimpleITK as sitk
-from nnunet.evaluation.metrics import ConfusionMatrix, ALL_METRICS
+from CartiMorph_nnUNet.evaluation.metrics import ConfusionMatrix, ALL_METRICS
 from batchgenerators.utilities.file_and_folder_operations import save_json, subfiles, join
 from collections import OrderedDict
 
 
 class Evaluator:
     """Object that holds test and reference segmentations with label information
     and computes a number of metrics on the two. 'labels' must either be an
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/evaluation/metrics.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/DatasetAnalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from batchgenerators.utilities.file_and_folder_operations import *
 from multiprocessing import Pool
 
-from nnunet.configuration import default_num_threads
-from nnunet.paths import nnUNet_raw_data, nnUNet_cropped_data
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.paths import nnUNet_raw_data, nnUNet_cropped_data
 import numpy as np
 import pickle
-from nnunet.preprocessing.cropping import get_patient_identifiers_from_cropped_files
+from CartiMorph_nnUNet.preprocessing.cropping import get_patient_identifiers_from_cropped_files
 from skimage.morphology import label
 from collections import OrderedDict
 
 
 class DatasetAnalyzer(object):
     def __init__(self, folder_with_cropped_data, overwrite=True, num_processes=default_num_threads):
         """
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/common_utils.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/common_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import numpy as np
 from copy import deepcopy
-from nnunet.network_architecture.generic_UNet import Generic_UNet
+from CartiMorph_nnUNet.network_architecture.generic_UNet import Generic_UNet
 import SimpleITK as sitk
 import shutil
 from batchgenerators.utilities.file_and_folder_operations import join
 
 
 def split_4d_nifti(filename, output_folder, add_zeros=False):
     img_itk = sitk.ReadImage(filename)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_2DUNet.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
 import shutil
 
-import nnunet
+import CartiMorph_nnUNet
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import load_pickle, subfiles
 from multiprocessing.pool import Pool
-from nnunet.configuration import default_num_threads
-from nnunet.experiment_planning.common_utils import get_pool_and_conv_props
-from nnunet.experiment_planning.experiment_planner_baseline_3DUNet import ExperimentPlanner
-from nnunet.experiment_planning.utils import add_classes_in_slice_info
-from nnunet.network_architecture.generic_UNet import Generic_UNet
-from nnunet.paths import *
-from nnunet.preprocessing.preprocessing import PreprocessorFor2D
-from nnunet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.experiment_planning.common_utils import get_pool_and_conv_props
+from CartiMorph_nnUNet.experiment_planning.experiment_planner_baseline_3DUNet import ExperimentPlanner
+from CartiMorph_nnUNet.experiment_planning.utils import add_classes_in_slice_info
+from CartiMorph_nnUNet.network_architecture.generic_UNet import Generic_UNet
+from CartiMorph_nnUNet.paths import *
+from CartiMorph_nnUNet.preprocessing.preprocessing import PreprocessorFor2D
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
 
 
 class ExperimentPlanner2D(ExperimentPlanner):
     def __init__(self, folder_with_cropped_data, preprocessed_output_folder):
         super(ExperimentPlanner2D, self).__init__(folder_with_cropped_data,
                                                   preprocessed_output_folder)
         self.data_identifier = default_data_identifier + "_2D"
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/experiment_planner_baseline_3DUNet.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import shutil
 from collections import OrderedDict
 from copy import deepcopy
 
-import nnunet
+import CartiMorph_nnUNet
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.configuration import default_num_threads
-from nnunet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
-from nnunet.experiment_planning.common_utils import get_pool_and_conv_props_poolLateV2
-from nnunet.experiment_planning.utils import create_lists_from_splitted_dataset
-from nnunet.network_architecture.generic_UNet import Generic_UNet
-from nnunet.paths import *
-from nnunet.preprocessing.cropping import get_case_identifier_from_npz
-from nnunet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
+from CartiMorph_nnUNet.experiment_planning.common_utils import get_pool_and_conv_props_poolLateV2
+from CartiMorph_nnUNet.experiment_planning.utils import create_lists_from_splitted_dataset
+from CartiMorph_nnUNet.network_architecture.generic_UNet import Generic_UNet
+from CartiMorph_nnUNet.paths import *
+from CartiMorph_nnUNet.preprocessing.cropping import get_case_identifier_from_npz
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
 
 
 class ExperimentPlanner(object):
     def __init__(self, folder_with_cropped_data, preprocessed_output_folder):
         self.folder_with_cropped_data = folder_with_cropped_data
         self.preprocessed_output_folder = preprocessed_output_folder
         self.list_of_cropped_npz_files = subfiles(self.folder_with_cropped_data, True, None, ".npz", True)
@@ -425,16 +425,16 @@
         if os.path.isdir(join(self.preprocessed_output_folder, "gt_segmentations")):
             shutil.rmtree(join(self.preprocessed_output_folder, "gt_segmentations"))
         shutil.copytree(join(self.folder_with_cropped_data, "gt_segmentations"),
                         join(self.preprocessed_output_folder, "gt_segmentations"))
         normalization_schemes = self.plans['normalization_schemes']
         use_nonzero_mask_for_normalization = self.plans['use_mask_for_norm']
         intensityproperties = self.plans['dataset_properties']['intensityproperties']
-        preprocessor_class = recursive_find_python_class([join(nnunet.__path__[0], "preprocessing")],
-                                                         self.preprocessor_name, current_module="nnunet.preprocessing")
+        preprocessor_class = recursive_find_python_class([join(CartiMorph_nnUNet.__path__[0], "preprocessing")],
+                                                         self.preprocessor_name, current_module="CartiMorph_nnUNet.preprocessing")
         assert preprocessor_class is not None
         preprocessor = preprocessor_class(normalization_schemes, use_nonzero_mask_for_normalization,
                                          self.transpose_forward,
                                           intensityproperties)
         target_spacings = [i["current_spacing"] for i in self.plans_per_stage.values()]
         if self.plans['num_stages'] > 1 and not isinstance(num_threads, (list, tuple)):
             num_threads = (default_num_threads, num_threads)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/nnUNet_plan_and_preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-import nnunet
+import CartiMorph_nnunet
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
-from nnunet.experiment_planning.utils import crop
-from nnunet.paths import *
+from CartiMorph_nnUNet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
+from CartiMorph_nnUNet.experiment_planning.utils import crop
+from CartiMorph_nnUNet.paths import *
 import shutil
-from nnunet.utilities.task_name_id_conversion import convert_id_to_task_name
-from nnunet.preprocessing.sanity_checks import verify_dataset_integrity
-from nnunet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.utilities.task_name_id_conversion import convert_id_to_task_name
+from CartiMorph_nnUNet.preprocessing.sanity_checks import verify_dataset_integrity
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
 
 
 def main():
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-t", "--task_ids", nargs="+", help="List of integers belonging to the task ids you wish to run"
@@ -64,15 +64,15 @@
                              "generated with the same number of modalities as the target dataset (LiTS -> BCV or "
                              "LiTS -> Task008_HepaticVessel is OK. BraTS -> LiTS is not (BraTS has 4 input modalities, "
                              "LiTS has just one)). Also only do things that make sense. This functionality is beta with"
                              "no support given.\n"
                              "Note that this will first print the old plans (which are going to be overwritten) and "
                              "then the new ones (provided that -no_pp was NOT set).")
     parser.add_argument("--overwrite_plans_identifier", type=str, default=None, required=False,
-                        help="If you set overwrite_plans you need to provide a unique identifier so that nnUNet knows "
+                        help="If you set overwrite_plans you need to provide a unique identifier so that CartiMorph_nnUNet knows "
                              "where to look for the correct plans and data. Assume your identifier is called "
                              "IDENTIFIER, the correct training command would be:\n"
                              "'nnUNet_train CONFIG TRAINER TASKID FOLD -p nnUNetPlans_pretrained_IDENTIFIER "
                              "-pretrained_weights FILENAME'")
 
     args = parser.parse_args()
     task_ids = args.task_ids
@@ -104,29 +104,29 @@
         if args.verify_dataset_integrity:
             verify_dataset_integrity(join(nnUNet_raw_data, task_name))
 
         crop(task_name, False, tf)
 
         tasks.append(task_name)
 
-    search_in = join(nnunet.__path__[0], "experiment_planning")
+    search_in = join(CartiMorph_nnUNet.__path__[0], "experiment_planning")
 
     if planner_name3d is not None:
-        planner_3d = recursive_find_python_class([search_in], planner_name3d, current_module="nnunet.experiment_planning")
+        planner_3d = recursive_find_python_class([search_in], planner_name3d, current_module="CartiMorph_nnUNet.experiment_planning")
         if planner_3d is None:
             raise RuntimeError("Could not find the Planner class %s. Make sure it is located somewhere in "
-                               "nnunet.experiment_planning" % planner_name3d)
+                               "CartiMorph_nnUNet.experiment_planning" % planner_name3d)
     else:
         planner_3d = None
 
     if planner_name2d is not None:
-        planner_2d = recursive_find_python_class([search_in], planner_name2d, current_module="nnunet.experiment_planning")
+        planner_2d = recursive_find_python_class([search_in], planner_name2d, current_module="CartiMorph_nnUNet.experiment_planning")
         if planner_2d is None:
             raise RuntimeError("Could not find the Planner class %s. Make sure it is located somewhere in "
-                               "nnunet.experiment_planning" % planner_name2d)
+                               "CartiMorph_nnUNet.experiment_planning" % planner_name2d)
     else:
         planner_2d = None
 
     for t in tasks:
         print("\n\n\n", t)
         cropped_out_dir = os.path.join(nnUNet_cropped_data, t)
         preprocessing_output_dir_this_task = os.path.join(preprocessing_output_dir, t)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/experiment_planning/utils.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/experiment_planning/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 import pickle
 import shutil
 from collections import OrderedDict
 from multiprocessing import Pool
 
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import join, isdir, maybe_mkdir_p, subfiles, subdirs, isfile
-from nnunet.configuration import default_num_threads
-from nnunet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
-from nnunet.experiment_planning.common_utils import split_4d_nifti
-from nnunet.paths import nnUNet_raw_data, nnUNet_cropped_data, preprocessing_output_dir
-from nnunet.preprocessing.cropping import ImageCropper
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.experiment_planning.DatasetAnalyzer import DatasetAnalyzer
+from CartiMorph_nnUNet.experiment_planning.common_utils import split_4d_nifti
+from CartiMorph_nnUNet.paths import nnUNet_raw_data, nnUNet_cropped_data, preprocessing_output_dir
+from CartiMorph_nnUNet.preprocessing.cropping import ImageCropper
+from CartiMorph_nnUNet.experiment_planning.experiment_planner_baseline_2DUNet import ExperimentPlanner2D
+from CartiMorph_nnUNet.experiment_planning.experiment_planner_baseline_3DUNet import ExperimentPlanner
 
 
 def split_4d(input_folder, num_processes=default_num_threads, overwrite_task_output_id=None):
     assert isdir(join(input_folder, "imagesTr")) and isdir(join(input_folder, "labelsTr")) and \
            isfile(join(input_folder, "dataset.json")), \
         "The input folder must be a valid Task folder from the Medical Segmentation Decathlon with at least the " \
         "imagesTr and labelsTr subfolders and the dataset.json file"
@@ -138,17 +140,14 @@
 def analyze_dataset(task_string, override=False, collect_intensityproperties=True, num_processes=default_num_threads):
     cropped_out_dir = join(nnUNet_cropped_data, task_string)
     dataset_analyzer = DatasetAnalyzer(cropped_out_dir, overwrite=override, num_processes=num_processes)
     _ = dataset_analyzer.analyze_dataset(collect_intensityproperties)
 
 
 def plan_and_preprocess(task_string, processes_lowres=default_num_threads, processes_fullres=3, no_preprocessing=False):
-    from nnunet.experiment_planning.experiment_planner_baseline_2DUNet import ExperimentPlanner2D
-    from nnunet.experiment_planning.experiment_planner_baseline_3DUNet import ExperimentPlanner
-
     preprocessing_output_dir_this_task_train = join(preprocessing_output_dir, task_string)
     cropped_out_dir = join(nnUNet_cropped_data, task_string)
     maybe_mkdir_p(preprocessing_output_dir_this_task_train)
 
     shutil.copy(join(cropped_out_dir, "dataset_properties.pkl"), preprocessing_output_dir_this_task_train)
     shutil.copy(join(nnUNet_raw_data, task_string, "dataset.json"), preprocessing_output_dir_this_task_train)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/predict.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,25 +20,25 @@
 
 import argparse
 from copy import deepcopy
 from typing import Tuple, Union, List
 
 import numpy as np
 from batchgenerators.augmentations.utils import resize_segmentation
-from nnunet.inference.segmentation_export import save_segmentation_nifti_from_softmax, save_segmentation_nifti
+from CartiMorph_nnUNet.inference.segmentation_export import save_segmentation_nifti_from_softmax, save_segmentation_nifti
 from batchgenerators.utilities.file_and_folder_operations import *
 from multiprocessing import Process, Queue
 import torch
 import SimpleITK as sitk
 import shutil
 from multiprocessing import Pool
-from nnunet.postprocessing.connected_components import load_remove_save, load_postprocessing
-from nnunet.training.model_restore import load_model_and_checkpoint_files
-from nnunet.training.network_training.nnUNetTrainer import nnUNetTrainer
-from nnunet.utilities.one_hot_encoding import to_one_hot
+from CartiMorph_nnUNet.postprocessing.connected_components import load_remove_save, load_postprocessing
+from CartiMorph_nnUNet.training.model_restore import load_model_and_checkpoint_files
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.utilities.one_hot_encoding import to_one_hot
 
 
 def preprocess_save_to_queue(preprocess_fn, q, list_of_lists, output_files, segs_from_prev_stage, classes,
                              transpose_forward):
     # suppress output
     # sys.stdout = open(os.devnull, 'w')
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/predict_simple.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/predict_simple.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 # import os
 # os.environ['MKL_NUM_THREADS'] = '6'
 # ---------------------------
 
 import argparse
 import torch
 
-from nnunet.inference.predict import predict_from_folder
-from nnunet.paths import default_plans_identifier, network_training_output_dir, default_cascade_trainer, default_trainer
+from CartiMorph_nnUNet.inference.predict import predict_from_folder
+from CartiMorph_nnUNet.paths import default_plans_identifier, network_training_output_dir, default_cascade_trainer, default_trainer
 from batchgenerators.utilities.file_and_folder_operations import join, isdir, save_json
-from nnunet.utilities.task_name_id_conversion import convert_id_to_task_name
+from CartiMorph_nnUNet.utilities.task_name_id_conversion import convert_id_to_task_name
 from time import time
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("-i", '--input_folder', help="Must contain all modalities for each patient in the correct"
                                                      " order (same as training). Files must be named "
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/inference/segmentation_export.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/inference/segmentation_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import sys
 from copy import deepcopy
 from typing import Union, Tuple
 
 import numpy as np
 import SimpleITK as sitk
 from batchgenerators.augmentations.utils import resize_segmentation
-from nnunet.preprocessing.preprocessing import get_lowres_axis, get_do_separate_z, resample_data_or_seg
+from CartiMorph_nnUNet.preprocessing.preprocessing import get_lowres_axis, get_do_separate_z, resample_data_or_seg
 from batchgenerators.utilities.file_and_folder_operations import *
 
 
 def save_segmentation_nifti_from_softmax(segmentation_softmax: Union[str, np.ndarray], out_fname: str,
                                          properties_dict: dict, order: int = 1,
                                          region_class_order: Tuple[Tuple[int]] = None,
                                          seg_postprogess_fn: callable = None, seg_postprocess_args: tuple = None,
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/custom_modules/helperModules.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/one_hot_encoding.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,22 +8,17 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+import numpy as np
 
-from torch import nn
 
-
-class Identity(nn.Module):
-    def __init__(self, *args, **kwargs):
-        super().__init__()
-
-    def forward(self, input):
-        return input
-
-
-class MyGroupNorm(nn.GroupNorm):
-    def __init__(self, num_channels, eps=1e-5, affine=True, num_groups=8):
-        super(MyGroupNorm, self).__init__(num_groups, num_channels, eps, affine)
+def to_one_hot(seg, all_seg_labels=None):
+    if all_seg_labels is None:
+        all_seg_labels = np.unique(seg)
+    result = np.zeros((len(all_seg_labels), *seg.shape), dtype=seg.dtype)
+    for i, l in enumerate(all_seg_labels):
+        result[i][seg == l] = 1
+    return result
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/generic_UNet.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/generic_UNet.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
 from copy import deepcopy
-from nnunet.utilities.nd_softmax import softmax_helper
+from CartiMorph_nnUNet.utilities.nd_softmax import softmax_helper
 from torch import nn
 import torch
 import numpy as np
-from nnunet.network_architecture.initialization import InitWeights_He
-from nnunet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.network_architecture.initialization import InitWeights_He
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
 import torch.nn.functional
 
 
 class ConvDropoutNormNonlin(nn.Module):
     """
     fixes a bug in ConvDropoutNormNonlin where lrelu was used regardless of nonlin. Bad.
     """
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/initialization.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/initialization.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/network_architecture/neural_network.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/network_architecture/neural_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
 import numpy as np
 from batchgenerators.augmentations.utils import pad_nd_image
-from nnunet.utilities.random_stuff import no_op
-from nnunet.utilities.to_torch import to_cuda, maybe_to_torch
+from CartiMorph_nnUNet.utilities.random_stuff import no_op
+from CartiMorph_nnUNet.utilities.to_torch import to_cuda, maybe_to_torch
 from torch import nn
 import torch
 from scipy.ndimage.filters import gaussian_filter
 from typing import Union, Tuple, List
 
 from torch.cuda.amp import autocast
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/paths.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/paths.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/postprocessing/connected_components.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/postprocessing/connected_components.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 import ast
 from copy import deepcopy
 from multiprocessing.pool import Pool
 
 import numpy as np
-from nnunet.configuration import default_num_threads
-from nnunet.evaluation.evaluator import aggregate_scores
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.evaluation.evaluator import aggregate_scores
 from scipy.ndimage import label
 import SimpleITK as sitk
-from nnunet.utilities.sitk_stuff import copy_geometry
+from CartiMorph_nnUNet.utilities.sitk_stuff import copy_geometry
 from batchgenerators.utilities.file_and_folder_operations import *
 import shutil
 
 
 def load_remove_save(input_file: str, output_file: str, for_which_classes: list,
                      minimum_valid_object_size: dict = None):
     # Only objects larger than minimum_valid_object_size will be removed. Keys in minimum_valid_object_size must
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/cropping.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/cropping.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/preprocessing/preprocessing.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/preprocessing/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from collections import OrderedDict
 from copy import deepcopy
 
 from batchgenerators.augmentations.utils import resize_segmentation
-from nnunet.configuration import default_num_threads, RESAMPLING_SEPARATE_Z_ANISO_THRESHOLD
-from nnunet.preprocessing.cropping import get_case_identifier_from_npz, ImageCropper
+from CartiMorph_nnUNet.configuration import default_num_threads, RESAMPLING_SEPARATE_Z_ANISO_THRESHOLD
+from CartiMorph_nnUNet.preprocessing.cropping import get_case_identifier_from_npz, ImageCropper
 from skimage.transform import resize
 from scipy.ndimage.interpolation import map_coordinates
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import *
 from multiprocessing.pool import Pool
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/default_configuration.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/default_configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,35 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-import nnunet
-from nnunet.paths import network_training_output_dir, preprocessing_output_dir, default_plans_identifier
+import CartiMorph_nnUNet
+from CartiMorph_nnUNet.paths import network_training_output_dir, preprocessing_output_dir, default_plans_identifier
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.experiment_planning.summarize_plans import summarize_plans
-from nnunet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.experiment_planning.summarize_plans import summarize_plans
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
 
 
 def get_configuration_from_output_folder(folder):
     # split off network_training_output_dir
     folder = folder[len(network_training_output_dir):]
     if folder.startswith("/"):
         folder = folder[1:]
 
     configuration, task, trainer_and_plans_identifier = folder.split("/")
     trainer, plans_identifier = trainer_and_plans_identifier.split("__")
     return configuration, task, trainer, plans_identifier
 
 
 def get_default_configuration(network, task, network_trainer, plans_identifier=default_plans_identifier,
-                              search_in=(nnunet.__path__[0], "training", "network_training"),
-                              base_module='nnunet.training.network_training'):
+                              search_in=(CartiMorph_nnUNet.__path__[0], "training", "network_training"),
+                              base_module='CartiMorph_nnUNet.training.network_training'):
     assert network in ['2d', '3d_lowres', '3d_fullres', '3d_cascade_fullres'], \
         "network can only be one of the following: \'2d\', \'3d_lowres\', \'3d_fullres\', \'3d_cascade_fullres\'"
 
     dataset_directory = join(preprocessing_output_dir, task)
 
     if network == '2d':
         plans_file = join(preprocessing_output_dir, task, plans_identifier + "_plans_2D.pkl")
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/load_pretrained_weights.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/load_pretrained_weights.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/run/run_training.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/run/run_training.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
 import argparse
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.run.default_configuration import get_default_configuration
-from nnunet.paths import default_plans_identifier
-from nnunet.run.load_pretrained_weights import load_pretrained_weights
-from nnunet.training.cascade_stuff.predict_next_stage import predict_next_stage
-from nnunet.training.network_training.nnUNetTrainer import nnUNetTrainer
-from nnunet.training.network_training.nnUNetTrainerCascadeFullRes import nnUNetTrainerCascadeFullRes
-from nnunet.training.network_training.nnUNetTrainerV2_CascadeFullRes import nnUNetTrainerV2CascadeFullRes
-from nnunet.utilities.task_name_id_conversion import convert_id_to_task_name
+from CartiMorph_nnUNet.run.default_configuration import get_default_configuration
+from CartiMorph_nnUNet.paths import default_plans_identifier
+from CartiMorph_nnUNet.run.load_pretrained_weights import load_pretrained_weights
+from CartiMorph_nnUNet.training.cascade_stuff.predict_next_stage import predict_next_stage
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainerCascadeFullRes import nnUNetTrainerCascadeFullRes
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainerV2_CascadeFullRes import nnUNetTrainerV2CascadeFullRes
+from CartiMorph_nnUNet.utilities.task_name_id_conversion import convert_id_to_task_name
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("network")
     parser.add_argument("network_trainer")
     parser.add_argument("task", help="can be task name or task id")
@@ -42,21 +42,21 @@
                              "is much more CPU and RAM intensive and should only be used if you know what you are "
                              "doing", required=False)
     parser.add_argument("--deterministic",
                         help="Makes training deterministic, but reduces training speed substantially. I (Fabian) think "
                              "this is not necessary. Deterministic training will make you overfit to some random seed. "
                              "Don't use that.",
                         required=False, default=False, action="store_true")
-    parser.add_argument("--npz", required=False, default=False, action="store_true", help="if set then nnUNet will "
+    parser.add_argument("--npz", required=False, default=False, action="store_true", help="if set then CartiMorph_nnUNet will "
                                                                                           "export npz files of "
                                                                                           "predicted segmentations "
                                                                                           "in the validation as well. "
                                                                                           "This is needed to run the "
                                                                                           "ensembling step so unless "
-                                                                                          "you are developing nnUNet "
+                                                                                          "you are developing CartiMorph_nnUNet "
                                                                                           "you should enable this")
     parser.add_argument("--find_lr", required=False, default=False, action="store_true",
                         help="not used here, just for fun")
     parser.add_argument("--valbest", required=False, default=False, action="store_true",
                         help="hands off. This is not intended to be used")
     parser.add_argument("--fp32", required=False, default=False, action="store_true",
                         help="disable mixed precision training and run old school fp32")
@@ -136,15 +136,15 @@
     # else:
     #     raise ValueError("force_separate_z must be None, True or False. Given: %s" % force_separate_z)
 
     plans_file, output_folder_name, dataset_directory, batch_dice, stage, \
     trainer_class = get_default_configuration(network, task, network_trainer, plans_identifier)
 
     if trainer_class is None:
-        raise RuntimeError("Could not find trainer class in nnunet.training.network_training")
+        raise RuntimeError("Could not find trainer class in CartiMorph_nnUNet.training.network_training")
 
     if network == "3d_cascade_fullres":
         assert issubclass(trainer_class, (nnUNetTrainerCascadeFullRes, nnUNetTrainerV2CascadeFullRes)), \
             "If running 3d_cascade_fullres then your " \
             "trainer class must be derived from " \
             "nnUNetTrainerCascadeFullRes"
     else:
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/cascade_stuff/predict_next_stage.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 
 from copy import deepcopy
 
 import numpy as np
 from batchgenerators.utilities.file_and_folder_operations import *
 import argparse
-from nnunet.preprocessing.preprocessing import resample_data_or_seg
+from CartiMorph_nnUNet.preprocessing.preprocessing import resample_data_or_seg
 from batchgenerators.utilities.file_and_folder_operations import maybe_mkdir_p
-import nnunet
-from nnunet.run.default_configuration import get_default_configuration
+import CartiMorph_nnUNet
+from CartiMorph_nnUNet.run.default_configuration import get_default_configuration
 from multiprocessing import Pool
 
-from nnunet.training.model_restore import recursive_find_python_class
-from nnunet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
 
 
 def resample_and_save(predicted, target_shape, output_file, force_separate_z=False,
                       interpolation_order=1, interpolation_order_z=0):
     if isinstance(predicted, str):
         assert isfile(predicted), "If isinstance(segmentation_softmax, str) then " \
                                   "isfile(segmentation_softmax) must be True"
@@ -106,20 +106,20 @@
     trainerclass = args.network_trainer
     task = args.task
     fold = args.fold
 
     plans_file, folder_with_preprocessed_data, output_folder_name, dataset_directory, batch_dice, stage = \
         get_default_configuration("3d_lowres", task)
 
-    trainer_class = recursive_find_python_class([join(nnunet.__path__[0], "training", "network_training")],
+    trainer_class = recursive_find_python_class([join(CartiMorph_nnUNet.__path__[0], "training", "network_training")],
                                                 trainerclass,
-                                                "nnunet.training.network_training")
+                                                "CartiMorph_nnUNet.training.network_training")
 
     if trainer_class is None:
-        raise RuntimeError("Could not find trainer class in nnunet.training.network_training")
+        raise RuntimeError("Could not find trainer class in CartiMorph_nnUNet.training.network_training")
     else:
         assert issubclass(trainer_class,
                           nnUNetTrainer), "network_trainer was found but is not derived from nnUNetTrainer"
 
     trainer = trainer_class(plans_file, fold, folder_with_preprocessed_data, output_folder=output_folder_name,
                             dataset_directory=dataset_directory, batch_dice=batch_dice, stage=stage)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/custom_transforms.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_moreDA.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,38 +13,41 @@
 #    limitations under the License.
 
 from batchgenerators.dataloading.multi_threaded_augmenter import MultiThreadedAugmenter
 from batchgenerators.transforms.abstract_transforms import Compose
 from batchgenerators.transforms.channel_selection_transforms import DataChannelSelectionTransform, \
     SegChannelSelectionTransform
 from batchgenerators.transforms.color_transforms import BrightnessMultiplicativeTransform, \
-    ContrastAugmentationTransform, BrightnessTransform, GammaTransform
+    ContrastAugmentationTransform, BrightnessTransform
+from batchgenerators.transforms.color_transforms import GammaTransform
 from batchgenerators.transforms.noise_transforms import GaussianNoiseTransform, GaussianBlurTransform
 from batchgenerators.transforms.resample_transforms import SimulateLowResolutionTransform
 from batchgenerators.transforms.spatial_transforms import SpatialTransform, MirrorTransform
 from batchgenerators.transforms.utility_transforms import RemoveLabelTransform, RenameTransform, NumpyToTensor
-from nnunet.training.data_augmentation.custom_transforms import Convert3DTo2DTransform, Convert2DTo3DTransform, \
+
+from CartiMorph_nnUNet.training.data_augmentation.custom_transforms import Convert3DTo2DTransform, Convert2DTo3DTransform, \
     MaskTransform, ConvertSegmentationToRegionsTransform
-from nnunet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params
-from nnunet.training.data_augmentation.downsampling import DownsampleSegForDSTransform3, DownsampleSegForDSTransform2
-from nnunet.training.data_augmentation.pyramid_augmentations import MoveSegAsOneHotToData, \
+from CartiMorph_nnUNet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params
+from CartiMorph_nnUNet.training.data_augmentation.downsampling import DownsampleSegForDSTransform3, DownsampleSegForDSTransform2
+from CartiMorph_nnUNet.training.data_augmentation.pyramid_augmentations import MoveSegAsOneHotToData, \
     ApplyRandomBinaryOperatorTransform, \
     RemoveRandomConnectedComponentFromOneHotEncodingTransform
 
 try:
     from batchgenerators.dataloading.nondet_multi_threaded_augmenter import NonDetMultiThreadedAugmenter
 except ImportError as ie:
     NonDetMultiThreadedAugmenter = None
 
 
-def get_insaneDA_augmentation(dataloader_train, dataloader_val, patch_size, params=default_3D_augmentation_params,
-                              border_val_seg=-1,
-                              seeds_train=None, seeds_val=None, order_seg=1, order_data=3, deep_supervision_scales=None,
-                              soft_ds=False,
-                              classes=None, pin_memory=True, regions=None):
+def get_moreDA_augmentation(dataloader_train, dataloader_val, patch_size, params=default_3D_augmentation_params,
+                            border_val_seg=-1,
+                            seeds_train=None, seeds_val=None, order_seg=1, order_data=3, deep_supervision_scales=None,
+                            soft_ds=False,
+                            classes=None, pin_memory=True, regions=None,
+                            use_nondetMultiThreadedAugmenter: bool = False):
     assert params.get('mirror') is None, "old version of params, use new keyword do_mirror"
 
     tr_transforms = []
 
     if params.get("selected_data_channels") is not None:
         tr_transforms.append(DataChannelSelectionTransform(params.get("selected_data_channels")))
 
@@ -57,50 +60,52 @@
         tr_transforms.append(Convert3DTo2DTransform())
         patch_size_spatial = patch_size[1:]
     else:
         patch_size_spatial = patch_size
         ignore_axes = None
 
     tr_transforms.append(SpatialTransform(
-        patch_size_spatial, patch_center_dist_from_border=None, do_elastic_deform=params.get("do_elastic"),
-        alpha=params.get("elastic_deform_alpha"), sigma=params.get("elastic_deform_sigma"),
+        patch_size_spatial, patch_center_dist_from_border=None,
+        do_elastic_deform=params.get("do_elastic"), alpha=params.get("elastic_deform_alpha"),
+        sigma=params.get("elastic_deform_sigma"),
         do_rotation=params.get("do_rotation"), angle_x=params.get("rotation_x"), angle_y=params.get("rotation_y"),
-        angle_z=params.get("rotation_z"), do_scale=params.get("do_scaling"), scale=params.get("scale_range"),
+        angle_z=params.get("rotation_z"), p_rot_per_axis=params.get("rotation_p_per_axis"),
+        do_scale=params.get("do_scaling"), scale=params.get("scale_range"),
         border_mode_data=params.get("border_mode_data"), border_cval_data=0, order_data=order_data,
         border_mode_seg="constant", border_cval_seg=border_val_seg,
         order_seg=order_seg, random_crop=params.get("random_crop"), p_el_per_sample=params.get("p_eldef"),
         p_scale_per_sample=params.get("p_scale"), p_rot_per_sample=params.get("p_rot"),
-        independent_scale_for_each_axis=params.get("independent_scale_factor_for_each_axis"),
-        p_independent_scale_per_axis=params.get("p_independent_scale_per_axis")
+        independent_scale_for_each_axis=params.get("independent_scale_factor_for_each_axis")
     ))
 
     if params.get("dummy_2D"):
         tr_transforms.append(Convert2DTo3DTransform())
 
     # we need to put the color augmentations after the dummy 2d part (if applicable). Otherwise the overloaded color
     # channel gets in the way
-    tr_transforms.append(GaussianNoiseTransform(p_per_sample=0.15))
-    tr_transforms.append(GaussianBlurTransform((0.5, 1.5), different_sigma_per_channel=True, p_per_sample=0.2,
+    tr_transforms.append(GaussianNoiseTransform(p_per_sample=0.1))
+    tr_transforms.append(GaussianBlurTransform((0.5, 1.), different_sigma_per_channel=True, p_per_sample=0.2,
                                                p_per_channel=0.5))
-    tr_transforms.append(BrightnessMultiplicativeTransform(multiplier_range=(0.70, 1.3), p_per_sample=0.15))
-    tr_transforms.append(ContrastAugmentationTransform(contrast_range=(0.65, 1.5), p_per_sample=0.15))
-    tr_transforms.append(SimulateLowResolutionTransform(zoom_range=(0.5, 1), per_channel=True,
-                                                        p_per_channel=0.5,
-                                                        order_downsample=0, order_upsample=3, p_per_sample=0.25,
-                                                        ignore_axes=ignore_axes))
-    tr_transforms.append(
-        GammaTransform(params.get("gamma_range"), True, True, retain_stats=params.get("gamma_retain_stats"),
-                       p_per_sample=0.15))  # inverted gamma
+    tr_transforms.append(BrightnessMultiplicativeTransform(multiplier_range=(0.75, 1.25), p_per_sample=0.15))
 
     if params.get("do_additive_brightness"):
         tr_transforms.append(BrightnessTransform(params.get("additive_brightness_mu"),
                                                  params.get("additive_brightness_sigma"),
                                                  True, p_per_sample=params.get("additive_brightness_p_per_sample"),
                                                  p_per_channel=params.get("additive_brightness_p_per_channel")))
 
+    tr_transforms.append(ContrastAugmentationTransform(p_per_sample=0.15))
+    tr_transforms.append(SimulateLowResolutionTransform(zoom_range=(0.5, 1), per_channel=True,
+                                                        p_per_channel=0.5,
+                                                        order_downsample=0, order_upsample=3, p_per_sample=0.25,
+                                                        ignore_axes=ignore_axes))
+    tr_transforms.append(
+        GammaTransform(params.get("gamma_range"), True, True, retain_stats=params.get("gamma_retain_stats"),
+                       p_per_sample=0.1))  # inverted gamma
+
     if params.get("do_gamma"):
         tr_transforms.append(
             GammaTransform(params.get("gamma_range"), False, True, retain_stats=params.get("gamma_retain_stats"),
                            p_per_sample=params["p_gamma"]))
 
     if params.get("do_mirror") or params.get("mirror"):
         tr_transforms.append(MirrorTransform(params.get("mirror_axes")))
@@ -109,22 +114,23 @@
         mask_was_used_for_normalization = params.get("mask_was_used_for_normalization")
         tr_transforms.append(MaskTransform(mask_was_used_for_normalization, mask_idx_in_seg=0, set_outside_to=0))
 
     tr_transforms.append(RemoveLabelTransform(-1, 0))
 
     if params.get("move_last_seg_chanel_to_data") is not None and params.get("move_last_seg_chanel_to_data"):
         tr_transforms.append(MoveSegAsOneHotToData(1, params.get("all_segmentation_labels"), 'seg', 'data'))
-        if params.get("cascade_do_cascade_augmentations") and not None and params.get(
+        if params.get("cascade_do_cascade_augmentations") is not None and params.get(
                 "cascade_do_cascade_augmentations"):
             if params.get("cascade_random_binary_transform_p") > 0:
                 tr_transforms.append(ApplyRandomBinaryOperatorTransform(
                     channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
                     p_per_sample=params.get("cascade_random_binary_transform_p"),
                     key="data",
-                    strel_size=params.get("cascade_random_binary_transform_size")))
+                    strel_size=params.get("cascade_random_binary_transform_size"),
+                    p_per_label=params.get("cascade_random_binary_transform_p_per_label")))
             if params.get("cascade_remove_conn_comp_p") > 0:
                 tr_transforms.append(
                     RemoveRandomConnectedComponentFromOneHotEncodingTransform(
                         channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
                         key="data",
                         p_per_sample=params.get("cascade_remove_conn_comp_p"),
                         fill_with_other_class_p=params.get("cascade_remove_conn_comp_max_size_percent_threshold"),
@@ -143,17 +149,26 @@
         else:
             tr_transforms.append(DownsampleSegForDSTransform2(deep_supervision_scales, 0, input_key='target',
                                                               output_key='target'))
 
     tr_transforms.append(NumpyToTensor(['data', 'target'], 'float'))
     tr_transforms = Compose(tr_transforms)
 
-    batchgenerator_train = MultiThreadedAugmenter(dataloader_train, tr_transforms, params.get('num_threads'),
-                                                  params.get("num_cached_per_thread"),
-                                                  seeds=seeds_train, pin_memory=pin_memory)
+    if use_nondetMultiThreadedAugmenter:
+        if NonDetMultiThreadedAugmenter is None:
+            raise RuntimeError('NonDetMultiThreadedAugmenter is not yet available')
+        batchgenerator_train = NonDetMultiThreadedAugmenter(dataloader_train, tr_transforms, params.get('num_threads'),
+                                                            params.get("num_cached_per_thread"), seeds=seeds_train,
+                                                            pin_memory=pin_memory)
+    else:
+        batchgenerator_train = MultiThreadedAugmenter(dataloader_train, tr_transforms, params.get('num_threads'),
+                                                      params.get("num_cached_per_thread"),
+                                                      seeds=seeds_train, pin_memory=pin_memory)
+    # batchgenerator_train = SingleThreadedAugmenter(dataloader_train, tr_transforms)
+    # import IPython;IPython.embed()
 
     val_transforms = []
     val_transforms.append(RemoveLabelTransform(-1, 0))
     if params.get("selected_data_channels") is not None:
         val_transforms.append(DataChannelSelectionTransform(params.get("selected_data_channels")))
     if params.get("selected_seg_channels") is not None:
         val_transforms.append(SegChannelSelectionTransform(params.get("selected_seg_channels")))
@@ -173,11 +188,23 @@
         else:
             val_transforms.append(DownsampleSegForDSTransform2(deep_supervision_scales, 0, input_key='target',
                                                                output_key='target'))
 
     val_transforms.append(NumpyToTensor(['data', 'target'], 'float'))
     val_transforms = Compose(val_transforms)
 
-    batchgenerator_val = MultiThreadedAugmenter(dataloader_val, val_transforms, max(params.get('num_threads') // 2, 1),
-                                                params.get("num_cached_per_thread"),
-                                                seeds=seeds_val, pin_memory=pin_memory)
-    return batchgenerator_train, batchgenerator_val
+    if use_nondetMultiThreadedAugmenter:
+        if NonDetMultiThreadedAugmenter is None:
+            raise RuntimeError('NonDetMultiThreadedAugmenter is not yet available')
+        batchgenerator_val = NonDetMultiThreadedAugmenter(dataloader_val, val_transforms,
+                                                          max(params.get('num_threads') // 2, 1),
+                                                          params.get("num_cached_per_thread"),
+                                                          seeds=seeds_val, pin_memory=pin_memory)
+    else:
+        batchgenerator_val = MultiThreadedAugmenter(dataloader_val, val_transforms,
+                                                    max(params.get('num_threads') // 2, 1),
+                                                    params.get("num_cached_per_thread"),
+                                                    seeds=seeds_val, pin_memory=pin_memory)
+    # batchgenerator_val = SingleThreadedAugmenter(dataloader_val, val_transforms)
+
+    return batchgenerator_train, batchgenerator_val
+
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/data_augmentation_insaneDA2.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/default_data_augmentation.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,156 +8,212 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+import os
+from copy import deepcopy
+
+import numpy as np
 from batchgenerators.dataloading.multi_threaded_augmenter import MultiThreadedAugmenter
 from batchgenerators.transforms.abstract_transforms import Compose
 from batchgenerators.transforms.channel_selection_transforms import DataChannelSelectionTransform, \
     SegChannelSelectionTransform
-from batchgenerators.transforms.color_transforms import BrightnessMultiplicativeTransform, \
-    ContrastAugmentationTransform, BrightnessTransform
 from batchgenerators.transforms.color_transforms import GammaTransform
-from batchgenerators.transforms.noise_transforms import GaussianNoiseTransform, GaussianBlurTransform
-from batchgenerators.transforms.resample_transforms import SimulateLowResolutionTransform
-from batchgenerators.transforms.spatial_transforms import MirrorTransform
-from batchgenerators.transforms.spatial_transforms import SpatialTransform_2
+from batchgenerators.transforms.spatial_transforms import SpatialTransform, MirrorTransform
 from batchgenerators.transforms.utility_transforms import RemoveLabelTransform, RenameTransform, NumpyToTensor
 
-from nnunet.training.data_augmentation.custom_transforms import Convert3DTo2DTransform, Convert2DTo3DTransform, \
+from CartiMorph_nnUNet.training.data_augmentation.custom_transforms import Convert3DTo2DTransform, Convert2DTo3DTransform, \
     MaskTransform, ConvertSegmentationToRegionsTransform
-from nnunet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params
-from nnunet.training.data_augmentation.downsampling import DownsampleSegForDSTransform3, DownsampleSegForDSTransform2
-from nnunet.training.data_augmentation.pyramid_augmentations import MoveSegAsOneHotToData, \
+from CartiMorph_nnUNet.training.data_augmentation.pyramid_augmentations import MoveSegAsOneHotToData, \
     ApplyRandomBinaryOperatorTransform, \
     RemoveRandomConnectedComponentFromOneHotEncodingTransform
+from CartiMorph_nnUNet.utilities.set_n_proc_DA import get_allowed_n_proc_DA
 
 try:
     from batchgenerators.dataloading.nondet_multi_threaded_augmenter import NonDetMultiThreadedAugmenter
 except ImportError as ie:
     NonDetMultiThreadedAugmenter = None
 
 
-def get_insaneDA_augmentation2(dataloader_train, dataloader_val, patch_size, params=default_3D_augmentation_params,
-                              border_val_seg=-1,
-                              seeds_train=None, seeds_val=None, order_seg=1, order_data=3, deep_supervision_scales=None,
-                              soft_ds=False,
-                              classes=None, pin_memory=True, regions=None):
+default_3D_augmentation_params = {
+    "selected_data_channels": None,
+    "selected_seg_channels": None,
+
+    "do_elastic": True,
+    "elastic_deform_alpha": (0., 900.),
+    "elastic_deform_sigma": (9., 13.),
+    "p_eldef": 0.2,
+
+    "do_scaling": True,
+    "scale_range": (0.85, 1.25),
+    "independent_scale_factor_for_each_axis": False,
+    "p_independent_scale_per_axis": 1,
+    "p_scale": 0.2,
+
+    "do_rotation": True,
+    "rotation_x": (-15. / 360 * 2. * np.pi, 15. / 360 * 2. * np.pi),
+    "rotation_y": (-15. / 360 * 2. * np.pi, 15. / 360 * 2. * np.pi),
+    "rotation_z": (-15. / 360 * 2. * np.pi, 15. / 360 * 2. * np.pi),
+    "rotation_p_per_axis": 1,
+    "p_rot": 0.2,
+
+    "random_crop": False,
+    "random_crop_dist_to_border": None,
+
+    "do_gamma": True,
+    "gamma_retain_stats": True,
+    "gamma_range": (0.7, 1.5),
+    "p_gamma": 0.3,
+
+    "do_mirror": True,
+    "mirror_axes": (0, 1, 2),
+
+    "dummy_2D": False,
+    "mask_was_used_for_normalization": None,
+    "border_mode_data": "constant",
+
+    "all_segmentation_labels": None,  # used for cascade
+    "move_last_seg_chanel_to_data": False,  # used for cascade
+    "cascade_do_cascade_augmentations": False,  # used for cascade
+    "cascade_random_binary_transform_p": 0.4,
+    "cascade_random_binary_transform_p_per_label": 1,
+    "cascade_random_binary_transform_size": (1, 8),
+    "cascade_remove_conn_comp_p": 0.2,
+    "cascade_remove_conn_comp_max_size_percent_threshold": 0.15,
+    "cascade_remove_conn_comp_fill_with_other_class_p": 0.0,
+
+    "do_additive_brightness": False,
+    "additive_brightness_p_per_sample": 0.15,
+    "additive_brightness_p_per_channel": 0.5,
+    "additive_brightness_mu": 0.0,
+    "additive_brightness_sigma": 0.1,
+
+    "num_threads": get_allowed_n_proc_DA() if get_allowed_n_proc_DA() is not None else 12,
+    "num_cached_per_thread": 1,
+}
+
+default_2D_augmentation_params = deepcopy(default_3D_augmentation_params)
+
+default_2D_augmentation_params["elastic_deform_alpha"] = (0., 200.)
+default_2D_augmentation_params["elastic_deform_sigma"] = (9., 13.)
+default_2D_augmentation_params["rotation_x"] = (-180. / 360 * 2. * np.pi, 180. / 360 * 2. * np.pi)
+default_2D_augmentation_params["rotation_y"] = (-0. / 360 * 2. * np.pi, 0. / 360 * 2. * np.pi)
+default_2D_augmentation_params["rotation_z"] = (-0. / 360 * 2. * np.pi, 0. / 360 * 2. * np.pi)
+
+# sometimes you have 3d data and a 3d net but cannot augment them properly in 3d due to anisotropy (which is currently
+# not supported in batchgenerators). In that case you can 'cheat' and transfer your 3d data into 2d data and
+# transform them back after augmentation
+default_2D_augmentation_params["dummy_2D"] = False
+default_2D_augmentation_params["mirror_axes"] = (0, 1)  # this can be (0, 1, 2) if dummy_2D=True
+
+
+def get_patch_size(final_patch_size, rot_x, rot_y, rot_z, scale_range):
+    if isinstance(rot_x, (tuple, list)):
+        rot_x = max(np.abs(rot_x))
+    if isinstance(rot_y, (tuple, list)):
+        rot_y = max(np.abs(rot_y))
+    if isinstance(rot_z, (tuple, list)):
+        rot_z = max(np.abs(rot_z))
+    rot_x = min(90 / 360 * 2. * np.pi, rot_x)
+    rot_y = min(90 / 360 * 2. * np.pi, rot_y)
+    rot_z = min(90 / 360 * 2. * np.pi, rot_z)
+    from batchgenerators.augmentations.utils import rotate_coords_3d, rotate_coords_2d
+    coords = np.array(final_patch_size)
+    final_shape = np.copy(coords)
+    if len(coords) == 3:
+        final_shape = np.max(np.vstack((np.abs(rotate_coords_3d(coords, rot_x, 0, 0)), final_shape)), 0)
+        final_shape = np.max(np.vstack((np.abs(rotate_coords_3d(coords, 0, rot_y, 0)), final_shape)), 0)
+        final_shape = np.max(np.vstack((np.abs(rotate_coords_3d(coords, 0, 0, rot_z)), final_shape)), 0)
+    elif len(coords) == 2:
+        final_shape = np.max(np.vstack((np.abs(rotate_coords_2d(coords, rot_x)), final_shape)), 0)
+    final_shape /= min(scale_range)
+    return final_shape.astype(int)
+
+
+def get_default_augmentation(dataloader_train, dataloader_val, patch_size, params=default_3D_augmentation_params,
+                             border_val_seg=-1, pin_memory=True,
+                             seeds_train=None, seeds_val=None, regions=None):
     assert params.get('mirror') is None, "old version of params, use new keyword do_mirror"
-
     tr_transforms = []
 
     if params.get("selected_data_channels") is not None:
         tr_transforms.append(DataChannelSelectionTransform(params.get("selected_data_channels")))
 
     if params.get("selected_seg_channels") is not None:
         tr_transforms.append(SegChannelSelectionTransform(params.get("selected_seg_channels")))
 
     # don't do color augmentations while in 2d mode with 3d data because the color channel is overloaded!!
     if params.get("dummy_2D") is not None and params.get("dummy_2D"):
-        ignore_axes = (0,)
         tr_transforms.append(Convert3DTo2DTransform())
         patch_size_spatial = patch_size[1:]
     else:
         patch_size_spatial = patch_size
-        ignore_axes = None
 
-    tr_transforms.append(SpatialTransform_2(
+    tr_transforms.append(SpatialTransform(
         patch_size_spatial, patch_center_dist_from_border=None, do_elastic_deform=params.get("do_elastic"),
-        deformation_scale=params.get("eldef_deformation_scale"),
+        alpha=params.get("elastic_deform_alpha"), sigma=params.get("elastic_deform_sigma"),
         do_rotation=params.get("do_rotation"), angle_x=params.get("rotation_x"), angle_y=params.get("rotation_y"),
         angle_z=params.get("rotation_z"), do_scale=params.get("do_scaling"), scale=params.get("scale_range"),
-        border_mode_data=params.get("border_mode_data"), border_cval_data=0, order_data=order_data,
-        border_mode_seg="constant", border_cval_seg=border_val_seg,
-        order_seg=order_seg, random_crop=params.get("random_crop"), p_el_per_sample=params.get("p_eldef"),
+        border_mode_data=params.get("border_mode_data"), border_cval_data=0, order_data=3, border_mode_seg="constant",
+        border_cval_seg=border_val_seg,
+        order_seg=1, random_crop=params.get("random_crop"), p_el_per_sample=params.get("p_eldef"),
         p_scale_per_sample=params.get("p_scale"), p_rot_per_sample=params.get("p_rot"),
-        independent_scale_for_each_axis=params.get("independent_scale_factor_for_each_axis"),
-        p_independent_scale_per_axis=params.get("p_independent_scale_per_axis")
+        independent_scale_for_each_axis=params.get("independent_scale_factor_for_each_axis")
     ))
-
-    if params.get("dummy_2D"):
+    if params.get("dummy_2D") is not None and params.get("dummy_2D"):
         tr_transforms.append(Convert2DTo3DTransform())
 
-    # we need to put the color augmentations after the dummy 2d part (if applicable). Otherwise the overloaded color
-    # channel gets in the way
-    tr_transforms.append(GaussianNoiseTransform(p_per_sample=0.15))
-    tr_transforms.append(GaussianBlurTransform((0.5, 1.5), different_sigma_per_channel=True, p_per_sample=0.2,
-                                               p_per_channel=0.5))
-    tr_transforms.append(BrightnessMultiplicativeTransform(multiplier_range=(0.70, 1.3), p_per_sample=0.15))
-    tr_transforms.append(ContrastAugmentationTransform(contrast_range=(0.65, 1.5), p_per_sample=0.15))
-    tr_transforms.append(SimulateLowResolutionTransform(zoom_range=(0.5, 1), per_channel=True,
-                                                        p_per_channel=0.5,
-                                                        order_downsample=0, order_upsample=3, p_per_sample=0.25,
-                                                        ignore_axes=ignore_axes))
-    tr_transforms.append(
-        GammaTransform(params.get("gamma_range"), True, True, retain_stats=params.get("gamma_retain_stats"),
-                       p_per_sample=0.15))  # inverted gamma
-
-    if params.get("do_additive_brightness"):
-        tr_transforms.append(BrightnessTransform(params.get("additive_brightness_mu"),
-                                                 params.get("additive_brightness_sigma"),
-                                                 True, p_per_sample=params.get("additive_brightness_p_per_sample"),
-                                                 p_per_channel=params.get("additive_brightness_p_per_channel")))
-
     if params.get("do_gamma"):
         tr_transforms.append(
             GammaTransform(params.get("gamma_range"), False, True, retain_stats=params.get("gamma_retain_stats"),
                            p_per_sample=params["p_gamma"]))
 
-    if params.get("do_mirror") or params.get("mirror"):
+    if params.get("do_mirror"):
         tr_transforms.append(MirrorTransform(params.get("mirror_axes")))
 
     if params.get("mask_was_used_for_normalization") is not None:
         mask_was_used_for_normalization = params.get("mask_was_used_for_normalization")
         tr_transforms.append(MaskTransform(mask_was_used_for_normalization, mask_idx_in_seg=0, set_outside_to=0))
 
     tr_transforms.append(RemoveLabelTransform(-1, 0))
 
     if params.get("move_last_seg_chanel_to_data") is not None and params.get("move_last_seg_chanel_to_data"):
         tr_transforms.append(MoveSegAsOneHotToData(1, params.get("all_segmentation_labels"), 'seg', 'data'))
         if params.get("cascade_do_cascade_augmentations") and not None and params.get(
                 "cascade_do_cascade_augmentations"):
-            if params.get("cascade_random_binary_transform_p") > 0:
-                tr_transforms.append(ApplyRandomBinaryOperatorTransform(
-                    channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
-                    p_per_sample=params.get("cascade_random_binary_transform_p"),
-                    key="data",
-                    strel_size=params.get("cascade_random_binary_transform_size")))
-            if params.get("cascade_remove_conn_comp_p") > 0:
-                tr_transforms.append(
-                    RemoveRandomConnectedComponentFromOneHotEncodingTransform(
-                        channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
-                        key="data",
-                        p_per_sample=params.get("cascade_remove_conn_comp_p"),
-                        fill_with_other_class_p=params.get("cascade_remove_conn_comp_max_size_percent_threshold"),
-                        dont_do_if_covers_more_than_X_percent=params.get(
-                            "cascade_remove_conn_comp_fill_with_other_class_p")))
+            tr_transforms.append(ApplyRandomBinaryOperatorTransform(
+                channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
+                p_per_sample=params.get("cascade_random_binary_transform_p"),
+                key="data",
+                strel_size=params.get("cascade_random_binary_transform_size")))
+            tr_transforms.append(RemoveRandomConnectedComponentFromOneHotEncodingTransform(
+                channel_idx=list(range(-len(params.get("all_segmentation_labels")), 0)),
+                key="data",
+                p_per_sample=params.get("cascade_remove_conn_comp_p"),
+                fill_with_other_class_p=params.get("cascade_remove_conn_comp_max_size_percent_threshold"),
+                dont_do_if_covers_more_than_X_percent=params.get("cascade_remove_conn_comp_fill_with_other_class_p")))
 
     tr_transforms.append(RenameTransform('seg', 'target', True))
 
     if regions is not None:
         tr_transforms.append(ConvertSegmentationToRegionsTransform(regions, 'target', 'target'))
 
-    if deep_supervision_scales is not None:
-        if soft_ds:
-            assert classes is not None
-            tr_transforms.append(DownsampleSegForDSTransform3(deep_supervision_scales, 'target', 'target', classes))
-        else:
-            tr_transforms.append(DownsampleSegForDSTransform2(deep_supervision_scales, 0, input_key='target',
-                                                              output_key='target'))
-
     tr_transforms.append(NumpyToTensor(['data', 'target'], 'float'))
+
     tr_transforms = Compose(tr_transforms)
+    # from batchgenerators.dataloading import SingleThreadedAugmenter
+    # batchgenerator_train = SingleThreadedAugmenter(dataloader_train, tr_transforms)
+    # import IPython;IPython.embed()
 
     batchgenerator_train = MultiThreadedAugmenter(dataloader_train, tr_transforms, params.get('num_threads'),
-                                                   params.get("num_cached_per_thread"),
-                                                   seeds=seeds_train, pin_memory=pin_memory)
-    #batchgenerator_train = SingleThreadedAugmenter(dataloader_train, tr_transforms)
+                                                  params.get("num_cached_per_thread"), seeds=seeds_train,
+                                                  pin_memory=pin_memory)
 
     val_transforms = []
     val_transforms.append(RemoveLabelTransform(-1, 0))
     if params.get("selected_data_channels") is not None:
         val_transforms.append(DataChannelSelectionTransform(params.get("selected_data_channels")))
     if params.get("selected_seg_channels") is not None:
         val_transforms.append(SegChannelSelectionTransform(params.get("selected_seg_channels")))
@@ -166,23 +222,37 @@
         val_transforms.append(MoveSegAsOneHotToData(1, params.get("all_segmentation_labels"), 'seg', 'data'))
 
     val_transforms.append(RenameTransform('seg', 'target', True))
 
     if regions is not None:
         val_transforms.append(ConvertSegmentationToRegionsTransform(regions, 'target', 'target'))
 
-    if deep_supervision_scales is not None:
-        if soft_ds:
-            assert classes is not None
-            val_transforms.append(DownsampleSegForDSTransform3(deep_supervision_scales, 'target', 'target', classes))
-        else:
-            val_transforms.append(DownsampleSegForDSTransform2(deep_supervision_scales, 0, input_key='target',
-                                                               output_key='target'))
-
     val_transforms.append(NumpyToTensor(['data', 'target'], 'float'))
     val_transforms = Compose(val_transforms)
 
+    # batchgenerator_val = SingleThreadedAugmenter(dataloader_val, val_transforms)
     batchgenerator_val = MultiThreadedAugmenter(dataloader_val, val_transforms, max(params.get('num_threads') // 2, 1),
-                                                params.get("num_cached_per_thread"),
-                                                seeds=seeds_val, pin_memory=pin_memory)
+                                                params.get("num_cached_per_thread"), seeds=seeds_val,
+                                                pin_memory=pin_memory)
     return batchgenerator_train, batchgenerator_val
 
+
+if __name__ == "__main__":
+    from CartiMorph_nnUNet.training.dataloading.dataset_loading import DataLoader3D, load_dataset
+    from CartiMorph_nnUNet.paths import preprocessing_output_dir
+    import os
+    import pickle
+
+    t = "Task002_Heart"
+    p = os.path.join(preprocessing_output_dir, t)
+    dataset = load_dataset(p, 0)
+    with open(os.path.join(p, "plans.pkl"), 'rb') as f:
+        plans = pickle.load(f)
+
+    basic_patch_size = get_patch_size(np.array(plans['stage_properties'][0].patch_size),
+                                      default_3D_augmentation_params['rotation_x'],
+                                      default_3D_augmentation_params['rotation_y'],
+                                      default_3D_augmentation_params['rotation_z'],
+                                      default_3D_augmentation_params['scale_range'])
+
+    dl = DataLoader3D(dataset, basic_patch_size, np.array(plans['stage_properties'][0].patch_size).astype(int), 1)
+    tr, val = get_default_augmentation(dl, dl, np.array(plans['stage_properties'][0].patch_size).astype(int))
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/downsampling.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/downsampling.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/data_augmentation/pyramid_augmentations.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/dataloading/dataset_loading.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/dataloading/dataset_loading.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 from collections import OrderedDict
 import numpy as np
 from multiprocessing import Pool
 
 from batchgenerators.dataloading.data_loader import SlimDataLoaderBase
 
-from nnunet.configuration import default_num_threads
-from nnunet.paths import preprocessing_output_dir
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.paths import preprocessing_output_dir
 from batchgenerators.utilities.file_and_folder_operations import *
 
 
 def get_case_identifiers(folder):
     case_identifiers = [i[:-4] for i in os.listdir(folder) if i.endswith("npz") and (i.find("segFromPrevStage") == -1)]
     return case_identifiers
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/learning_rate/poly_lr.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/learning_rate/poly_lr.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/TopK_loss.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 import numpy as np
 import torch
-from nnunet.training.loss_functions.crossentropy import RobustCrossEntropyLoss
+from CartiMorph_nnUNet.training.loss_functions.crossentropy import RobustCrossEntropyLoss
 
 
 class TopKLoss(RobustCrossEntropyLoss):
     """
     Network has to have NO LINEARITY!
     """
     def __init__(self, weight=None, ignore_index=-100, k=10):
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/deep_supervision.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/dice_loss.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/dice_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
 import torch
-from nnunet.training.loss_functions.TopK_loss import TopKLoss
-from nnunet.training.loss_functions.crossentropy import RobustCrossEntropyLoss
-from nnunet.utilities.nd_softmax import softmax_helper
-from nnunet.utilities.tensor_utilities import sum_tensor
+from CartiMorph_nnUNet.training.loss_functions.TopK_loss import TopKLoss
+from CartiMorph_nnUNet.training.loss_functions.crossentropy import RobustCrossEntropyLoss
+from CartiMorph_nnUNet.utilities.nd_softmax import softmax_helper
+from CartiMorph_nnUNet.utilities.tensor_utilities import sum_tensor
 from torch import nn
 import numpy as np
 
 
 class GDL(nn.Module):
     def __init__(self, apply_nonlin=None, batch_dice=False, do_bg=True, smooth=1.,
                  square=False, square_volumes=False):
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/loss_functions/focal_loss.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/loss_functions/focal_loss.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/model_restore.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/model_restore.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import nnunet
+import CartiMorph_nnUNet
 import torch
 from batchgenerators.utilities.file_and_folder_operations import *
 import importlib
 import pkgutil
-from nnunet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
 
 
 def recursive_find_python_class(folder, trainer_name, current_module):
     tr = None
     for importer, modname, ispkg in pkgutil.iter_modules(folder):
         # print(modname, ispkg)
         if not ispkg:
@@ -40,44 +40,44 @@
 
     return tr
 
 
 def restore_model(pkl_file, checkpoint=None, train=False, fp16=None):
     """
     This is a utility function to load any nnUNet trainer from a pkl. It will recursively search
-    nnunet.trainig.network_training for the file that contains the trainer and instantiate it with the arguments saved in the pkl file. If checkpoint
+    CartiMorph_nnUNet.trainig.network_training for the file that contains the trainer and instantiate it with the arguments saved in the pkl file. If checkpoint
     is specified, it will furthermore load the checkpoint file in train/test mode (as specified by train).
     The pkl file required here is the one that will be saved automatically when calling nnUNetTrainer.save_checkpoint.
     :param pkl_file:
     :param checkpoint:
     :param train:
     :param fp16: if None then we take no action. If True/False we overwrite what the model has in its init
     :return:
     """
     info = load_pickle(pkl_file)
     init = info['init']
     name = info['name']
-    search_in = join(nnunet.__path__[0], "training", "network_training")
-    tr = recursive_find_python_class([search_in], name, current_module="nnunet.training.network_training")
+    search_in = join(CartiMorph_nnUNet.__path__[0], "training", "network_training")
+    tr = recursive_find_python_class([search_in], name, current_module="CartiMorph_nnUNet.training.network_training")
 
     if tr is None:
         """
         Fabian only. This will trigger searching for trainer classes in other repositories as well
         """
         try:
             import meddec
             search_in = join(meddec.__path__[0], "model_training")
             tr = recursive_find_python_class([search_in], name, current_module="meddec.model_training")
         except ImportError:
             pass
 
     if tr is None:
-        raise RuntimeError("Could not find the model trainer specified in checkpoint in nnunet.trainig.network_training. If it "
+        raise RuntimeError("Could not find the model trainer specified in checkpoint in CartiMorph_nnUNet.trainig.network_training. If it "
                            "is not located there, please move it or change the code of restore_model. Your model "
-                           "trainer can be located in any directory within nnunet.trainig.network_training (search is recursive)."
+                           "trainer can be located in any directory within CartiMorph_nnUNet.trainig.network_training (search is recursive)."
                            "\nDebug info: \ncheckpoint file: %s\nName of trainer: %s " % (checkpoint, name))
     assert issubclass(tr, nnUNetTrainer), "The network trainer was found but is not a subclass of nnUNetTrainer. " \
                                           "Please make it so!"
 
     # this is now deprecated
     """if len(init) == 7:
         print("warning: this model seems to have been saved with a previous version of nnUNet. Attempting to load it "
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2_CascadeFullRes.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,95 +9,123 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
+from multiprocessing.pool import Pool
 from time import sleep
-
-import numpy as np
-import torch
+import matplotlib
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.postprocessing.connected_components import determine_postprocessing
+from CartiMorph_nnUNet.training.data_augmentation.data_augmentation_moreDA import get_moreDA_augmentation
+from CartiMorph_nnUNet.training.dataloading.dataset_loading import DataLoader3D, unpack_dataset
+from CartiMorph_nnUNet.evaluation.evaluator import aggregate_scores
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.paths import network_training_output_dir
+from CartiMorph_nnUNet.inference.segmentation_export import save_segmentation_nifti_from_softmax
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.training.data_augmentation.data_augmentation_moreDA import get_moreDA_augmentation
-from torch import nn
-from torch.nn.parallel import DistributedDataParallel as DDP
-from torch.nn.utils import clip_grad_norm_
+import numpy as np
+from CartiMorph_nnUNet.training.loss_functions.deep_supervision import MultipleOutputLoss2
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
+from CartiMorph_nnUNet.utilities.one_hot_encoding import to_one_hot
+import shutil
 
-from nnunet.evaluation.region_based_evaluation import evaluate_regions, get_brats_regions
-from nnunet.network_architecture.generic_UNet import Generic_UNet
-from nnunet.network_architecture.initialization import InitWeights_He
-from nnunet.network_architecture.neural_network import SegmentationNetwork
-from nnunet.training.dataloading.dataset_loading import unpack_dataset
-from nnunet.training.loss_functions.deep_supervision import MultipleOutputLoss2
-from nnunet.training.loss_functions.dice_loss import DC_and_BCE_loss, get_tp_fp_fn_tn, SoftDiceLoss
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
-from nnunet.training.network_training.nnUNetTrainerV2_DDP import nnUNetTrainerV2_DDP
-from nnunet.utilities.distributed import awesome_allgather_function
-from nnunet.utilities.to_torch import maybe_to_torch, to_cuda
+from torch import nn
 
+matplotlib.use("agg")
 
-class nnUNetTrainerV2BraTSRegions_BN(nnUNetTrainerV2):
-    def initialize_network(self):
-        if self.threeD:
-            conv_op = nn.Conv3d
-            dropout_op = nn.Dropout3d
-            norm_op = nn.BatchNorm3d
 
+class nnUNetTrainerV2CascadeFullRes(nnUNetTrainerV2):
+    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
+                 unpack_data=True, deterministic=True, previous_trainer="nnUNetTrainerV2", fp16=False):
+        super().__init__(plans_file, fold, output_folder, dataset_directory,
+                         batch_dice, stage, unpack_data, deterministic, fp16)
+        self.init_args = (plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
+                          deterministic, previous_trainer, fp16)
+
+        if self.output_folder is not None:
+            task = self.output_folder.split("/")[-3]
+            plans_identifier = self.output_folder.split("/")[-2].split("__")[-1]
+
+            folder_with_segs_prev_stage = join(network_training_output_dir, "3d_lowres",
+                                               task, previous_trainer + "__" + plans_identifier, "pred_next_stage")
+            self.folder_with_segs_from_prev_stage = folder_with_segs_prev_stage
+            # Do not put segs_prev_stage into self.output_folder as we need to unpack them for performance and we
+            # don't want to do that in self.output_folder because that one is located on some network drive.
         else:
-            conv_op = nn.Conv2d
-            dropout_op = nn.Dropout2d
-            norm_op = nn.BatchNorm2d
-
-        norm_op_kwargs = {'eps': 1e-5, 'affine': True}
-        dropout_op_kwargs = {'p': 0, 'inplace': True}
-        net_nonlin = nn.LeakyReLU
-        net_nonlin_kwargs = {'negative_slope': 1e-2, 'inplace': True}
-        self.network = Generic_UNet(self.num_input_channels, self.base_num_features, self.num_classes,
-                                    len(self.net_num_pool_op_kernel_sizes),
-                                    self.conv_per_stage, 2, conv_op, norm_op, norm_op_kwargs, dropout_op,
-                                    dropout_op_kwargs,
-                                    net_nonlin, net_nonlin_kwargs, True, False, lambda x: x, InitWeights_He(1e-2),
-                                    self.net_num_pool_op_kernel_sizes, self.net_conv_kernel_sizes, False, True, True)
-        if torch.cuda.is_available():
-            self.network.cuda()
-        self.network.inference_apply_nonlin = torch.nn.Softmax(1)
+            self.folder_with_segs_from_prev_stage = None
 
+    def do_split(self):
+        super().do_split()
+        for k in self.dataset:
+            self.dataset[k]['seg_from_prev_stage_file'] = join(self.folder_with_segs_from_prev_stage,
+                                                               k + "_segFromPrevStage.npz")
+            assert isfile(self.dataset[k]['seg_from_prev_stage_file']), \
+                "seg from prev stage missing: %s. " \
+                "Please run all 5 folds of the 3d_lowres configuration of this " \
+                "task!" % (self.dataset[k]['seg_from_prev_stage_file'])
+        for k in self.dataset_val:
+            self.dataset_val[k]['seg_from_prev_stage_file'] = join(self.folder_with_segs_from_prev_stage,
+                                                                   k + "_segFromPrevStage.npz")
+        for k in self.dataset_tr:
+            self.dataset_tr[k]['seg_from_prev_stage_file'] = join(self.folder_with_segs_from_prev_stage,
+                                                                  k + "_segFromPrevStage.npz")
+
+    def get_basic_generators(self):
+        self.load_dataset()
+        self.do_split()
 
-class nnUNetTrainerV2BraTSRegions(nnUNetTrainerV2):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.regions = get_brats_regions()
-        self.regions_class_order = (1, 2, 3)
-        self.loss = DC_and_BCE_loss({}, {'batch_dice': False, 'do_bg': True, 'smooth': 0})
+        if self.threeD:
+            dl_tr = DataLoader3D(self.dataset_tr, self.basic_generator_patch_size, self.patch_size, self.batch_size,
+                                 True, oversample_foreground_percent=self.oversample_foreground_percent,
+                                 pad_mode="constant", pad_sides=self.pad_all_sides)
+            dl_val = DataLoader3D(self.dataset_val, self.patch_size, self.patch_size, self.batch_size, True,
+                                  oversample_foreground_percent=self.oversample_foreground_percent,
+                                  pad_mode="constant", pad_sides=self.pad_all_sides)
+        else:
+            raise NotImplementedError("2D has no cascade")
+
+        return dl_tr, dl_val
 
     def process_plans(self, plans):
         super().process_plans(plans)
-        """
-        The network has as many outputs as we have regions
-        """
-        self.num_classes = len(self.regions)
+        self.num_input_channels += (self.num_classes - 1)  # for seg from prev stage
+
+    def setup_DA_params(self):
+        super().setup_DA_params()
+
+        self.data_aug_params["num_cached_per_thread"] = 2
+
+        self.data_aug_params['move_last_seg_chanel_to_data'] = True
+        self.data_aug_params['cascade_do_cascade_augmentations'] = True
+
+        self.data_aug_params['cascade_random_binary_transform_p'] = 0.4
+        self.data_aug_params['cascade_random_binary_transform_p_per_label'] = 1
+        self.data_aug_params['cascade_random_binary_transform_size'] = (1, 8)
+
+        self.data_aug_params['cascade_remove_conn_comp_p'] = 0.2
+        self.data_aug_params['cascade_remove_conn_comp_max_size_percent_threshold'] = 0.15
+        self.data_aug_params['cascade_remove_conn_comp_fill_with_other_class_p'] = 0.0
 
-    def initialize_network(self):
-        """inference_apply_nonlin to sigmoid"""
-        super().initialize_network()
-        self.network.inference_apply_nonlin = nn.Sigmoid()
+        # we have 2 channels now because the segmentation from the previous stage is stored in 'seg' as well until it
+        # is moved to 'data' at the end
+        self.data_aug_params['selected_seg_channels'] = [0, 1]
+        # needed for converting the segmentation from the previous stage to one hot
+        self.data_aug_params['all_segmentation_labels'] = list(range(1, self.num_classes))
 
     def initialize(self, training=True, force_load_plans=False):
         """
-        this is a copy of nnUNetTrainerV2's initialize. We only add the regions to the data augmentation
+        For prediction of test cases just set training=False, this will prevent loading of training data and
+        training batchgenerator initialization
         :param training:
-        :param force_load_plans:
         :return:
         """
         if not self.was_initialized:
-            maybe_mkdir_p(self.output_folder)
-
             if force_load_plans or (self.plans is None):
                 self.load_plans_file()
 
             self.process_plans(self.plans)
 
             self.setup_DA_params()
 
@@ -116,15 +144,21 @@
             self.ds_loss_weights = weights
             # now wrap the loss
             self.loss = MultipleOutputLoss2(self.loss, self.ds_loss_weights)
             ################# END ###################
 
             self.folder_with_preprocessed_data = join(self.dataset_directory, self.plans['data_identifier'] +
                                                       "_stage%d" % self.stage)
+
             if training:
+                if not isdir(self.folder_with_segs_from_prev_stage):
+                    raise RuntimeError(
+                        "Cannot run final stage of cascade. Run corresponding 3d_lowres first and predict the "
+                        "segmentations for the next stage")
+
                 self.dl_tr, self.dl_val = self.get_basic_generators()
                 if self.unpack_data:
                     print("unpacking dataset")
                     unpack_dataset(self.folder_with_preprocessed_data)
                     print("done")
                 else:
                     print(
@@ -132,289 +166,188 @@
                         "will wait all winter for your model to finish!")
 
                 self.tr_gen, self.val_gen = get_moreDA_augmentation(self.dl_tr, self.dl_val,
                                                                     self.data_aug_params[
                                                                         'patch_size_for_spatialtransform'],
                                                                     self.data_aug_params,
                                                                     deep_supervision_scales=self.deep_supervision_scales,
-                                                                    regions=self.regions)
+                                                                    pin_memory=self.pin_memory)
                 self.print_to_log_file("TRAINING KEYS:\n %s" % (str(self.dataset_tr.keys())),
                                        also_print_to_console=False)
                 self.print_to_log_file("VALIDATION KEYS:\n %s" % (str(self.dataset_val.keys())),
                                        also_print_to_console=False)
             else:
                 pass
 
             self.initialize_network()
             self.initialize_optimizer_and_scheduler()
 
             assert isinstance(self.network, (SegmentationNetwork, nn.DataParallel))
         else:
             self.print_to_log_file('self.was_initialized is True, not running self.initialize again')
+
         self.was_initialized = True
 
-    def validate(self, do_mirroring: bool = True, use_sliding_window: bool = True,
-                 step_size: int = 0.5, save_softmax: bool = True, use_gaussian: bool = True, overwrite: bool = True,
+    def validate(self, do_mirroring: bool = True, use_sliding_window: bool = True, step_size: float = 0.5,
+                 save_softmax: bool = True, use_gaussian: bool = True, overwrite: bool = True,
                  validation_folder_name: str = 'validation_raw', debug: bool = False, all_in_gpu: bool = False,
                  segmentation_export_kwargs: dict = None, run_postprocessing_on_folds: bool = True):
-        super().validate(do_mirroring=do_mirroring, use_sliding_window=use_sliding_window, step_size=step_size,
-                               save_softmax=save_softmax, use_gaussian=use_gaussian,
-                               overwrite=overwrite, validation_folder_name=validation_folder_name, debug=debug,
-                               all_in_gpu=all_in_gpu, segmentation_export_kwargs=segmentation_export_kwargs,
-                               run_postprocessing_on_folds=run_postprocessing_on_folds)
-        # run brats specific validation
-        output_folder = join(self.output_folder, validation_folder_name)
-        evaluate_regions(output_folder, self.gt_niftis_folder, self.regions)
+        assert self.was_initialized, "must initialize, ideally with checkpoint (or train first)"
 
-    def run_online_evaluation(self, output, target):
-        output = output[0]
-        target = target[0]
-        with torch.no_grad():
-            out_sigmoid = torch.sigmoid(output)
-            out_sigmoid = (out_sigmoid > 0.5).float()
-
-            if self.threeD:
-                axes = (0, 2, 3, 4)
+        current_mode = self.network.training
+        self.network.eval()
+        # save whether network is in deep supervision mode or not
+        ds = self.network.do_ds
+        # disable deep supervision
+        self.network.do_ds = False
+
+        if segmentation_export_kwargs is None:
+            if 'segmentation_export_params' in self.plans.keys():
+                force_separate_z = self.plans['segmentation_export_params']['force_separate_z']
+                interpolation_order = self.plans['segmentation_export_params']['interpolation_order']
+                interpolation_order_z = self.plans['segmentation_export_params']['interpolation_order_z']
             else:
-                axes = (0, 2, 3)
-
-            tp, fp, fn, _ = get_tp_fp_fn_tn(out_sigmoid, target, axes=axes)
-
-            tp_hard = tp.detach().cpu().numpy()
-            fp_hard = fp.detach().cpu().numpy()
-            fn_hard = fn.detach().cpu().numpy()
-
-            self.online_eval_foreground_dc.append(list((2 * tp_hard) / (2 * tp_hard + fp_hard + fn_hard + 1e-8)))
-            self.online_eval_tp.append(list(tp_hard))
-            self.online_eval_fp.append(list(fp_hard))
-            self.online_eval_fn.append(list(fn_hard))
-
-
-class nnUNetTrainerV2BraTSRegions_Dice(nnUNetTrainerV2BraTSRegions):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.loss = SoftDiceLoss(apply_nonlin=torch.sigmoid, **{'batch_dice': False, 'do_bg': True, 'smooth': 0})
-
-
-class nnUNetTrainerV2BraTSRegions_DDP(nnUNetTrainerV2_DDP):
-    def __init__(self, plans_file, fold, local_rank, output_folder=None, dataset_directory=None, batch_dice=True,
-                 stage=None,
-                 unpack_data=True, deterministic=True, distribute_batch_size=False, fp16=False):
-        super().__init__(plans_file, fold, local_rank, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, distribute_batch_size, fp16)
-        self.regions = get_brats_regions()
-        self.regions_class_order = (1, 2, 3)
-        self.loss = None
-        self.ce_loss = nn.BCEWithLogitsLoss()
-
-    def process_plans(self, plans):
-        super().process_plans(plans)
-        """
-        The network has as many outputs as we have regions
-        """
-        self.num_classes = len(self.regions)
-
-    def initialize_network(self):
-        """inference_apply_nonlin to sigmoid"""
-        super().initialize_network()
-        self.network.inference_apply_nonlin = nn.Sigmoid()
-
-    def initialize(self, training=True, force_load_plans=False):
-        """
-        this is a copy of nnUNetTrainerV2's initialize. We only add the regions to the data augmentation
-        :param training:
-        :param force_load_plans:
-        :return:
-        """
-        if not self.was_initialized:
-            maybe_mkdir_p(self.output_folder)
-
-            if force_load_plans or (self.plans is None):
-                self.load_plans_file()
-
-            self.process_plans(self.plans)
-
-            self.setup_DA_params()
-
-            self.folder_with_preprocessed_data = join(self.dataset_directory, self.plans['data_identifier'] +
-                                                      "_stage%d" % self.stage)
-            if training:
-                self.dl_tr, self.dl_val = self.get_basic_generators()
-                if self.unpack_data:
-                    if self.local_rank == 0:
-                        print("unpacking dataset")
-                        unpack_dataset(self.folder_with_preprocessed_data)
-                        print("done")
-                    else:
-                        # we need to wait until worker 0 has finished unpacking
-                        npz_files = subfiles(self.folder_with_preprocessed_data, suffix=".npz", join=False)
-                        case_ids = [i[:-4] for i in npz_files]
-                        all_present = all(
-                            [isfile(join(self.folder_with_preprocessed_data, i + ".npy")) for i in case_ids])
-                        while not all_present:
-                            print("worker", self.local_rank, "is waiting for unpacking")
-                            sleep(3)
-                            all_present = all(
-                                [isfile(join(self.folder_with_preprocessed_data, i + ".npy")) for i in case_ids])
-                        # there is some slight chance that there may arise some error because dataloader are loading a file
-                        # that is still being written by worker 0. We ignore this for now an address it only if it becomes
-                        # relevant
-                        # (this can occur because while worker 0 writes the file is technically present so the other workers
-                        # will proceed and eventually try to read it)
-                else:
-                    print(
-                        "INFO: Not unpacking data! Training may be slow due to that. Pray you are not using 2d or you "
-                        "will wait all winter for your model to finish!")
-
-                # setting weights for deep supervision losses
-                net_numpool = len(self.net_num_pool_op_kernel_sizes)
-
-                # we give each output a weight which decreases exponentially (division by 2) as the resolution decreases
-                # this gives higher resolution outputs more weight in the loss
-                weights = np.array([1 / (2 ** i) for i in range(net_numpool)])
-
-                # we don't use the lowest 2 outputs. Normalize weights so that they sum to 1
-                mask = np.array([True if i < net_numpool - 1 else False for i in range(net_numpool)])
-                weights[~mask] = 0
-                weights = weights / weights.sum()
-                self.ds_loss_weights = weights
-
-                seeds_train = np.random.random_integers(0, 99999, self.data_aug_params.get('num_threads'))
-                seeds_val = np.random.random_integers(0, 99999, max(self.data_aug_params.get('num_threads') // 2, 1))
-                print("seeds train", seeds_train)
-                print("seeds_val", seeds_val)
-                self.tr_gen, self.val_gen = get_moreDA_augmentation(self.dl_tr, self.dl_val,
-                                                                    self.data_aug_params[
-                                                                        'patch_size_for_spatialtransform'],
-                                                                    self.data_aug_params,
-                                                                    deep_supervision_scales=self.deep_supervision_scales,
-                                                                    seeds_train=seeds_train,
-                                                                    seeds_val=seeds_val,
-                                                                    pin_memory=self.pin_memory,
-                                                                    regions=self.regions)
-                self.print_to_log_file("TRAINING KEYS:\n %s" % (str(self.dataset_tr.keys())),
-                                       also_print_to_console=False)
-                self.print_to_log_file("VALIDATION KEYS:\n %s" % (str(self.dataset_val.keys())),
-                                       also_print_to_console=False)
-            else:
-                pass
-
-            self.initialize_network()
-            self.initialize_optimizer_and_scheduler()
-            self._maybe_init_amp()
-            self.network = DDP(self.network, self.local_rank)
-
+                force_separate_z = None
+                interpolation_order = 1
+                interpolation_order_z = 0
         else:
-            self.print_to_log_file('self.was_initialized is True, not running self.initialize again')
-        self.was_initialized = True
+            force_separate_z = segmentation_export_kwargs['force_separate_z']
+            interpolation_order = segmentation_export_kwargs['interpolation_order']
+            interpolation_order_z = segmentation_export_kwargs['interpolation_order_z']
+
+        if self.dataset_val is None:
+            self.load_dataset()
+            self.do_split()
 
-    def validate(self, do_mirroring: bool = True, use_sliding_window: bool = True,
-                 step_size: int = 0.5, save_softmax: bool = True, use_gaussian: bool = True, overwrite: bool = True,
-                 validation_folder_name: str = 'validation_raw', debug: bool = False, all_in_gpu: bool = False,
-                 segmentation_export_kwargs: dict = None, run_postprocessing_on_folds: bool = True):
-        super().validate(do_mirroring=do_mirroring, use_sliding_window=use_sliding_window, step_size=step_size,
-                               save_softmax=save_softmax, use_gaussian=use_gaussian,
-                               overwrite=overwrite, validation_folder_name=validation_folder_name, debug=debug,
-                               all_in_gpu=all_in_gpu, segmentation_export_kwargs=segmentation_export_kwargs,
-                               run_postprocessing_on_folds=run_postprocessing_on_folds)
-        # run brats specific validation
         output_folder = join(self.output_folder, validation_folder_name)
-        evaluate_regions(output_folder, self.gt_niftis_folder, self.regions)
-
-    def run_iteration(self, data_generator, do_backprop=True, run_online_evaluation=False):
-        raise NotImplementedError("this class has not been changed to work with pytorch amp yet!")
-        data_dict = next(data_generator)
-        data = data_dict['data']
-        target = data_dict['target']
-
-        data = maybe_to_torch(data)
-        target = maybe_to_torch(target)
-
-        if torch.cuda.is_available():
-            data = to_cuda(data, gpu_id=None)
-            target = to_cuda(target, gpu_id=None)
-
-        self.optimizer.zero_grad()
-
-        output = self.network(data)
-        del data
-
-        total_loss = None
-
-        for i in range(len(output)):
-            # Starting here it gets spicy!
-            axes = tuple(range(2, len(output[i].size())))
-
-            # network does not do softmax. We need to do softmax for dice
-            output_softmax = torch.sigmoid(output[i])
-
-            # get the tp, fp and fn terms we need
-            tp, fp, fn, _ = get_tp_fp_fn_tn(output_softmax, target[i], axes, mask=None)
-            # for dice, compute nominator and denominator so that we have to accumulate only 2 instead of 3 variables
-            # do_bg=False in nnUNetTrainer -> [:, 1:]
-            nominator = 2 * tp[:, 1:]
-            denominator = 2 * tp[:, 1:] + fp[:, 1:] + fn[:, 1:]
-
-            if self.batch_dice:
-                # for DDP we need to gather all nominator and denominator terms from all GPUS to do proper batch dice
-                nominator = awesome_allgather_function.apply(nominator)
-                denominator = awesome_allgather_function.apply(denominator)
-                nominator = nominator.sum(0)
-                denominator = denominator.sum(0)
-            else:
-                pass
+        maybe_mkdir_p(output_folder)
+        # this is for debug purposes
+        my_input_args = {'do_mirroring': do_mirroring,
+                         'use_sliding_window': use_sliding_window,
+                         'step': step_size,
+                         'save_softmax': save_softmax,
+                         'use_gaussian': use_gaussian,
+                         'overwrite': overwrite,
+                         'validation_folder_name': validation_folder_name,
+                         'debug': debug,
+                         'all_in_gpu': all_in_gpu,
+                         'segmentation_export_kwargs': segmentation_export_kwargs,
+                         }
+        save_json(my_input_args, join(output_folder, "validation_args.json"))
+
+        if do_mirroring:
+            if not self.data_aug_params['do_mirror']:
+                raise RuntimeError("We did not train with mirroring so you cannot do inference with mirroring enabled")
+            mirror_axes = self.data_aug_params['mirror_axes']
+        else:
+            mirror_axes = ()
 
-            ce_loss = self.ce_loss(output[i], target[i])
+        pred_gt_tuples = []
 
-            # we smooth by 1e-5 to penalize false positives if tp is 0
-            dice_loss = (- (nominator + 1e-5) / (denominator + 1e-5)).mean()
-            if total_loss is None:
-                total_loss = self.ds_loss_weights[i] * (ce_loss + dice_loss)
-            else:
-                total_loss += self.ds_loss_weights[i] * (ce_loss + dice_loss)
+        export_pool = Pool(default_num_threads)
+        results = []
 
-        if run_online_evaluation:
-            with torch.no_grad():
-                output = output[0]
-                target = target[0]
-                out_sigmoid = torch.sigmoid(output)
-                out_sigmoid = (out_sigmoid > 0.5).float()
+        for k in self.dataset_val.keys():
+            properties = load_pickle(self.dataset[k]['properties_file'])
+            fname = properties['list_of_data_files'][0].split("/")[-1][:-12]
 
-                if self.threeD:
-                    axes = (2, 3, 4)
-                else:
-                    axes = (2, 3)
+            if overwrite or (not isfile(join(output_folder, fname + ".nii.gz"))) or \
+                    (save_softmax and not isfile(join(output_folder, fname + ".npz"))):
+                data = np.load(self.dataset[k]['data_file'])['data']
 
-                tp, fp, fn, _ = get_tp_fp_fn_tn(out_sigmoid, target, axes=axes)
+                # concat segmentation of previous step
+                seg_from_prev_stage = np.load(join(self.folder_with_segs_from_prev_stage,
+                                                   k + "_segFromPrevStage.npz"))['data'][None]
 
-                tp_hard = awesome_allgather_function.apply(tp)
-                fp_hard = awesome_allgather_function.apply(fp)
-                fn_hard = awesome_allgather_function.apply(fn)
-                # print_if_rank0("after allgather", tp_hard.shape)
+                print(k, data.shape)
+                data[-1][data[-1] == -1] = 0
 
-                # print_if_rank0("after sum", tp_hard.shape)
+                data_for_net = np.concatenate((data[:-1], to_one_hot(seg_from_prev_stage[0], range(1, self.num_classes))))
 
-                self.run_online_evaluation(tp_hard.detach().cpu().numpy().sum(0),
-                                           fp_hard.detach().cpu().numpy().sum(0),
-                                           fn_hard.detach().cpu().numpy().sum(0))
-        del target
+                softmax_pred = self.predict_preprocessed_data_return_seg_and_softmax(data_for_net,
+                                                                                     do_mirroring=do_mirroring,
+                                                                                     mirror_axes=mirror_axes,
+                                                                                     use_sliding_window=use_sliding_window,
+                                                                                     step_size=step_size,
+                                                                                     use_gaussian=use_gaussian,
+                                                                                     all_in_gpu=all_in_gpu,
+                                                                                     mixed_precision=self.fp16)[1]
 
-        if do_backprop:
-            if not self.fp16 or amp is None or not torch.cuda.is_available():
-                total_loss.backward()
-            else:
-                with amp.scale_loss(total_loss, self.optimizer) as scaled_loss:
-                    scaled_loss.backward()
-            _ = clip_grad_norm_(self.network.parameters(), 12)
-            self.optimizer.step()
-
-        return total_loss.detach().cpu().numpy()
-
-    def run_online_evaluation(self, tp, fp, fn):
-        self.online_eval_foreground_dc.append(list((2 * tp) / (2 * tp + fp + fn + 1e-8)))
-        self.online_eval_tp.append(list(tp))
-        self.online_eval_fp.append(list(fp))
-        self.online_eval_fn.append(list(fn))
+                softmax_pred = softmax_pred.transpose([0] + [i + 1 for i in self.transpose_backward])
 
+                if save_softmax:
+                    softmax_fname = join(output_folder, fname + ".npz")
+                else:
+                    softmax_fname = None
 
+                """There is a problem with python process communication that prevents us from communicating objects 
+                larger than 2 GB between processes (basically when the length of the pickle string that will be sent is 
+                communicated by the multiprocessing.Pipe object then the placeholder (I think) does not allow for long 
+                enough strings (lol). This could be fixed by changing i to l (for long) but that would require manually 
+                patching system python code. We circumvent that problem here by saving softmax_pred to a npy file that will 
+                then be read (and finally deleted) by the Process. save_segmentation_nifti_from_softmax can take either 
+                filename or np.ndarray and will handle this automatically"""
+                if np.prod(softmax_pred.shape) > (2e9 / 4 * 0.85):  # *0.85 just to be save
+                    np.save(join(output_folder, fname + ".npy"), softmax_pred)
+                    softmax_pred = join(output_folder, fname + ".npy")
+
+                results.append(export_pool.starmap_async(save_segmentation_nifti_from_softmax,
+                                                         ((softmax_pred, join(output_folder, fname + ".nii.gz"),
+                                                           properties, interpolation_order, None, None, None,
+                                                           softmax_fname, None, force_separate_z,
+                                                           interpolation_order_z),
+                                                          )
+                                                         )
+                               )
+
+            pred_gt_tuples.append([join(output_folder, fname + ".nii.gz"),
+                                   join(self.gt_niftis_folder, fname + ".nii.gz")])
+
+        _ = [i.get() for i in results]
+        self.print_to_log_file("finished prediction")
+
+        # evaluate raw predictions
+        self.print_to_log_file("evaluation of raw predictions")
+        task = self.dataset_directory.split("/")[-1]
+        job_name = self.experiment_name
+        _ = aggregate_scores(pred_gt_tuples, labels=list(range(self.num_classes)),
+                             json_output_file=join(output_folder, "summary.json"),
+                             json_name=job_name + " val tiled %s" % (str(use_sliding_window)),
+                             json_author="Fabian",
+                             json_task=task, num_threads=default_num_threads)
+
+        if run_postprocessing_on_folds:
+            # in the old nnunet we would stop here. Now we add a postprocessing. This postprocessing can remove everything
+            # except the largest connected component for each class. To see if this improves results, we do this for all
+            # classes and then rerun the evaluation. Those classes for which this resulted in an improved dice score will
+            # have this applied during inference as well
+            self.print_to_log_file("determining postprocessing")
+            determine_postprocessing(self.output_folder, self.gt_niftis_folder, validation_folder_name,
+                                     final_subf_name=validation_folder_name + "_postprocessed", debug=debug)
+            # after this the final predictions for the vlaidation set can be found in validation_folder_name_base + "_postprocessed"
+            # They are always in that folder, even if no postprocessing as applied!
+
+        # detemining postprocesing on a per-fold basis may be OK for this fold but what if another fold finds another
+        # postprocesing to be better? In this case we need to consolidate. At the time the consolidation is going to be
+        # done we won't know what self.gt_niftis_folder was, so now we copy all the niftis into a separate folder to
+        # be used later
+        gt_nifti_folder = join(self.output_folder_base, "gt_niftis")
+        maybe_mkdir_p(gt_nifti_folder)
+        for f in subfiles(self.gt_niftis_folder, suffix=".nii.gz"):
+            success = False
+            attempts = 0
+            e = None
+            while not success and attempts < 10:
+                try:
+                    shutil.copy(f, gt_nifti_folder)
+                    success = True
+                except OSError as e:
+                    attempts += 1
+                    sleep(1)
+            if not success:
+                print("Could not copy gt nifti file %s into folder %s" % (f, gt_nifti_folder))
+                if e is not None:
+                    raise e
+
+        # restore network deep supervision mode
+        self.network.train(current_mode)
+        self.network.do_ds = ds
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/competitions_with_custom_Trainers/BraTS2020/nnUNetTrainerV2BraTSRegions_moreDA.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerV2.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,56 +9,63 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
+from collections import OrderedDict
+from typing import Tuple
+
 import numpy as np
 import torch
-from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.training.data_augmentation.data_augmentation_insaneDA2 import get_insaneDA_augmentation2
+from CartiMorph_nnUNet.training.data_augmentation.data_augmentation_moreDA import get_moreDA_augmentation
+from CartiMorph_nnUNet.training.loss_functions.deep_supervision import MultipleOutputLoss2
+from CartiMorph_nnUNet.utilities.to_torch import maybe_to_torch, to_cuda
+from CartiMorph_nnUNet.network_architecture.generic_UNet import Generic_UNet
+from CartiMorph_nnUNet.network_architecture.initialization import InitWeights_He
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.training.data_augmentation.default_data_augmentation import default_2D_augmentation_params, \
+    get_patch_size, default_3D_augmentation_params
+from CartiMorph_nnUNet.training.dataloading.dataset_loading import unpack_dataset
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.utilities.nd_softmax import softmax_helper
+from sklearn.model_selection import KFold
 from torch import nn
+from torch.cuda.amp import autocast
+from CartiMorph_nnUNet.training.learning_rate.poly_lr import poly_lr
+from batchgenerators.utilities.file_and_folder_operations import *
 
-from nnunet.evaluation.region_based_evaluation import evaluate_regions, get_brats_regions
-from nnunet.network_architecture.generic_UNet import Generic_UNet
-from nnunet.network_architecture.initialization import InitWeights_He
-from nnunet.network_architecture.neural_network import SegmentationNetwork
-from nnunet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params, \
-    default_2D_augmentation_params, get_patch_size
-from nnunet.training.dataloading.dataset_loading import unpack_dataset
-from nnunet.training.loss_functions.deep_supervision import MultipleOutputLoss2
-from nnunet.training.loss_functions.dice_loss import DC_and_BCE_loss, get_tp_fp_fn_tn
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
-from nnunet.training.network_training.nnUNet_variants.data_augmentation.nnUNetTrainerV2_DA3 import \
-    nnUNetTrainerV2_DA3_BN
 
+class nnUNetTrainer_CMTbase(nnUNetTrainer):
+    """
+    Info for Fabian: same as internal nnUNetTrainerV2_2
+    """
 
-class nnUNetTrainerV2BraTSRegions_DA3_BN(nnUNetTrainerV2_DA3_BN):
     def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
                  unpack_data=True, deterministic=True, fp16=False):
         super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
                          deterministic, fp16)
-        self.regions = get_brats_regions()
-        self.regions_class_order = (1, 2, 3)
-        self.loss = DC_and_BCE_loss({}, {'batch_dice': False, 'do_bg': True, 'smooth': 0})
+        self.max_num_epochs = 1000
+        self.initial_lr = 1e-2
+        self.deep_supervision_scales = None
+        self.ds_loss_weights = None
 
-    def process_plans(self, plans):
-        super().process_plans(plans)
-        """
-        The network has as many outputs as we have regions
-        """
-        self.num_classes = len(self.regions)
-
-    def initialize_network(self):
-        """inference_apply_nonlin to sigmoid"""
-        super().initialize_network()
-        self.network.inference_apply_nonlin = nn.Sigmoid()
+        self.pin_memory = True
 
     def initialize(self, training=True, force_load_plans=False):
+        """
+        - replaced get_default_augmentation with get_moreDA_augmentation
+        - enforce to only run this code once
+        - loss function wrapper for deep supervision
+
+        :param training:
+        :param force_load_plans:
+        :return:
+        """
         if not self.was_initialized:
             maybe_mkdir_p(self.output_folder)
 
             if force_load_plans or (self.plans is None):
                 self.load_plans_file()
 
             self.process_plans(self.plans)
@@ -91,22 +98,22 @@
                     unpack_dataset(self.folder_with_preprocessed_data)
                     print("done")
                 else:
                     print(
                         "INFO: Not unpacking data! Training may be slow due to that. Pray you are not using 2d or you "
                         "will wait all winter for your model to finish!")
 
-                self.tr_gen, self.val_gen = get_insaneDA_augmentation2(
+                self.tr_gen, self.val_gen = get_moreDA_augmentation(
                     self.dl_tr, self.dl_val,
                     self.data_aug_params[
                         'patch_size_for_spatialtransform'],
                     self.data_aug_params,
                     deep_supervision_scales=self.deep_supervision_scales,
                     pin_memory=self.pin_memory,
-                    regions=self.regions
+                    use_nondetMultiThreadedAugmenter=False
                 )
                 self.print_to_log_file("TRAINING KEYS:\n %s" % (str(self.dataset_tr.keys())),
                                        also_print_to_console=False)
                 self.print_to_log_file("VALIDATION KEYS:\n %s" % (str(self.dataset_val.keys())),
                                        also_print_to_console=False)
             else:
                 pass
@@ -115,53 +122,25 @@
             self.initialize_optimizer_and_scheduler()
 
             assert isinstance(self.network, (SegmentationNetwork, nn.DataParallel))
         else:
             self.print_to_log_file('self.was_initialized is True, not running self.initialize again')
         self.was_initialized = True
 
-    def validate(self, do_mirroring: bool = True, use_sliding_window: bool = True,
-                 step_size: int = 0.5, save_softmax: bool = True, use_gaussian: bool = True, overwrite: bool = True,
-                 validation_folder_name: str = 'validation_raw', debug: bool = False, all_in_gpu: bool = False,
-                 segmentation_export_kwargs: dict = None, run_postprocessing_on_folds: bool = True):
-        super().validate(do_mirroring=do_mirroring, use_sliding_window=use_sliding_window, step_size=step_size,
-                         save_softmax=save_softmax, use_gaussian=use_gaussian,
-                         overwrite=overwrite, validation_folder_name=validation_folder_name, debug=debug,
-                         all_in_gpu=all_in_gpu, segmentation_export_kwargs=segmentation_export_kwargs,
-                         run_postprocessing_on_folds=run_postprocessing_on_folds)
-        # run brats specific validation
-        output_folder = join(self.output_folder, validation_folder_name)
-        evaluate_regions(output_folder, self.gt_niftis_folder, self.regions)
-
-    def run_online_evaluation(self, output, target):
-        output = output[0]
-        target = target[0]
-        with torch.no_grad():
-            out_sigmoid = torch.sigmoid(output)
-            out_sigmoid = (out_sigmoid > 0.5).float()
-
-            if self.threeD:
-                axes = (0, 2, 3, 4)
-            else:
-                axes = (0, 2, 3)
-
-            tp, fp, fn, _ = get_tp_fp_fn_tn(out_sigmoid, target, axes=axes)
-
-            tp_hard = tp.detach().cpu().numpy()
-            fp_hard = fp.detach().cpu().numpy()
-            fn_hard = fn.detach().cpu().numpy()
-
-            self.online_eval_foreground_dc.append(list((2 * tp_hard) / (2 * tp_hard + fp_hard + fn_hard + 1e-8)))
-            self.online_eval_tp.append(list(tp_hard))
-            self.online_eval_fp.append(list(fp_hard))
-            self.online_eval_fn.append(list(fn_hard))
-
-
-class nnUNetTrainerV2BraTSRegions_DA3(nnUNetTrainerV2BraTSRegions_DA3_BN):
     def initialize_network(self):
+        """
+        - momentum 0.99
+        - SGD instead of Adam
+        - self.lr_scheduler = None because we do poly_lr
+        - deep supervision = True
+        - i am sure I forgot something here
+
+        Known issue: forgot to set neg_slope=0 in InitWeights_He; should not make a difference though
+        :return:
+        """
         if self.threeD:
             conv_op = nn.Conv3d
             dropout_op = nn.Dropout3d
             norm_op = nn.InstanceNorm3d
 
         else:
             conv_op = nn.Conv2d
@@ -172,60 +151,227 @@
         dropout_op_kwargs = {'p': 0, 'inplace': True}
         net_nonlin = nn.LeakyReLU
         net_nonlin_kwargs = {'negative_slope': 1e-2, 'inplace': True}
         self.network = Generic_UNet(self.num_input_channels, self.base_num_features, self.num_classes,
                                     len(self.net_num_pool_op_kernel_sizes),
                                     self.conv_per_stage, 2, conv_op, norm_op, norm_op_kwargs, dropout_op,
                                     dropout_op_kwargs,
-                                    net_nonlin, net_nonlin_kwargs, True, False, lambda x: x, InitWeights_He(1e-2),
+                                    net_nonlin, net_nonlin_kwargs, True, False, self.my_activation, InitWeights_He(1e-2),
                                     self.net_num_pool_op_kernel_sizes, self.net_conv_kernel_sizes, False, True, True)
         if torch.cuda.is_available():
             self.network.cuda()
-        self.network.inference_apply_nonlin = nn.Sigmoid()
+        self.network.inference_apply_nonlin = softmax_helper
 
+    def my_activation(self, x):
+        return x
 
-class nnUNetTrainerV2BraTSRegions_DA3_BD(nnUNetTrainerV2BraTSRegions_DA3):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.loss = DC_and_BCE_loss({}, {'batch_dice': True, 'do_bg': True, 'smooth': 0})
+    def initialize_optimizer_and_scheduler(self):
+        assert self.network is not None, "self.initialize_network must be called first"
+        self.optimizer = torch.optim.SGD(self.network.parameters(), self.initial_lr, weight_decay=self.weight_decay,
+                                         momentum=0.99, nesterov=True)
+        self.lr_scheduler = None
 
+    def run_online_evaluation(self, output, target):
+        """
+        due to deep supervision the return value and the reference are now lists of tensors. We only need the full
+        resolution output because this is what we are interested in in the end. The others are ignored
+        :param output:
+        :param target:
+        :return:
+        """
+        target = target[0]
+        output = output[0]
+        return super().run_online_evaluation(output, target)
 
-class nnUNetTrainerV2BraTSRegions_DA3_BN_BD(nnUNetTrainerV2BraTSRegions_DA3_BN):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.loss = DC_and_BCE_loss({}, {'batch_dice': True, 'do_bg': True, 'smooth': 0})
+    def validate(self, do_mirroring: bool = True, use_sliding_window: bool = True,
+                 step_size: float = 0.5, save_softmax: bool = True, use_gaussian: bool = True, overwrite: bool = True,
+                 validation_folder_name: str = 'validation_raw', debug: bool = False, all_in_gpu: bool = False,
+                 segmentation_export_kwargs: dict = None, run_postprocessing_on_folds: bool = True):
+        """
+        We need to wrap this because we need to enforce self.network.do_ds = False for prediction
+        """
+        ds = self.network.do_ds
+        self.network.do_ds = False
+        ret = super().validate(do_mirroring=do_mirroring, use_sliding_window=use_sliding_window, step_size=step_size,
+                               save_softmax=save_softmax, use_gaussian=use_gaussian,
+                               overwrite=overwrite, validation_folder_name=validation_folder_name, debug=debug,
+                               all_in_gpu=all_in_gpu, segmentation_export_kwargs=segmentation_export_kwargs,
+                               run_postprocessing_on_folds=run_postprocessing_on_folds)
+
+        self.network.do_ds = ds
+        return ret
+
+    def predict_preprocessed_data_return_seg_and_softmax(self, data: np.ndarray, do_mirroring: bool = True,
+                                                         mirror_axes: Tuple[int] = None,
+                                                         use_sliding_window: bool = True, step_size: float = 0.5,
+                                                         use_gaussian: bool = True, pad_border_mode: str = 'constant',
+                                                         pad_kwargs: dict = None, all_in_gpu: bool = False,
+                                                         verbose: bool = True, mixed_precision=True) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        We need to wrap this because we need to enforce self.network.do_ds = False for prediction
+        """
+        ds = self.network.do_ds
+        self.network.do_ds = False
+        ret = super().predict_preprocessed_data_return_seg_and_softmax(data,
+                                                                       do_mirroring=do_mirroring,
+                                                                       mirror_axes=mirror_axes,
+                                                                       use_sliding_window=use_sliding_window,
+                                                                       step_size=step_size, use_gaussian=use_gaussian,
+                                                                       pad_border_mode=pad_border_mode,
+                                                                       pad_kwargs=pad_kwargs, all_in_gpu=all_in_gpu,
+                                                                       verbose=verbose,
+                                                                       mixed_precision=mixed_precision)
+        self.network.do_ds = ds
+        return ret
+
+    def run_iteration(self, data_generator, do_backprop=True, run_online_evaluation=False):
+        """
+        gradient clipping improves training stability
+
+        :param data_generator:
+        :param do_backprop:
+        :param run_online_evaluation:
+        :return:
+        """
+        data_dict = next(data_generator)
+        data = data_dict['data']
+        target = data_dict['target']
+
+        data = maybe_to_torch(data)
+        target = maybe_to_torch(target)
+
+        if torch.cuda.is_available():
+            data = to_cuda(data)
+            target = to_cuda(target)
+
+        self.optimizer.zero_grad()
+
+        if self.fp16:
+            with autocast():
+                output = self.network(data)
+                del data
+                l = self.loss(output, target)
+
+            if do_backprop:
+                self.amp_grad_scaler.scale(l).backward()
+                self.amp_grad_scaler.unscale_(self.optimizer)
+                torch.nn.utils.clip_grad_norm_(self.network.parameters(), 12)
+                self.amp_grad_scaler.step(self.optimizer)
+                self.amp_grad_scaler.update()
+        else:
+            output = self.network(data)
+            del data
+            l = self.loss(output, target)
+
+            if do_backprop:
+                l.backward()
+                torch.nn.utils.clip_grad_norm_(self.network.parameters(), 12)
+                self.optimizer.step()
+
+        if run_online_evaluation:
+            self.run_online_evaluation(output, target)
+
+        del target
+
+        return l.detach().cpu().numpy()
+
+    def do_split(self):
+        """
+        The default split is a 5 fold CV on all available training cases. nnU-Net will create a split (it is seeded,
+        so always the same) and save it as splits_final.pkl file in the preprocessed data directory.
+        Sometimes you may want to create your own split for various reasons. For this you will need to create your own
+        splits_final.pkl file. If this file is present, nnU-Net is going to use it and whatever splits are defined in
+        it. You can create as many splits in this file as you want. Note that if you define only 4 splits (fold 0-3)
+        and then set fold=4 when training (that would be the fifth split), nnU-Net will print a warning and proceed to
+        use a random 80:20 data split.
+        :return:
+        """
+        if self.fold == "all":
+            # if fold==all then we use all images for training and validation
+            tr_keys = val_keys = list(self.dataset.keys())
+        else:
+            splits_file = join(self.dataset_directory, "splits_final.pkl")
 
+            # if the split file does not exist we need to create it
+            if not isfile(splits_file):
+                self.print_to_log_file("Creating new 5-fold cross-validation split...")
+                splits = []
+                all_keys_sorted = np.sort(list(self.dataset.keys()))
+                kfold = KFold(n_splits=5, shuffle=True, random_state=12345)
+                for i, (train_idx, test_idx) in enumerate(kfold.split(all_keys_sorted)):
+                    train_keys = np.array(all_keys_sorted)[train_idx]
+                    test_keys = np.array(all_keys_sorted)[test_idx]
+                    splits.append(OrderedDict())
+                    splits[-1]['train'] = train_keys
+                    splits[-1]['val'] = test_keys
+                save_pickle(splits, splits_file)
+
+            else:
+                self.print_to_log_file("Using splits from existing split file:", splits_file)
+                splits = load_pickle(splits_file)
+                self.print_to_log_file("The split file contains %d splits." % len(splits))
+
+            self.print_to_log_file("Desired fold for training: %d" % self.fold)
+            if self.fold < len(splits):
+                tr_keys = splits[self.fold]['train']
+                val_keys = splits[self.fold]['val']
+                self.print_to_log_file("This split has %d training and %d validation cases."
+                                       % (len(tr_keys), len(val_keys)))
+            else:
+                self.print_to_log_file("INFO: You requested fold %d for training but splits "
+                                       "contain only %d folds. I am now creating a "
+                                       "random (but seeded) 80:20 split!" % (self.fold, len(splits)))
+                # if we request a fold that is not in the split file, create a random 80:20 split
+                rnd = np.random.RandomState(seed=12345 + self.fold)
+                keys = np.sort(list(self.dataset.keys()))
+                idx_tr = rnd.choice(len(keys), int(len(keys) * 0.8), replace=False)
+                idx_val = [i for i in range(len(keys)) if i not in idx_tr]
+                tr_keys = [keys[i] for i in idx_tr]
+                val_keys = [keys[i] for i in idx_val]
+                self.print_to_log_file("This random 80:20 split has %d training and %d validation cases."
+                                       % (len(tr_keys), len(val_keys)))
+
+        tr_keys.sort()
+        val_keys.sort()
+        self.dataset_tr = OrderedDict()
+        for i in tr_keys:
+            self.dataset_tr[i] = self.dataset[i]
+        self.dataset_val = OrderedDict()
+        for i in val_keys:
+            self.dataset_val[i] = self.dataset[i]
 
-class nnUNetTrainerV2BraTSRegions_DA4_BN(nnUNetTrainerV2BraTSRegions_DA3_BN):
     def setup_DA_params(self):
-        nnUNetTrainerV2.setup_DA_params(self)
+        """
+        - we increase roation angle from [-15, 15] to [-30, 30]
+        - scale range is now (0.7, 1.4), was (0.85, 1.25)
+        - we don't do elastic deformation anymore
+
+        :return:
+        """
+
         self.deep_supervision_scales = [[1, 1, 1]] + list(list(i) for i in 1 / np.cumprod(
             np.vstack(self.net_num_pool_op_kernel_sizes), axis=0))[:-1]
 
         if self.threeD:
             self.data_aug_params = default_3D_augmentation_params
-            self.data_aug_params['rotation_x'] = (-90. / 360 * 2. * np.pi, 90. / 360 * 2. * np.pi)
-            self.data_aug_params['rotation_y'] = (-90. / 360 * 2. * np.pi, 90. / 360 * 2. * np.pi)
-            self.data_aug_params['rotation_z'] = (-90. / 360 * 2. * np.pi, 90. / 360 * 2. * np.pi)
+            self.data_aug_params['rotation_x'] = (-30. / 360 * 2. * np.pi, 30. / 360 * 2. * np.pi)
+            self.data_aug_params['rotation_y'] = (-30. / 360 * 2. * np.pi, 30. / 360 * 2. * np.pi)
+            self.data_aug_params['rotation_z'] = (-30. / 360 * 2. * np.pi, 30. / 360 * 2. * np.pi)
             if self.do_dummy_2D_aug:
                 self.data_aug_params["dummy_2D"] = True
                 self.print_to_log_file("Using dummy2d data augmentation")
                 self.data_aug_params["elastic_deform_alpha"] = \
                     default_2D_augmentation_params["elastic_deform_alpha"]
                 self.data_aug_params["elastic_deform_sigma"] = \
                     default_2D_augmentation_params["elastic_deform_sigma"]
                 self.data_aug_params["rotation_x"] = default_2D_augmentation_params["rotation_x"]
         else:
             self.do_dummy_2D_aug = False
             if max(self.patch_size) / min(self.patch_size) > 1.5:
-                default_2D_augmentation_params['rotation_x'] = (-180. / 360 * 2. * np.pi, 180. / 360 * 2. * np.pi)
+                default_2D_augmentation_params['rotation_x'] = (-15. / 360 * 2. * np.pi, 15. / 360 * 2. * np.pi)
             self.data_aug_params = default_2D_augmentation_params
         self.data_aug_params["mask_was_used_for_normalization"] = self.use_mask_for_norm
 
         if self.do_dummy_2D_aug:
             self.basic_generator_patch_size = get_patch_size(self.patch_size[1:],
                                                              self.data_aug_params['rotation_x'],
                                                              self.data_aug_params['rotation_y'],
@@ -234,38 +380,77 @@
             self.basic_generator_patch_size = np.array([self.patch_size[0]] + list(self.basic_generator_patch_size))
         else:
             self.basic_generator_patch_size = get_patch_size(self.patch_size, self.data_aug_params['rotation_x'],
                                                              self.data_aug_params['rotation_y'],
                                                              self.data_aug_params['rotation_z'],
                                                              self.data_aug_params['scale_range'])
 
+        self.data_aug_params["scale_range"] = (0.7, 1.4)
+        self.data_aug_params["do_elastic"] = False
         self.data_aug_params['selected_seg_channels'] = [0]
         self.data_aug_params['patch_size_for_spatialtransform'] = self.patch_size
 
-        self.data_aug_params["p_rot"] = 0.3
+        self.data_aug_params["num_cached_per_thread"] = 2
 
-        self.data_aug_params["scale_range"] = (0.65, 1.6)
-        self.data_aug_params["p_scale"] = 0.3
-        self.data_aug_params["independent_scale_factor_for_each_axis"] = True
-        self.data_aug_params["p_independent_scale_per_axis"] = 0.3
+    def maybe_update_lr(self, epoch=None):
+        """
+        if epoch is not None we overwrite epoch. Else we use epoch = self.epoch + 1
+
+        (maybe_update_lr is called in on_epoch_end which is called before epoch is incremented.
+        herefore we need to do +1 here)
+
+        :param epoch:
+        :return:
+        """
+        if epoch is None:
+            ep = self.epoch + 1
+        else:
+            ep = epoch
+        self.optimizer.param_groups[0]['lr'] = poly_lr(ep, self.max_num_epochs, self.initial_lr, 0.9)
+        self.print_to_log_file("lr:", np.round(self.optimizer.param_groups[0]['lr'], decimals=6))
 
-        self.data_aug_params["do_elastic"] = True
-        self.data_aug_params["p_eldef"] = 0.2
-        self.data_aug_params["eldef_deformation_scale"] = (0, 0.25)
+    def on_epoch_end(self):
+        """
+        overwrite patient-based early stopping. Always run to 1000 epochs
+        :return:
+        """
+        super().on_epoch_end()
+        continue_training = self.epoch < self.max_num_epochs
 
-        self.data_aug_params["do_additive_brightness"] = True
-        self.data_aug_params["additive_brightness_mu"] = 0
-        self.data_aug_params["additive_brightness_sigma"] = 0.2
-        self.data_aug_params["additive_brightness_p_per_sample"] = 0.3
-        self.data_aug_params["additive_brightness_p_per_channel"] = 0.5
+        # it can rarely happen that the momentum of nnUNetTrainerV2 is too high for some dataset. If at epoch 100 the
+        # estimated validation Dice is still 0 then we reduce the momentum from 0.99 to 0.95
+        if self.epoch == 100:
+            if self.all_val_eval_metrics[-1] == 0:
+                self.optimizer.param_groups[0]["momentum"] = 0.95
+                self.network.apply(InitWeights_He(1e-2))
+                self.print_to_log_file("At epoch 100, the mean foreground Dice was 0. This can be caused by a too "
+                                       "high momentum. High momentum (0.99) is good for datasets where it works, but "
+                                       "sometimes causes issues such as this one. Momentum has now been reduced to "
+                                       "0.95 and network weights have been reinitialized")
+        return continue_training
 
-        self.data_aug_params['gamma_range'] = (0.5, 1.6)
+    def run_training(self):
+        """
+        if we run with -c then we need to set the correct lr for the first epoch, otherwise it will run the first
+        continued epoch with self.initial_lr
 
-        self.data_aug_params['num_cached_per_thread'] = 4
+        we also need to make sure deep supervision in the network is enabled for training, thus the wrapper
+        :return:
+        """
+        self.maybe_update_lr(self.epoch)  # if we dont overwrite epoch then self.epoch+1 is used which is not what we
+        # want at the start of the training
+        ds = self.network.do_ds
+        self.network.do_ds = True
+        ret = super().run_training()
+        self.network.do_ds = ds
+        return ret
 
 
-class nnUNetTrainerV2BraTSRegions_DA4_BN_BD(nnUNetTrainerV2BraTSRegions_DA4_BN):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
+# (modified by YC Yao: yao_yongcheng@link.cuhk.edu.hk)
+# added functionality: set training epoch
+class nnUNetTrainerV2(nnUNetTrainer_CMTbase):
+     def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
                  unpack_data=True, deterministic=True, fp16=False):
         super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
                          deterministic, fp16)
-        self.loss = DC_and_BCE_loss({}, {'batch_dice': True, 'do_bg': True, 'smooth': 0})
+     def set_trainingEpoch(self, epoch):
+        self.max_num_epochs = epoch
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/network_trainer.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/network_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 from _warnings import warn
 from typing import Tuple
 
 import matplotlib
 from batchgenerators.utilities.file_and_folder_operations import *
-from nnunet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
 from sklearn.model_selection import KFold
 from torch import nn
 from torch.cuda.amp import GradScaler, autocast
 from torch.optim.lr_scheduler import _LRScheduler
 
 matplotlib.use("agg")
 from time import time, sleep
@@ -32,15 +32,15 @@
 import matplotlib.pyplot as plt
 import sys
 from collections import OrderedDict
 import torch.backends.cudnn as cudnn
 from abc import abstractmethod
 from datetime import datetime
 from tqdm import trange
-from nnunet.utilities.to_torch import maybe_to_torch, to_cuda
+from CartiMorph_nnUNet.utilities.to_torch import maybe_to_torch, to_cuda
 
 
 class NetworkTrainer(object):
     def __init__(self, deterministic=True, fp16=False):
         """
         A generic class that can train almost any neural network (RNNs excluded). It provides basic functionality such
         as the training loop, tracking of training and validation losses (and the target metric if you implement it)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 import matplotlib
 import numpy as np
 import torch
 from batchgenerators.utilities.file_and_folder_operations import *
 from torch import nn
 from torch.optim import lr_scheduler
 
-import nnunet
-from nnunet.configuration import default_num_threads
-from nnunet.evaluation.evaluator import aggregate_scores
-from nnunet.inference.segmentation_export import save_segmentation_nifti_from_softmax
-from nnunet.network_architecture.generic_UNet import Generic_UNet
-from nnunet.network_architecture.initialization import InitWeights_He
-from nnunet.network_architecture.neural_network import SegmentationNetwork
-from nnunet.postprocessing.connected_components import determine_postprocessing
-from nnunet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params, \
+import CartiMorph_nnUNet
+from CartiMorph_nnUNet.training.model_restore import recursive_find_python_class
+from CartiMorph_nnUNet.configuration import default_num_threads
+from CartiMorph_nnUNet.evaluation.evaluator import aggregate_scores
+from CartiMorph_nnUNet.inference.segmentation_export import save_segmentation_nifti_from_softmax
+from CartiMorph_nnUNet.network_architecture.generic_UNet import Generic_UNet
+from CartiMorph_nnUNet.network_architecture.initialization import InitWeights_He
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.postprocessing.connected_components import determine_postprocessing
+from CartiMorph_nnUNet.training.data_augmentation.default_data_augmentation import default_3D_augmentation_params, \
     default_2D_augmentation_params, get_default_augmentation, get_patch_size
-from nnunet.training.dataloading.dataset_loading import load_dataset, DataLoader3D, DataLoader2D, unpack_dataset
-from nnunet.training.loss_functions.dice_loss import DC_and_CE_loss
-from nnunet.training.network_training.network_trainer import NetworkTrainer
-from nnunet.utilities.nd_softmax import softmax_helper
-from nnunet.utilities.tensor_utilities import sum_tensor
+from CartiMorph_nnUNet.training.dataloading.dataset_loading import load_dataset, DataLoader3D, DataLoader2D, unpack_dataset
+from CartiMorph_nnUNet.training.loss_functions.dice_loss import DC_and_CE_loss
+from CartiMorph_nnUNet.training.network_training.network_trainer import NetworkTrainer
+from CartiMorph_nnUNet.utilities.nd_softmax import softmax_helper
+from CartiMorph_nnUNet.utilities.tensor_utilities import sum_tensor
 
 matplotlib.use("agg")
 
 
 class nnUNetTrainer(NetworkTrainer):
     def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
                  unpack_data=True, deterministic=True, fp16=False):
@@ -417,27 +418,27 @@
 
     def preprocess_patient(self, input_files):
         """
         Used to predict new unseen data. Not used for the preprocessing of the training/test data
         :param input_files:
         :return:
         """
-        from nnunet.training.model_restore import recursive_find_python_class
+        
         preprocessor_name = self.plans.get('preprocessor_name')
         if preprocessor_name is None:
             if self.threeD:
                 preprocessor_name = "GenericPreprocessor"
             else:
                 preprocessor_name = "PreprocessorFor2D"
 
         print("using preprocessor", preprocessor_name)
-        preprocessor_class = recursive_find_python_class([join(nnunet.__path__[0], "preprocessing")],
+        preprocessor_class = recursive_find_python_class([join(CartiMorph_nnUNet.__path__[0], "preprocessing")],
                                                          preprocessor_name,
-                                                         current_module="nnunet.preprocessing")
-        assert preprocessor_class is not None, "Could not find preprocessor %s in nnunet.preprocessing" % \
+                                                         current_module="CartiMorph_nnUNet.preprocessing")
+        assert preprocessor_class is not None, "Could not find preprocessor %s in CartiMorph_nnUNet.preprocessing" % \
                                                preprocessor_name
         preprocessor = preprocessor_class(self.normalization_schemes, self.use_mask_for_norm,
                                           self.transpose_forward, self.intensity_properties)
 
         d, s, properties = preprocessor.preprocess_test_case(input_files,
                                                              self.plans['plans_per_stage'][self.stage][
                                                                  'current_spacing'])
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/network_training/nnUNetTrainerCascadeFullRes.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 #    limitations under the License.
 
 
 from multiprocessing.pool import Pool
 from time import sleep
 
 import matplotlib
-from nnunet.postprocessing.connected_components import determine_postprocessing
-from nnunet.training.data_augmentation.default_data_augmentation import get_default_augmentation
-from nnunet.training.dataloading.dataset_loading import DataLoader3D, unpack_dataset
-from nnunet.evaluation.evaluator import aggregate_scores
-from nnunet.training.network_training.nnUNetTrainer import nnUNetTrainer
-from nnunet.network_architecture.neural_network import SegmentationNetwork
-from nnunet.paths import network_training_output_dir
-from nnunet.inference.segmentation_export import save_segmentation_nifti_from_softmax
+from CartiMorph_nnUNet.postprocessing.connected_components import determine_postprocessing
+from CartiMorph_nnUNet.training.data_augmentation.default_data_augmentation import get_default_augmentation
+from CartiMorph_nnUNet.training.dataloading.dataset_loading import DataLoader3D, unpack_dataset
+from CartiMorph_nnUNet.evaluation.evaluator import aggregate_scores
+from CartiMorph_nnUNet.training.network_training.nnUNetTrainer import nnUNetTrainer
+from CartiMorph_nnUNet.network_architecture.neural_network import SegmentationNetwork
+from CartiMorph_nnUNet.paths import network_training_output_dir
+from CartiMorph_nnUNet.inference.segmentation_export import save_segmentation_nifti_from_softmax
 from batchgenerators.utilities.file_and_folder_operations import *
 import numpy as np
-from nnunet.utilities.one_hot_encoding import to_one_hot
+from CartiMorph_nnUNet.utilities.one_hot_encoding import to_one_hot
 import shutil
 
 matplotlib.use("agg")
 
 
 class nnUNetTrainerCascadeFullRes(nnUNetTrainer):
     def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_DA2.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/random_stuff.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,23 +9,13 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
-
-
-class nnUNetTrainerV2_DA2(nnUNetTrainerV2):
-    def setup_DA_params(self):
-        super().setup_DA_params()
-
-        self.data_aug_params["independent_scale_factor_for_each_axis"] = True
-
-        if self.threeD:
-            self.data_aug_params["rotation_p_per_axis"] = 0.5
-        else:
-            self.data_aug_params["rotation_p_per_axis"] = 1
-
-        self.data_aug_params["do_additive_brightness"] = True
+class no_op(object):
+    def __enter__(self):
+        pass
 
+    def __exit__(self, *args):
+        pass
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/data_augmentation/nnUNetTrainerV2_independentScalePerAxis.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/sitk_stuff.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
+import SimpleITK as sitk
 
 
-class nnUNetTrainerV2_independentScalePerAxis(nnUNetTrainerV2):
-    def setup_DA_params(self):
-        super().setup_DA_params()
-        self.data_aug_params["independent_scale_factor_for_each_axis"] = True
+def copy_geometry(image: sitk.Image, ref: sitk.Image):
+    image.SetOrigin(ref.GetOrigin())
+    image.SetDirection(ref.GetDirection())
+    image.SetSpacing(ref.GetSpacing())
+    return image
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_CE.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/recursive_delete_npz.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,31 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
-from nnunet.training.loss_functions.crossentropy import RobustCrossEntropyLoss
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
 
 
-class nnUNetTrainerV2_Loss_CE(nnUNetTrainerV2):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.loss = RobustCrossEntropyLoss()
+from batchgenerators.utilities.file_and_folder_operations import *
+import argparse
+import os
+
+
+def recursive_delete_npz(current_directory: str):
+    npz_files = subfiles(current_directory, join=True, suffix=".npz")
+    npz_files = [i for i in npz_files if not i.endswith("segFromPrevStage.npz")] # to be extra safe
+    _ = [os.remove(i) for i in npz_files]
+    for d in subdirs(current_directory, join=False):
+        if d != "pred_next_stage":
+            recursive_delete_npz(join(current_directory, d))
+
+
+if __name__ == "__main__":
+    parser = argparse.ArgumentParser(usage="USE THIS RESPONSIBLY! DANGEROUS! I (Fabian) use this to remove npz files "
+                                           "after I ran figure_out_what_to_submit")
+    parser.add_argument("-f", help="folder", required=True)
+
+    args = parser.parse_args()
+
+    recursive_delete_npz(args.f)
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/network_training/nnUNet_variants/loss_function/nnUNetTrainerV2_Loss_DiceCE_noSmooth.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/file_endings.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-from nnunet.training.network_training.nnUNetTrainerV2 import nnUNetTrainerV2
-from nnunet.training.loss_functions.dice_loss import SoftDiceLoss, DC_and_CE_loss
+from batchgenerators.utilities.file_and_folder_operations import *
 
 
-class nnUNetTrainerV2_Loss_DiceCE_noSmooth(nnUNetTrainerV2):
-    def __init__(self, plans_file, fold, output_folder=None, dataset_directory=None, batch_dice=True, stage=None,
-                 unpack_data=True, deterministic=True, fp16=False):
-        super().__init__(plans_file, fold, output_folder, dataset_directory, batch_dice, stage, unpack_data,
-                         deterministic, fp16)
-        self.loss = DC_and_CE_loss({'batch_dice': self.batch_dice, 'smooth': 0, 'do_bg': False}, {})
+def remove_trailing_slash(filename: str):
+    while filename.endswith('/'):
+        filename = filename[:-1]
+    return filename
 
 
+def maybe_add_0000_to_all_niigz(folder):
+    nii_gz = subfiles(folder, suffix='.nii.gz')
+    for n in nii_gz:
+        n = remove_trailing_slash(n)
+        if not n.endswith('_0000.nii.gz'):
+            os.rename(n, n[:-7] + '_0000.nii.gz')
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/training/optimizer/ranger.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/training/optimizer/ranger.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/distributed.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/distributed.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/file_conversions.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/file_conversions.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/folder_names.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/folder_names.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/image_reorientation.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/image_reorientation.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/nd_softmax.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/nd_softmax.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/one_hot_encoding.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/to_torch.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,24 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
-import numpy as np
+import torch
 
 
-def to_one_hot(seg, all_seg_labels=None):
-    if all_seg_labels is None:
-        all_seg_labels = np.unique(seg)
-    result = np.zeros((len(all_seg_labels), *seg.shape), dtype=seg.dtype)
-    for i, l in enumerate(all_seg_labels):
-        result[i][seg == l] = 1
-    return result
+def maybe_to_torch(d):
+    if isinstance(d, list):
+        d = [maybe_to_torch(i) if not isinstance(i, torch.Tensor) else i for i in d]
+    elif not isinstance(d, torch.Tensor):
+        d = torch.from_numpy(d).float()
+    return d
+
+
+def to_cuda(data, non_blocking=True, gpu_id=0):
+    if isinstance(data, list):
+        data = [i.cuda(gpu_id, non_blocking=non_blocking) for i in data]
+    else:
+        data = data.cuda(gpu_id, non_blocking=non_blocking)
+    return data
```

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/recursive_rename_taskXX_to_taskXXX.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/set_n_proc_DA.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/set_n_proc_DA.py`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/CartiMorph_nnUNet/utilities/task_name_id_conversion.py` & `CartiMorph_nnUNet-1.7.4/CartiMorph_nnUNet/utilities/task_name_id_conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 
-from nnunet.paths import nnUNet_raw_data, preprocessing_output_dir, nnUNet_cropped_data, network_training_output_dir
+from CartiMorph_nnUNet.paths import nnUNet_raw_data, preprocessing_output_dir, nnUNet_cropped_data, network_training_output_dir
 from batchgenerators.utilities.file_and_folder_operations import *
 import numpy as np
 
 
 def convert_id_to_task_name(task_id: int):
     startswith = "Task%03.0d" % task_id
     if preprocessing_output_dir is not None:
```

### Comparing `CartiMorph_nnUNet-1.7.3/LICENSE` & `CartiMorph_nnUNet-1.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CartiMorph_nnUNet-1.7.3/README.md` & `CartiMorph_nnUNet-1.7.4/README.md`

 * *Files identical despite different names*

