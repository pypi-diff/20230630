# Comparing `tmp/adversarial-robustness-toolbox-1.9.0.tar.gz` & `tmp/adversarial-robustness-toolbox-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adversarial-robustness-toolbox-1.9.0.tar", last modified: Sat Dec 18 22:27:25 2021, max compression
+gzip compressed data, was "dist/adversarial-robustness-toolbox-1.9.1.tar", last modified: Fri Jan  7 13:28:20 2022, max compression
```

## Comparing `adversarial-robustness-toolbox-1.9.0.tar` & `adversarial-robustness-toolbox-1.9.1.tar`

### file list

```diff
@@ -1,658 +1,658 @@
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      513 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/AUTHORS
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      702 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1170 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/CONTRIBUTING.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1105 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/LICENSE
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3238 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/MAINTAINERS.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      141 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/MANIFEST.in
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6949 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/PKG-INFO
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1159 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5274 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/README-cn.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5516 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/README.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2278 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/SECURITY.md
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6949 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25599 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        1 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1210 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/requires.txt
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       10 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/top_level.txt
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1016 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      498 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18617 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/attack.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3896 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3923 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_asr.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11476 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26388 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25815 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23179 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3203 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/utils.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_texture/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_texture/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19230 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_texture/adversarial_texture_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11317 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/auto_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    28413 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/auto_projected_gradient_descent.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19035 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/boundary.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    95832 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/brendel_bethge.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    60935 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/carlini.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7899 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/decision_tree_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10402 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/deepfool.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16589 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/dpatch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21398 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/dpatch_robust.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17427 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/elastic_net.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26077 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/fast_gradient.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9230 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10306 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10452 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10926 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/frame_saliency.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17770 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/geometric_decision_based_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6090 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/hclu.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26757 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/hop_skip_jump.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    40067 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/imperceptible_asr.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39984 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/imperceptible_asr_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3189 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/iterative_method.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3351 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/algorithms.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15235 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/laser_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9917 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18423 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/lowprofool.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7597 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/newtonfool.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/over_the_air_flickering/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/over_the_air_flickering/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15034 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/over_the_air_flickering/over_the_air_flickering_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39578 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/pe_malware_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    63022 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/pixel_threshold.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11936 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19674 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    22255 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21537 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_tensorflow_v2.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10091 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/saliency_map.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12263 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/shadow_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    49236 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/shapeshifter.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20440 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/simba.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9950 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/spatial_transformation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23453 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/square_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8623 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/targeted_universal_perturbation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10957 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/universal_perturbation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9675 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/virtual_adversarial.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    31264 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/wasserstein.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    28684 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/zoo.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      293 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6972 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/copycat_cnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20702 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/functionally_equivalent_extraction.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16566 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/knockoff_nets.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      252 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      703 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6978 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/baseline.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9425 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/black_box.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8087 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/meminf_based.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7776 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/true_label_baseline.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6874 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/white_box_decision_tree.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6204 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/white_box_lifestyle_decision_tree.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      549 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17848 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/black_box.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4574 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/black_box_rule_based.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12676 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/label_only_boundary_distance.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1471 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/label_only_gap_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16872 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/shadow_models.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/model_inversion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      115 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/model_inversion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6999 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/model_inversion/mi_face.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/reconstruction/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      132 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/reconstruction/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4081 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/inference/reconstruction/white_box.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      583 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14844 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/adversarial_embedding_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3737 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/backdoor_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16208 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/bullseye_polytope_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6616 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/clean_label_backdoor_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13226 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/feature_collision_attack.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/perturbations/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      202 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/perturbations/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7121 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/perturbations/image_perturbations.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10646 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/poisoning_attack_svm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3852 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/config.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13047 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/data_generators.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      265 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      164 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      232 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16409 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/detector.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      323 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13185 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/detector.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9140 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scanner.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8788 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scanningops.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4055 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scoring_functions.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      640 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34719 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/activation_defence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17888 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/clustering_analyzer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7856 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/ground_truth_evaluator.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3829 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/poison_filtering_defence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10689 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/provenance_defense.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8549 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/roni.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8032 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/spectral_signature_defense.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      475 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2383 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/class_labels.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3214 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/gaussian_noise.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2574 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/high_confidence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3786 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/postprocessor.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4269 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/reverse_sigmoid.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2526 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/rounded.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1352 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4388 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/feature_squeezing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6201 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/gaussian_augmentation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7366 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/inverse_gan.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8014 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/jpeg_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3993 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/label_smoothing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6420 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/mp3_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5009 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/mp3_compression_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6805 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/pixel_defend.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12375 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/preprocessor.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3815 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/resample.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5361 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9533 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5368 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7295 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/thermometer_encoding.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9900 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/variance_minimization.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5925 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/video_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5530 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/video_compression_pytorch.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      462 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13436 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4382 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_fbf.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11029 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_fbf_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4857 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_madry_pgd.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2324 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/trainer/trainer.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      238 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/evasion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      170 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/evasion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4568 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/evasion/defensive_distillation.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      217 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5809 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/neural_cleanse.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3367 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/strip.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3504 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/defences/transformer/transformer.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      797 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      114 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1936 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/abstain.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      445 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7418 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11348 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9725 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/randomized_smoothing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12569 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10097 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/GPy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1370 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17266 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/blackbox.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6865 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/catboost.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7711 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/classifier.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10027 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/deep_partition_ensemble.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17624 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/detector_classifier.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16456 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/ensemble.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    38090 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/keras.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8540 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/lightgbm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23337 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/mxnet.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    43547 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8940 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/query_efficient_bb.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    61364 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/scikitlearn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    59538 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10827 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/classification/xgboost.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      144 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1614 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/encoder.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7997 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21642 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/estimator.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/generation/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      156 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/generation/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1619 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/generation/generator.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7927 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/generation/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3707 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/keras.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3083 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/mxnet.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      399 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1840 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/object_detector.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19607 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/python_object_detector.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5079 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/pytorch_faster_rcnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    27085 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/tensorflow_faster_rcnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4117 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/utils.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      208 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1835 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/object_tracker.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34539 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/pytorch_goturn.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      338 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      214 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19309 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/keras.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14619 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/neural_cleanse.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/strip/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       94 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/strip/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5701 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/strip/strip.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14494 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/pytorch.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/regression/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      189 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/regression/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1335 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/regression/regressor.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12457 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/regression/scikitlearn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2477 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/scikitlearn.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      395 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39049 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/pytorch_deep_speech.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26028 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/pytorch_espresso.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2805 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/speech_recognizer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25203 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/tensorflow_lingvo.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12885 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/estimators/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1544 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/evaluation.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/security_curve/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      138 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/security_curve/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7925 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/evaluations/security_curve/security_curve.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2713 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/exceptions.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      118 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/classification/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      107 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/classification/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12118 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/classification/jax.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4409 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/jax.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      522 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2763 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/gradient_check.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16346 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/metrics.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/privacy/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      108 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/privacy/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5956 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/privacy/membership_leakage.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17652 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/metrics/verification_decisions_trees.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3061 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/optimizers.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      316 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      183 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9178 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7599 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/pytorch.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1485 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/image_rotation/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/image_rotation/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4942 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/image_rotation/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4025 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4081 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4778 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4826 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4044 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4099 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4113 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4214 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4775 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4833 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4656 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4631 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1502 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/preprocessing.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      370 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4530 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/numpy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3786 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3632 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2275 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13573 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/summary_writer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    52420 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6466 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/art/visualization.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      627 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/Makefile
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5540 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/conf.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/guide/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      202 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/guide/examples.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      232 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/guide/notebooks.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      197 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/guide/setup.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/images/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17845 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/adversarial_threats_art.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   117720 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/adversarial_threats_attacker.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   265489 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/art_architecture.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    46317 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/art_lfai.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4748 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/art_logo.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   983947 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/art_logo_3d_1.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   173317 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/summary_writer_patch.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   280253 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/summary_writer_scalar.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   228467 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/images/white_hat_blue_red.png
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3892 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/index.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      834 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/make.bat
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6360 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/evasion.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      428 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/extraction.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      952 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/attribute_inference.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      809 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/membership_inference.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      247 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/model_inversion.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      262 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/reconstruction.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      873 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/poisoning.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      827 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/attacks.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      477 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/data_generators.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      321 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/detector_evasion.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      267 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/detector_evasion_subsetscanning.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      602 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/detector_poisoning.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      675 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/postprocessor.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1783 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/preprocessor.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      816 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/trainer.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      247 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/transformer_evasion.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      306 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences/transformer_poisoning.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       69 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/defences.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      117 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/certification.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      705 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/certification_randomized_smoothing.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2202 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/classification.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2046 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/classification_scikitlearn.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      333 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/encoding.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      350 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/generation.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      799 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/object_detection.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      445 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/object_tracking.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      433 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/poison_mitigation.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      259 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/regression.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      431 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/regression_scikitlearn.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      844 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/speech_recognition.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1442 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/estimators.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       78 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/evaluations.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      141 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/exceptions.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      644 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/metrics.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      279 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/audio.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1621 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/expectation_over_transformation.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      621 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/standardisation_mean_std.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       84 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/tests/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1451 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/tests/utils.rst
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1087 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/docs/modules/utils.rst
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/examples/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3112 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/README.md
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7997 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_FBF.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3465 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_cifar10.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3912 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_data_augmentation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5436 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/application_object_detection.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8407 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_fasterrcnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5454 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_inverse_gan.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2501 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_keras.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2493 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_lightgbm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2625 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_mxnet.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2966 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8448 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_pytorch_goturn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1920 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_scikit_learn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2585 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3316 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_tensorflow_v2.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2493 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/get_started_xgboost.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    69938 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/inverse_gan_author_utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2907 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/mnist_cnn_features_level_fgsm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1970 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/mnist_cnn_fgsm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8492 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/mnist_poison_detection.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3009 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/examples/mnist_transferability.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       29 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/pyproject.toml
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      756 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/setup.cfg
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4040 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/setup.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1942 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/conftest.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4030 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/conftest.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3792 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5839 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5928 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3637 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_adversarial_asr.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7767 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_adversarial_texture_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7109 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_auto_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5664 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_auto_projected_gradient_descent.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5059 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_boundary.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4818 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_brendel_and_bethge.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7442 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_dpatch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11164 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_dpatch_robust.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11000 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_fast_gradient.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6335 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_frame_saliency.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8108 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_geometric_decision_based_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19312 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4968 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr_pytorch.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10140 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9038 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_laser_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19887 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_lowprofool.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6575 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_over_the_air.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    24259 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_pe_malware_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6494 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_shadow_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4431 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_square_attack.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5112 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_baseline.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18887 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_black_box.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20841 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_meminf_based.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5028 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_true_label_baseline.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3754 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_white_box_decision_tree.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6330 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_white_box_lifestyle_decision_tree.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11855 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_black_box.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4352 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_black_box_rule_based.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6377 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_label_only_boundary_distance.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3265 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_label_only_gap_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6962 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_shadow_models.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/model_inversion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/model_inversion/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5014 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/model_inversion/test_mi_face.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3457 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/test_reconstruction.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6097 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_bullseye_polytope_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2809 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_clean_label_backdoor_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2973 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_image_perturbations.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5938 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_adversarial_embedding.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15184 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_adversarial_patch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7956 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_backdoor_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    47152 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_carlini.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15702 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_copycat_cnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3482 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_decision_tree_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13393 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_deepfool.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    29897 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_elastic_net.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4708 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_feature_collision.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    33834 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_functionally_equivalent_extraction.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4953 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_hclu.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    37911 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_hop_skip_jump.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12146 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_input_filter.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17646 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_iterative_method.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16537 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_knockoff_nets.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10217 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_newtonfool.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6582 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_pixel_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9643 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_poisoning_attack_svm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34039 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_projected_gradient_descent.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14748 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_saliency_map.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16985 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_shapeshifter.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8968 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_simba.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7296 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_spatial_transformation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7269 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_targeted_universal_perturbation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5841 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_threshold_attack.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10777 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_universal_perturbation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10660 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_virtual_adversarial.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20470 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_wasserstein.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11361 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/test_zoo.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9072 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/attacks/utils.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/classifiersFrameworks/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11579 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/classifiersFrameworks/test_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12131 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/classifiersFrameworks/test_tensorflow.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/subsetscanning/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/subsetscanning/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3039 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/subsetscanning/test_detector.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7449 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/test_detector.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12920 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_activation_defence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11930 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_clustering_analyzer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10740 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_ground_truth_evaluator.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7973 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_provenance_defence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6995 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_roni.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3646 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_spectral_signature_defense.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2204 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/conftest.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2804 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_inverse_gan.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5881 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_jpeg_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4758 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_mp3_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4700 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_mp3_compression_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1031 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_preprocessor.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3367 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_resample.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4462 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6042 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6445 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing_tensorflow.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3596 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_video_compression.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4689 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_video_compression_pytorch.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9188 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_adversarial_trainer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3040 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_adversarial_trainer_madry_pgd.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3668 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_class_labels.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9847 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_defensive_distillation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3400 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_feature_squeezing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4292 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_gaussian_augmentation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4281 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_gaussian_noise.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5765 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_high_confidence.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2490 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_label_smoothing.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4491 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_neural_cleanse.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5056 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_pixel_defend.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8878 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_reverse_sigmoid.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2930 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_rounded.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5697 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_thermometer_encoding.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3633 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/test_variance_minimization.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/trainer/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/trainer/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4545 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/trainer/test_adversarial_trainer_FBF.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/poisoning/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/poisoning/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2261 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/poisoning/test_strip.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/certification/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/certification/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11748 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/certification/test_randomized_smoothing.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4243 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_GPy.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6173 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_blackbox.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3124 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_blackbox_existing_predictions.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2367 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_catboost.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5292 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_classifier.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10568 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deep_partition_ensemble.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    70785 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_common.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20799 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_common.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2934 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_specific.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8929 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_specific.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6701 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_detector_classifier.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9006 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_ensemble.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12280 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_input_filter.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2088 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_jax.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5232 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_jax.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2349 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_lightgbm.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5964 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_query_efficient_bb.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25143 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_scikitlearn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3920 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_xgboost.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12060 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_pytorch_faster_rcnn.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14679 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_pytorch_object_detector.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11526 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_tensorflow_faster_rcnn.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_tracking/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_tracking/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3638 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/object_tracking/test_pytorch_goturn.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/regression/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2665 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/regression/test_scikitlearn.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2052 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/conftest.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    27926 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_deep_speech.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5212 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_deep_speech.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4484 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_espresso.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5302 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_espresso.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13525 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_tensorflow_lingvo.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/evaluations/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/evaluations/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3308 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/evaluations/test_security_curve.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/privacy/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/privacy/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4816 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/privacy/test_membership_leakage.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2968 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/test_gradient_check.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16000 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/test_metrics.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6184 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/metrics/test_verification_decision_trees.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19262 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7538 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7187 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter_pytorch.json
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6734 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter_pytorch.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/__init__.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/__init__.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4715 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_brightness.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5922 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_contrast.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3209 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_gaussian_noise.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3177 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_shot_noise.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5740 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_zoom_blur.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3180 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/test_image_rotation.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3757 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/preprocessing/test_standardisation_mean_std.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15422 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/test_data_generators.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1773 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/test_optimizers.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4654 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/test_summary_writer.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19134 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/test_utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4588 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/test_visualization.py
-drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2021-12-18 22:27:25.000000 adversarial-robustness-toolbox-1.9.0/tests/utils/
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5345 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/utils/test_utils.py
--rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    62459 2021-12-18 22:25:26.000000 adversarial-robustness-toolbox-1.9.0/tests/utils.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      513 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/AUTHORS
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      702 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1170 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/CONTRIBUTING.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1105 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/LICENSE
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3238 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/MAINTAINERS.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      141 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/MANIFEST.in
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6949 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/PKG-INFO
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1159 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5274 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/README-cn.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5516 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/README.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2278 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/SECURITY.md
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6949 2022-01-07 13:28:19.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25599 2022-01-07 13:28:19.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        1 2022-01-07 13:28:19.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1210 2022-01-07 13:28:19.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       10 2022-01-07 13:28:19.000000 adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/top_level.txt
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1016 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      498 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18617 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/attack.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3896 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3923 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_asr.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11476 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26388 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25815 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23179 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3203 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/utils.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_texture/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_texture/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19230 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_texture/adversarial_texture_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11317 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/auto_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    28413 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/auto_projected_gradient_descent.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19035 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/boundary.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    95832 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/brendel_bethge.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    60935 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/carlini.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7899 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/decision_tree_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10402 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/deepfool.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16589 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/dpatch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21398 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/dpatch_robust.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17427 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/elastic_net.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26077 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/fast_gradient.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9230 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10306 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10452 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10926 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/frame_saliency.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17770 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/geometric_decision_based_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6090 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/hclu.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26757 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/hop_skip_jump.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    40067 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/imperceptible_asr.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39984 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/imperceptible_asr_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3189 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/iterative_method.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3351 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/algorithms.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15235 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/laser_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9922 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18423 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/lowprofool.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7597 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/newtonfool.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/over_the_air_flickering/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/over_the_air_flickering/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15034 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/over_the_air_flickering/over_the_air_flickering_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39578 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/pe_malware_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    63022 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/pixel_threshold.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11936 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19674 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    22255 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21537 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_tensorflow_v2.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10091 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/saliency_map.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12263 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/shadow_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    49236 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/shapeshifter.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20440 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/simba.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9950 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/spatial_transformation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23453 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/square_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8623 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/targeted_universal_perturbation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10957 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/universal_perturbation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9675 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/virtual_adversarial.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    31264 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/wasserstein.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    28684 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/zoo.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      293 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6972 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/copycat_cnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20702 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/functionally_equivalent_extraction.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16566 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/knockoff_nets.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      252 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      703 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6978 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/baseline.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9425 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/black_box.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8087 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/meminf_based.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7776 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/true_label_baseline.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6874 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/white_box_decision_tree.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6204 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/white_box_lifestyle_decision_tree.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      549 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17848 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/black_box.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4574 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/black_box_rule_based.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12676 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/label_only_boundary_distance.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1471 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/label_only_gap_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16872 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/shadow_models.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/model_inversion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      115 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/model_inversion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6999 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/model_inversion/mi_face.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/reconstruction/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      132 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/reconstruction/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4081 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/inference/reconstruction/white_box.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      583 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14844 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/adversarial_embedding_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3737 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/backdoor_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16208 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/bullseye_polytope_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6616 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/clean_label_backdoor_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13226 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/feature_collision_attack.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/perturbations/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      202 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/perturbations/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7121 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/perturbations/image_perturbations.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10646 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/poisoning_attack_svm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3852 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/config.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13047 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/data_generators.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      265 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      164 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      232 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16409 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/detector.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      323 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13185 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/detector.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9140 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scanner.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8788 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scanningops.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4055 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scoring_functions.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      640 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34719 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/activation_defence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17888 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/clustering_analyzer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7856 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/ground_truth_evaluator.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3829 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/poison_filtering_defence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10689 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/provenance_defense.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8549 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/roni.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8032 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/spectral_signature_defense.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      475 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2383 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/class_labels.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3214 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/gaussian_noise.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2574 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/high_confidence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3786 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/postprocessor.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4269 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/reverse_sigmoid.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2526 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/rounded.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1352 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4388 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/feature_squeezing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6201 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/gaussian_augmentation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7366 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/inverse_gan.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8014 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/jpeg_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3993 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/label_smoothing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6420 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/mp3_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5009 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/mp3_compression_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6805 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/pixel_defend.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12375 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/preprocessor.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3815 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/resample.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5361 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9533 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5368 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7295 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/thermometer_encoding.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9900 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/variance_minimization.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6331 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/video_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5708 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/video_compression_pytorch.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      462 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13436 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4382 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_fbf.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11029 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_fbf_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4857 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_madry_pgd.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2324 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/trainer/trainer.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      238 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/evasion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      170 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/evasion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4568 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/evasion/defensive_distillation.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      217 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5809 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/neural_cleanse.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3367 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/strip.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3504 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/defences/transformer/transformer.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      797 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      114 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1936 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/abstain.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      445 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7418 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11348 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9725 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/randomized_smoothing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12569 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10097 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/GPy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1370 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17266 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/blackbox.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6865 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/catboost.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7711 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/classifier.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10027 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/deep_partition_ensemble.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17624 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/detector_classifier.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16456 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/ensemble.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    38204 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/keras.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8540 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/lightgbm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    23337 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/mxnet.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    43694 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8940 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/query_efficient_bb.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    61364 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/scikitlearn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    59538 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10827 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/classification/xgboost.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      144 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1614 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/encoder.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7997 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    21642 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/estimator.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/generation/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      156 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/generation/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1619 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/generation/generator.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7927 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/generation/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3707 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/keras.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3083 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/mxnet.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      399 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1840 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/object_detector.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19607 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/python_object_detector.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5079 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/pytorch_faster_rcnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    27085 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/tensorflow_faster_rcnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4117 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/utils.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      208 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1835 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/object_tracker.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34621 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/pytorch_goturn.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      338 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      214 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19309 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/keras.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14619 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/neural_cleanse.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/strip/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       94 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/strip/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5701 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/strip/strip.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14494 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/pytorch.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/regression/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      189 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/regression/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1335 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/regression/regressor.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12457 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/regression/scikitlearn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2477 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/scikitlearn.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      395 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    39049 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/pytorch_deep_speech.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    26028 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/pytorch_espresso.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2805 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/speech_recognizer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25203 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/tensorflow_lingvo.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12885 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/estimators/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1544 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/evaluation.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/security_curve/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      138 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/security_curve/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7925 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/evaluations/security_curve/security_curve.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2713 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/exceptions.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      118 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/classification/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      107 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/classification/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12118 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/classification/jax.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4409 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/jax.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      522 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2763 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/gradient_check.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16346 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/metrics.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/privacy/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      108 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/privacy/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5956 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/privacy/membership_leakage.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17652 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/metrics/verification_decisions_trees.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3061 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/optimizers.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      316 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      183 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9178 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7599 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/pytorch.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1485 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/image_rotation/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/image_rotation/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4942 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/image_rotation/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4025 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4081 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4778 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4826 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4044 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4099 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4113 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4214 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4775 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4833 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4656 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4631 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1502 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/preprocessing.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      370 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4530 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/numpy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3786 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3632 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2275 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13573 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/summary_writer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    52948 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6466 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/art/visualization.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      627 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/Makefile
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5540 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/conf.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/guide/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      202 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/guide/examples.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      232 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/guide/notebooks.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      197 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/guide/setup.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/images/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17845 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/adversarial_threats_art.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   117720 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/adversarial_threats_attacker.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   265489 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/art_architecture.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    46317 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/art_lfai.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4748 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/art_logo.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   983947 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/art_logo_3d_1.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   173317 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/summary_writer_patch.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   280253 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/summary_writer_scalar.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)   228467 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/images/white_hat_blue_red.png
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3892 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/index.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      834 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/make.bat
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6360 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/evasion.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      428 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/extraction.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      952 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/attribute_inference.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      809 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/membership_inference.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      247 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/model_inversion.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      262 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/reconstruction.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      873 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/poisoning.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      827 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/attacks.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      477 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/data_generators.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      321 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/detector_evasion.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      267 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/detector_evasion_subsetscanning.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      602 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/detector_poisoning.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      675 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/postprocessor.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1783 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/preprocessor.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      816 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/trainer.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      247 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/transformer_evasion.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      306 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences/transformer_poisoning.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       69 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/defences.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      117 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/certification.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      705 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/certification_randomized_smoothing.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2202 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/classification.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2046 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/classification_scikitlearn.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      333 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/encoding.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      350 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/generation.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      799 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/object_detection.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      445 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/object_tracking.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      433 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/poison_mitigation.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      259 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/regression.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      431 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/regression_scikitlearn.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      844 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/speech_recognition.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1442 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/estimators.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       78 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/evaluations.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      141 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/exceptions.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      644 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/metrics.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      279 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/audio.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1621 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/expectation_over_transformation.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      621 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/standardisation_mean_std.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       84 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/tests/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1451 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/tests/utils.rst
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1087 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/docs/modules/utils.rst
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/examples/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3112 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/README.md
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7997 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_FBF.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3465 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_cifar10.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3912 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_data_augmentation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5436 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/application_object_detection.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8407 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_fasterrcnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5454 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_inverse_gan.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2501 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_keras.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2493 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_lightgbm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2625 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_mxnet.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2966 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8448 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_pytorch_goturn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1920 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_scikit_learn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2585 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3316 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_tensorflow_v2.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2493 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/get_started_xgboost.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    69938 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/inverse_gan_author_utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2907 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/mnist_cnn_features_level_fgsm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1970 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/mnist_cnn_fgsm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8492 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/mnist_poison_detection.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3009 2022-01-07 13:27:53.000000 adversarial-robustness-toolbox-1.9.1/examples/mnist_transferability.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)       29 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/pyproject.toml
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)      756 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/setup.cfg
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4040 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/setup.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1942 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/conftest.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4030 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/conftest.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3792 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5839 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5928 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3637 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_adversarial_asr.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7767 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_adversarial_texture_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7109 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_auto_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5664 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_auto_projected_gradient_descent.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5059 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_boundary.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4818 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_brendel_and_bethge.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7442 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_dpatch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11164 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_dpatch_robust.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11000 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_fast_gradient.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6335 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_frame_saliency.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8108 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_geometric_decision_based_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19312 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4968 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr_pytorch.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10140 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9038 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_laser_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19887 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_lowprofool.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6575 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_over_the_air.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    24259 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_pe_malware_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6494 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_shadow_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4431 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_square_attack.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5112 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_baseline.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    18887 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_black_box.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20841 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_meminf_based.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5028 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_true_label_baseline.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3754 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_white_box_decision_tree.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6330 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_white_box_lifestyle_decision_tree.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11855 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_black_box.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4352 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_black_box_rule_based.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6377 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_label_only_boundary_distance.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3265 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_label_only_gap_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6962 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_shadow_models.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/model_inversion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/model_inversion/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5014 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/model_inversion/test_mi_face.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3457 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/test_reconstruction.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6097 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_bullseye_polytope_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2809 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_clean_label_backdoor_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2973 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_image_perturbations.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5938 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_adversarial_embedding.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15184 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_adversarial_patch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7956 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_backdoor_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    47152 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_carlini.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15702 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_copycat_cnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3482 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_decision_tree_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13393 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_deepfool.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    29897 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_elastic_net.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4708 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_feature_collision.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    33834 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_functionally_equivalent_extraction.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4953 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_hclu.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    37911 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_hop_skip_jump.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12146 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_input_filter.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    17646 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_iterative_method.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16537 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_knockoff_nets.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10217 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_newtonfool.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6582 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_pixel_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9643 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_poisoning_attack_svm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    34039 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_projected_gradient_descent.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14748 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_saliency_map.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16985 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_shapeshifter.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8968 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_simba.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7296 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_spatial_transformation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7269 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_targeted_universal_perturbation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5841 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_threshold_attack.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10777 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_universal_perturbation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10660 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_virtual_adversarial.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20470 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_wasserstein.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11361 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/test_zoo.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9072 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/attacks/utils.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/classifiersFrameworks/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11579 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/classifiersFrameworks/test_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12131 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/classifiersFrameworks/test_tensorflow.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/subsetscanning/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/subsetscanning/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3039 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/subsetscanning/test_detector.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7449 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/test_detector.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12920 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_activation_defence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11930 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_clustering_analyzer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10740 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_ground_truth_evaluator.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7973 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_provenance_defence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6995 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_roni.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3646 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_spectral_signature_defense.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2204 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/conftest.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2804 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_inverse_gan.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5881 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_jpeg_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4758 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_mp3_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4700 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_mp3_compression_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1031 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_preprocessor.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3367 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_resample.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4462 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6042 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6445 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing_tensorflow.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3596 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_video_compression.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4689 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_video_compression_pytorch.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9188 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_adversarial_trainer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3040 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_adversarial_trainer_madry_pgd.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3668 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_class_labels.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9847 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_defensive_distillation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3400 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_feature_squeezing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4292 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_gaussian_augmentation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4281 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_gaussian_noise.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5765 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_high_confidence.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2490 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_label_smoothing.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4491 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_neural_cleanse.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5056 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_pixel_defend.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8878 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_reverse_sigmoid.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2930 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_rounded.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5697 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_thermometer_encoding.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3633 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/test_variance_minimization.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/trainer/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/trainer/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4545 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/trainer/test_adversarial_trainer_FBF.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/poisoning/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/poisoning/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2261 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/poisoning/test_strip.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/certification/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/certification/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11748 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/certification/test_randomized_smoothing.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4243 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_GPy.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6173 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_blackbox.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3124 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_blackbox_existing_predictions.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2367 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_catboost.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5292 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_classifier.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    10568 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deep_partition_ensemble.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    70785 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_common.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    20799 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_common.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2934 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_specific.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     8929 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_specific.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6701 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_detector_classifier.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     9006 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_ensemble.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12280 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_input_filter.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2088 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_jax.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5232 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_jax.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2349 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_lightgbm.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5964 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_query_efficient_bb.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    25143 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_scikitlearn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3920 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_xgboost.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    12060 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_pytorch_faster_rcnn.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    14679 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_pytorch_object_detector.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    11526 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_tensorflow_faster_rcnn.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_tracking/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_tracking/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3638 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/object_tracking/test_pytorch_goturn.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/regression/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2665 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/regression/test_scikitlearn.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2052 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/conftest.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    27926 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_deep_speech.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5212 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_deep_speech.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4484 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_espresso.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5302 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_espresso.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    13525 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_tensorflow_lingvo.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/evaluations/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/evaluations/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3308 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/evaluations/test_security_curve.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/privacy/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/privacy/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4816 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/privacy/test_membership_leakage.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     2968 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/test_gradient_check.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    16000 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/test_metrics.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6184 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/metrics/test_verification_decision_trees.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19262 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7538 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     7187 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter_pytorch.json
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     6734 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter_pytorch.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/__init__.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/__init__.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4715 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_brightness.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5922 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_contrast.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3209 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_gaussian_noise.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3177 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_shot_noise.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5740 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_zoom_blur.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3180 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/test_image_rotation.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     3757 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/preprocessing/test_standardisation_mean_std.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    15422 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/test_data_generators.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     1773 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/test_optimizers.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4654 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/test_summary_writer.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    19616 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/test_utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     4588 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/test_visualization.py
+drwxrwxr-x   0 bbuesser  (1000) bbuesser  (1001)        0 2022-01-07 13:28:20.000000 adversarial-robustness-toolbox-1.9.1/tests/utils/
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)     5345 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/utils/test_utils.py
+-rw-rw-r--   0 bbuesser  (1000) bbuesser  (1001)    62459 2022-01-07 13:27:54.000000 adversarial-robustness-toolbox-1.9.1/tests/utils.py
```

### Comparing `adversarial-robustness-toolbox-1.9.0/AUTHORS` & `adversarial-robustness-toolbox-1.9.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/CODE_OF_CONDUCT.md` & `adversarial-robustness-toolbox-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/CONTRIBUTING.md` & `adversarial-robustness-toolbox-1.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/LICENSE` & `adversarial-robustness-toolbox-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/MAINTAINERS.md` & `adversarial-robustness-toolbox-1.9.1/MAINTAINERS.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/PKG-INFO` & `adversarial-robustness-toolbox-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adversarial-robustness-toolbox
-Version: 1.9.0
+Version: 1.9.1
 Summary: Toolbox for adversarial machine learning.
 Home-page: https://github.com/Trusted-AI/adversarial-robustness-toolbox
 Author: Irina Nicolae
 Author-email: irinutza.n@gmail.com
 Maintainer: Beat Buesser
 Maintainer-email: beat.buesser@ie.ibm.com
 License: MIT
```

### Comparing `adversarial-robustness-toolbox-1.9.0/PULL_REQUEST_TEMPLATE.md` & `adversarial-robustness-toolbox-1.9.1/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/README-cn.md` & `adversarial-robustness-toolbox-1.9.1/README-cn.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/README.md` & `adversarial-robustness-toolbox-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/SECURITY.md` & `adversarial-robustness-toolbox-1.9.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/PKG-INFO` & `adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adversarial-robustness-toolbox
-Version: 1.9.0
+Version: 1.9.1
 Summary: Toolbox for adversarial machine learning.
 Home-page: https://github.com/Trusted-AI/adversarial-robustness-toolbox
 Author: Irina Nicolae
 Author-email: irinutza.n@gmail.com
 Maintainer: Beat Buesser
 Maintainer-email: beat.buesser@ie.ibm.com
 License: MIT
```

### Comparing `adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/SOURCES.txt` & `adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/adversarial_robustness_toolbox.egg-info/requires.txt` & `adversarial-robustness-toolbox-1.9.1/adversarial_robustness_toolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from art import defences
 from art import estimators
 from art import evaluations
 from art import metrics
 from art import preprocessing
 
 # Semantic Version
-__version__ = "1.9.0"
+__version__ = "1.9.1"
 
 # pylint: disable=C0103
 
 LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_asr.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_asr.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/adversarial_patch_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/adversarial_patch_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_patch/utils.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_patch/utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/adversarial_texture/adversarial_texture_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/adversarial_texture/adversarial_texture_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/auto_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/auto_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/auto_projected_gradient_descent.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/auto_projected_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/boundary.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/boundary.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/brendel_bethge.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/brendel_bethge.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/carlini.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/carlini.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/decision_tree_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/decision_tree_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/deepfool.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/deepfool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/dpatch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/dpatch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/dpatch_robust.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/dpatch_robust.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/elastic_net.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/elastic_net.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/fast_gradient.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/fast_gradient.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/feature_adversaries/feature_adversaries_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/feature_adversaries/feature_adversaries_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/frame_saliency.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/frame_saliency.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/geometric_decision_based_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/geometric_decision_based_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/hclu.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/hclu.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/hop_skip_jump.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/hop_skip_jump.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/imperceptible_asr.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/imperceptible_asr.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/imperceptible_asr/imperceptible_asr_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/imperceptible_asr/imperceptible_asr_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/iterative_method.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/iterative_method.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/algorithms.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/algorithms.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/laser_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/laser_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/laser_attack/utils.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/laser_attack/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from abc import ABC, abstractmethod
 from logging import Logger
 from pathlib import Path
 import string
 from typing import Any, Callable, List, Tuple, Union
 
 import numpy as np
-import matplotlib.pyplot as plt
 
 
 class Line:
     """
     Representation of the linear function.
     """
 
@@ -252,14 +251,16 @@
     Saves normalized RGB image, passed as numpy array to the set directory - default: "attack".
 
     :param image: Image to save.
     :param number: i.e. class of the image.
     :param name_length: Length of the random string in the name.
     :param directory: Directory where images will be saved.
     """
+    import matplotlib.pyplot as plt
+
     alphabet = np.array(list(string.ascii_letters))
     Path(directory).mkdir(exist_ok=True)
     im_name = f"{directory}/{number}_{''.join(np.random.choice(alphabet, size=name_length))}.jpg"
     plt.imsave(im_name, image)
 
 
 class DebugInfo:
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/lowprofool.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/lowprofool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/newtonfool.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/newtonfool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/over_the_air_flickering/over_the_air_flickering_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/over_the_air_flickering/over_the_air_flickering_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/pe_malware_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/pe_malware_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/pixel_threshold.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/pixel_threshold.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_tensorflow_v2.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/projected_gradient_descent/projected_gradient_descent_tensorflow_v2.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/saliency_map.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/saliency_map.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/shadow_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/shadow_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/shapeshifter.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/shapeshifter.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/simba.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/simba.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/spatial_transformation.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/spatial_transformation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/square_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/square_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/targeted_universal_perturbation.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/targeted_universal_perturbation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/universal_perturbation.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/universal_perturbation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/virtual_adversarial.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/virtual_adversarial.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/wasserstein.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/wasserstein.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/evasion/zoo.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/evasion/zoo.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/copycat_cnn.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/copycat_cnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/functionally_equivalent_extraction.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/functionally_equivalent_extraction.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/extraction/knockoff_nets.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/extraction/knockoff_nets.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/baseline.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/baseline.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/black_box.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/black_box.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/meminf_based.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/meminf_based.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/true_label_baseline.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/true_label_baseline.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/white_box_decision_tree.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/white_box_decision_tree.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/attribute_inference/white_box_lifestyle_decision_tree.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/attribute_inference/white_box_lifestyle_decision_tree.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/black_box.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/black_box.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/black_box_rule_based.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/black_box_rule_based.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/label_only_boundary_distance.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/label_only_boundary_distance.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/label_only_gap_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/label_only_gap_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/membership_inference/shadow_models.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/membership_inference/shadow_models.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/model_inversion/mi_face.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/model_inversion/mi_face.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/inference/reconstruction/white_box.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/inference/reconstruction/white_box.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/adversarial_embedding_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/adversarial_embedding_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/backdoor_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/bullseye_polytope_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/bullseye_polytope_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/clean_label_backdoor_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/clean_label_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/feature_collision_attack.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/feature_collision_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/perturbations/image_perturbations.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/perturbations/image_perturbations.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/attacks/poisoning/poisoning_attack_svm.py` & `adversarial-robustness-toolbox-1.9.1/art/attacks/poisoning/poisoning_attack_svm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/config.py` & `adversarial-robustness-toolbox-1.9.1/art/config.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/data_generators.py` & `adversarial-robustness-toolbox-1.9.1/art/data_generators.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/detector.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/detector.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scanner.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scanner.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scanningops.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scanningops.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/evasion/subsetscanning/scoring_functions.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/evasion/subsetscanning/scoring_functions.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/activation_defence.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/activation_defence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/clustering_analyzer.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/clustering_analyzer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/ground_truth_evaluator.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/ground_truth_evaluator.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/poison_filtering_defence.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/poison_filtering_defence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/provenance_defense.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/provenance_defense.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/roni.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/roni.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/detector/poison/spectral_signature_defense.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/detector/poison/spectral_signature_defense.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/class_labels.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/class_labels.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/gaussian_noise.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/high_confidence.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/high_confidence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/postprocessor.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/postprocessor.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/reverse_sigmoid.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/reverse_sigmoid.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/postprocessor/rounded.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/postprocessor/rounded.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/feature_squeezing.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/feature_squeezing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/gaussian_augmentation.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/gaussian_augmentation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/inverse_gan.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/inverse_gan.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/jpeg_compression.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/jpeg_compression.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/label_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/mp3_compression.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/mp3_compression.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/mp3_compression_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/mp3_compression_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/pixel_defend.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/pixel_defend.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/preprocessor.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/preprocessor.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/resample.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/resample.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/spatial_smoothing_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/spatial_smoothing_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/thermometer_encoding.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/thermometer_encoding.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/variance_minimization.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/variance_minimization.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/video_compression.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/video_compression.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
 import os
 from tempfile import TemporaryDirectory
 from typing import Optional, Tuple
+import warnings
 
 import numpy as np
 from tqdm.auto import tqdm
 
 from art import config
 from art.defences.preprocessor.preprocessor import Preprocessor
 
@@ -74,28 +75,32 @@
         self.verbose = verbose
         self._check_params()
 
     def __call__(self, x: np.ndarray, y: Optional[np.ndarray] = None) -> Tuple[np.ndarray, Optional[np.ndarray]]:
         """
         Apply video compression to sample `x`.
 
-        :param x: Sample to compress of shape NCFHW or NFHWC. `x` values are expected to be in the data range [0, 255].
+        :param x: Sample to compress of shape NCFHW or NFHWC. `x` values are expected to be either in range [0, 1] or
+                  [0, 255].
         :param y: Labels of the sample `x`. This function does not affect them in any way.
         :return: Compressed sample.
         """
 
         def compress_video(x: np.ndarray, video_format: str, constant_rate_factor: int, dir_: str = ""):
             """
             Apply video compression to video input of shape (frames, height, width, channel).
             """
             import ffmpeg
 
             video_path = os.path.join(dir_, f"tmp_video.{video_format}")
             _, height, width, _ = x.shape
 
+            if (height % 2) != 0 or (width % 2) != 0:
+                warnings.warn("Codec might require even number of pixels in height and width.")
+
             # numpy to local video file
             process = (
                 ffmpeg.input("pipe:", format="rawvideo", pix_fmt="rgb24", s=f"{width}x{height}")
                 .output(video_path, pix_fmt="yuv420p", vcodec="libx264", crf=constant_rate_factor)
                 .overwrite_output()
                 .run_async(pipe_stdin=True, quiet=True)
             )
@@ -114,19 +119,27 @@
         if x.ndim != 5:
             raise ValueError("Video compression can only be applied to spatio-temporal data.")
 
         if self.channels_first:
             x = np.transpose(x, (0, 2, 3, 4, 1))
 
         # apply video compression per video item
+        scale = 1
+        if x.min() >= 0 and x.max() <= 1.0:
+            scale = 255
+
         x_compressed = x.copy()
         with TemporaryDirectory(dir=config.ART_DATA_PATH) as tmp_dir:
             for i, x_i in enumerate(tqdm(x, desc="Video compression", disable=not self.verbose)):
+                x_i *= scale
                 x_compressed[i] = compress_video(x_i, self.video_format, self.constant_rate_factor, dir_=tmp_dir)
 
+        x_compressed = x_compressed / scale
+        x_compressed = x_compressed.astype(x.dtype)
+
         if self.channels_first:
             x_compressed = np.transpose(x_compressed, (0, 4, 1, 2, 3))
 
         return x_compressed, y
 
     def _check_params(self) -> None:
         if not (isinstance(self.constant_rate_factor, int) and 0 <= self.constant_rate_factor < 52):
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/preprocessor/video_compression_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/preprocessor/video_compression_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,19 +112,25 @@
 
     def forward(
         self, x: "torch.Tensor", y: Optional["torch.Tensor"] = None
     ) -> Tuple["torch.Tensor", Optional["torch.Tensor"]]:
         """
         Apply video compression to sample `x`.
 
-        :param x: Sample to compress of shape NCFHW or NFHWC. `x` values are expected to be in the data range [0, 255].
+        :param x: Sample to compress of shape NCFHW or NFHWC. `x` values are expected to be either in range [0, 1] or
+                  [0, 255].
         :param y: Labels of the sample `x`. This function does not affect them in any way.
         :return: Compressed sample.
         """
+        scale = 1
+        if x.min() >= 0 and x.max() <= 1.0:
+            scale = 255
+        x = x * scale
         x_compressed = self._compression_pytorch_numpy.apply(x)
+        x_compressed = x_compressed / scale
         return x_compressed, y
 
     def _check_params(self) -> None:
         if not (isinstance(self.constant_rate_factor, int) and 0 <= self.constant_rate_factor < 52):
             raise ValueError("Constant rate factor must be an integer in the range [0, 51].")
 
         if not isinstance(self.verbose, bool):
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_fbf.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_fbf.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_fbf_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_fbf_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/trainer/adversarial_trainer_madry_pgd.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/trainer/adversarial_trainer_madry_pgd.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/trainer/trainer.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/transformer/evasion/defensive_distillation.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/transformer/evasion/defensive_distillation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/neural_cleanse.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/neural_cleanse.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/transformer/poisoning/strip.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/transformer/poisoning/strip.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/defences/transformer/transformer.py` & `adversarial-robustness-toolbox-1.9.1/art/defences/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/certification/abstain.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/certification/abstain.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/randomized_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/randomized_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/certification/randomized_smoothing/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/certification/randomized_smoothing/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/GPy.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/GPy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/blackbox.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/blackbox.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/catboost.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/catboost.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/classifier.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/classifier.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/deep_partition_ensemble.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/deep_partition_ensemble.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/detector_classifier.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/detector_classifier.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/ensemble.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/ensemble.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/keras.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,24 +388,26 @@
         if self._reduce_labels:
             y_preprocessed = np.argmax(y_preprocessed, axis=1)
 
         predictions = self._model.predict(x_preprocessed)
 
         if self._orig_loss and hasattr(self._orig_loss, "reduction"):
             prev_reduction = self._orig_loss.reduction
-            self._orig_loss.reduction = self._losses.Reduction.NONE
+            if hasattr(self._losses, "Reduction"):
+                self._orig_loss.reduction = self._losses.Reduction.NONE
             loss = self._orig_loss(y_preprocessed, predictions)
             self._orig_loss.reduction = prev_reduction
         else:
             prev_reduction = []
             predictions = k.constant(predictions)
             y_preprocessed = k.constant(y_preprocessed)
             for loss_function in self._model.loss_functions:
                 prev_reduction.append(loss_function.reduction)
-                loss_function.reduction = self._losses.Reduction.NONE
+                if hasattr(self._losses, "Reduction"):
+                    loss_function.reduction = self._losses.Reduction.NONE
             loss = self._loss_function(y_preprocessed, predictions)
             for i, loss_function in enumerate(self._model.loss_functions):
                 loss_function.reduction = prev_reduction[i]
 
         loss_value = k.eval(loss)
 
         if reduction == "none":
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/lightgbm.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/lightgbm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/mxnet.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/mxnet.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,32 +830,36 @@
         :return: The output of `layer`, where the first dimension is the batch size corresponding to `x`.
         """
         import torch  # lgtm [py/repeated-import]
 
         self._model.eval()
 
         # Apply defences
-        x_preprocessed, _ = self._apply_preprocessing(x=x, y=None, fit=False)
+        if framework:
+            no_grad = False
+        else:
+            no_grad = True
+        x_preprocessed, _ = self._apply_preprocessing(x=x, y=None, fit=False, no_grad=no_grad)
 
         # Get index of the extracted layer
         if isinstance(layer, six.string_types):
             if layer not in self._layer_names:  # pragma: no cover
                 raise ValueError("Layer name %s not supported" % layer)
             layer_index = self._layer_names.index(layer)
 
         elif isinstance(layer, int):
             layer_index = layer
 
         else:  # pragma: no cover
             raise TypeError("Layer must be of type str or int")
 
         if framework:
-            if isinstance(x, torch.Tensor):
-                return self._model(x)[layer_index]
-            return self._model(torch.from_numpy(x).to(self._device))[layer_index]
+            if isinstance(x_preprocessed, torch.Tensor):
+                return self._model(x_preprocessed)[layer_index]
+            return self._model(torch.from_numpy(x_preprocessed).to(self._device))[layer_index]
 
         # Run prediction with batch processing
         results = []
         num_batch = int(np.ceil(len(x_preprocessed) / float(batch_size)))
 
         for m in range(num_batch):
             # Batch indexes
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/query_efficient_bb.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/query_efficient_bb.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/scikitlearn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/scikitlearn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/classification/xgboost.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/classification/xgboost.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/encoder.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/encoder.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/encoding/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/encoding/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/estimator.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/generation/generator.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/generation/generator.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/generation/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/generation/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/keras.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/keras.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/mxnet.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/mxnet.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/object_detector.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/object_detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/python_object_detector.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/python_object_detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/pytorch_faster_rcnn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/pytorch_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/tensorflow_faster_rcnn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/tensorflow_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_detection/utils.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/object_tracker.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/object_tracker.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/object_tracking/pytorch_goturn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/object_tracking/pytorch_goturn.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,18 +666,19 @@
         for i in range(x.shape[0]):
             if isinstance(x, np.ndarray):
                 x_i = torch.from_numpy(x[i]).to(self.device)
             else:
                 x_i = x[i].to(self.device)
 
             # Apply preprocessing
+            x_i = torch.unsqueeze(x_i, dim=0)
             x_i, _ = self._apply_preprocessing(x_i, y=None, fit=False, no_grad=False)
+            x_i = torch.squeeze(x_i)
 
             y_pred = self._track(x=x_i, y_init=y_init[i])
-
             prediction_dict = dict()
             if isinstance(x, np.ndarray):
                 prediction_dict["boxes"] = y_pred.detach().cpu().numpy()
             else:
                 prediction_dict["boxes"] = y_pred
             predictions.append(prediction_dict)
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/keras.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/keras.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/neural_cleanse/neural_cleanse.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/neural_cleanse/neural_cleanse.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/poison_mitigation/strip/strip.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/poison_mitigation/strip/strip.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/regression/regressor.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/regression/regressor.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/regression/scikitlearn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/regression/scikitlearn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/scikitlearn.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/scikitlearn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/pytorch_deep_speech.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/pytorch_deep_speech.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/pytorch_espresso.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/pytorch_espresso.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/speech_recognizer.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/speech_recognizer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/speech_recognition/tensorflow_lingvo.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/speech_recognition/tensorflow_lingvo.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/estimators/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/estimators/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/evaluations/evaluation.py` & `adversarial-robustness-toolbox-1.9.1/art/evaluations/evaluation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/evaluations/security_curve/security_curve.py` & `adversarial-robustness-toolbox-1.9.1/art/evaluations/security_curve/security_curve.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/exceptions.py` & `adversarial-robustness-toolbox-1.9.1/art/exceptions.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/classification/jax.py` & `adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/classification/jax.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/experimental/estimators/jax.py` & `adversarial-robustness-toolbox-1.9.1/art/experimental/estimators/jax.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/metrics/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/metrics/gradient_check.py` & `adversarial-robustness-toolbox-1.9.1/art/metrics/gradient_check.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/metrics/metrics.py` & `adversarial-robustness-toolbox-1.9.1/art/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/metrics/privacy/membership_leakage.py` & `adversarial-robustness-toolbox-1.9.1/art/metrics/privacy/membership_leakage.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/metrics/verification_decisions_trees.py` & `adversarial-robustness-toolbox-1.9.1/art/metrics/verification_decisions_trees.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/optimizers.py` & `adversarial-robustness-toolbox-1.9.1/art/optimizers.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/audio/l_filter/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/audio/l_filter/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/__init__.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/image_rotation/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/image_rotation/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/brightness/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/contrast/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/gaussian_noise/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/shot_noise/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/natural_corruptions/zoom_blur/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/expectation_over_transformation/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/expectation_over_transformation/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/preprocessing.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/numpy.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/numpy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/pytorch.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/preprocessing/standardisation_mean_std/utils.py` & `adversarial-robustness-toolbox-1.9.1/art/preprocessing/standardisation_mean_std/utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/summary_writer.py` & `adversarial-robustness-toolbox-1.9.1/art/summary_writer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/art/utils.py` & `adversarial-robustness-toolbox-1.9.1/art/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,25 +971,28 @@
     y_train = targets[:split_index]
     x_test = data[split_index:]
     y_test = targets[split_index:]
 
     return (x_train, y_train), (x_test, y_test), min_, max_
 
 
-def load_nursery(raw: bool = False, test_set: float = 0.2, transform_social: bool = False) -> DATASET_TYPE:
+def load_nursery(
+    raw: bool = False, scaled: bool = True, test_set: float = 0.2, transform_social: bool = False
+) -> DATASET_TYPE:
     """
     Loads the UCI Nursery dataset from `config.ART_DATA_PATH` or downloads it if necessary.
 
     :param raw: `True` if no preprocessing should be applied to the data. Otherwise, categorical data is one-hot
-                encoded and data is scaled using sklearn's StandardScaler.
+                encoded and data is scaled using sklearn's StandardScaler according to the value of `scaled`.
+    :param scaled: `True` if data should be scaled.
     :param test_set: Proportion of the data to use as validation split. The value should be between 0 and 1.
     :param transform_social: If `True`, transforms the social feature to be binary for the purpose of attribute
                              inference. This is done by assigning the original value 'problematic' the new value 1, and
                              the other original values are assigned the new value 0.
-    :return: Entire dataset and labels.
+    :return: Entire dataset and labels as numpy array.
     """
     import pandas as pd
     import sklearn.preprocessing
 
     # Download data if needed
     path = get_file(
         "nursery.data",
@@ -1046,35 +1049,43 @@
             data[feature] = pd.Categorical(data.loc[:, feature], categories=values, ordered=False)
             one_hot_vector = pd.get_dummies(data[feature], prefix=feature)
             data = pd.concat([data, one_hot_vector], axis=1)
             features_to_remove.append(feature)
         data = data.drop(features_to_remove, axis=1)
 
         # normalize data
-        label = data.loc[:, "label"]
-        features = data.drop(["label"], axis=1)
-        scaler = sklearn.preprocessing.StandardScaler()
-        scaler.fit(features)
-        scaled_features = pd.DataFrame(scaler.transform(features), columns=features.columns)
-
-        data = pd.concat([label, scaled_features], axis=1, join="inner")
+        if scaled:
+            label = data.loc[:, "label"]
+            features = data.drop(["label"], axis=1)
+            scaler = sklearn.preprocessing.StandardScaler()
+            scaler.fit(features)
+            scaled_features = pd.DataFrame(scaler.transform(features), columns=features.columns)
+            data = pd.concat([label, scaled_features], axis=1, join="inner")
 
     features = data.drop(["label"], axis=1)
-    min_, max_ = np.amin(features.to_numpy()), np.amax(features.to_numpy())
+    if raw:
+        numeric_features = features.drop(categorical_features, axis=1).to_numpy().astype(np.int32)
+        min_, max_ = np.amin(numeric_features), np.amax(numeric_features)
+    else:
+        min_, max_ = np.amin(features.to_numpy().astype(np.float64)), np.amax(features.to_numpy().astype(np.float64))
 
     # Split training and test sets
     stratified = sklearn.model_selection.StratifiedShuffleSplit(n_splits=1, test_size=test_set, random_state=18)
     for train_set_i, test_set_i in stratified.split(data, data["label"]):
         train = data.iloc[train_set_i]
         test = data.iloc[test_set_i]
     x_train = train.drop(["label"], axis=1).to_numpy()
     y_train = train.loc[:, "label"].to_numpy()
     x_test = test.drop(["label"], axis=1).to_numpy()
     y_test = test.loc[:, "label"].to_numpy()
 
+    if not raw and not scaled:
+        x_train = x_train.astype(np.float64)
+        x_test = x_test.astype(np.float64)
+
     return (x_train, y_train), (x_test, y_test), min_, max_
 
 
 def load_dataset(
     name: str,
 ) -> DATASET_TYPE:
     """
```

### Comparing `adversarial-robustness-toolbox-1.9.0/art/visualization.py` & `adversarial-robustness-toolbox-1.9.1/art/visualization.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/Makefile` & `adversarial-robustness-toolbox-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/conf.py` & `adversarial-robustness-toolbox-1.9.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 project = "Adversarial Robustness Toolbox"
 copyright = "2018, The Adversarial Robustness Toolbox (ART) Authors"
 author = "Maria-Irina Nicolae"
 
 # The short X.Y version
 version = "1.9"
 # The full version, including alpha/beta/rc tags
-release = "1.9.0"
+release = "1.9.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/adversarial_threats_art.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/adversarial_threats_art.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/adversarial_threats_attacker.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/adversarial_threats_attacker.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/art_architecture.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/art_architecture.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/art_lfai.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/art_lfai.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/art_logo.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/art_logo.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/art_logo_3d_1.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/art_logo_3d_1.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/summary_writer_patch.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/summary_writer_patch.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/summary_writer_scalar.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/summary_writer_scalar.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/images/white_hat_blue_red.png` & `adversarial-robustness-toolbox-1.9.1/docs/images/white_hat_blue_red.png`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/index.rst` & `adversarial-robustness-toolbox-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/make.bat` & `adversarial-robustness-toolbox-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/evasion.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/evasion.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/attribute_inference.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/attribute_inference.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/inference/membership_inference.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/inference/membership_inference.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/attacks/poisoning.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/attacks/poisoning.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/attacks.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/attacks.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/defences/detector_poisoning.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/defences/detector_poisoning.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/defences/postprocessor.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/defences/postprocessor.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/defences/preprocessor.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/defences/preprocessor.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/defences/trainer.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/defences/trainer.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/certification_randomized_smoothing.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/certification_randomized_smoothing.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/classification.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/classification.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/classification_scikitlearn.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/classification_scikitlearn.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/object_detection.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/object_detection.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators/speech_recognition.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators/speech_recognition.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/estimators.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/estimators.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/metrics.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/metrics.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/expectation_over_transformation.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/expectation_over_transformation.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/preprocessing/standardisation_mean_std.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/preprocessing/standardisation_mean_std.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/tests/utils.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/tests/utils.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/docs/modules/utils.rst` & `adversarial-robustness-toolbox-1.9.1/docs/modules/utils.rst`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/README.md` & `adversarial-robustness-toolbox-1.9.1/examples/README.md`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_FBF.py` & `adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_FBF.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_cifar10.py` & `adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_cifar10.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/adversarial_training_data_augmentation.py` & `adversarial-robustness-toolbox-1.9.1/examples/adversarial_training_data_augmentation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/application_object_detection.py` & `adversarial-robustness-toolbox-1.9.1/examples/application_object_detection.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_fasterrcnn.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_fasterrcnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_inverse_gan.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_inverse_gan.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_keras.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_keras.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_lightgbm.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_lightgbm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_mxnet.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_mxnet.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_pytorch_goturn.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_pytorch_goturn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_scikit_learn.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_scikit_learn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_tensorflow_v2.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_tensorflow_v2.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/get_started_xgboost.py` & `adversarial-robustness-toolbox-1.9.1/examples/get_started_xgboost.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/inverse_gan_author_utils.py` & `adversarial-robustness-toolbox-1.9.1/examples/inverse_gan_author_utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/mnist_cnn_features_level_fgsm.py` & `adversarial-robustness-toolbox-1.9.1/examples/mnist_cnn_features_level_fgsm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/mnist_cnn_fgsm.py` & `adversarial-robustness-toolbox-1.9.1/examples/mnist_cnn_fgsm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/mnist_poison_detection.py` & `adversarial-robustness-toolbox-1.9.1/examples/mnist_poison_detection.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/examples/mnist_transferability.py` & `adversarial-robustness-toolbox-1.9.1/examples/mnist_transferability.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/setup.cfg` & `adversarial-robustness-toolbox-1.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/setup.py` & `adversarial-robustness-toolbox-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/conftest.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/conftest.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/conftest.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/conftest.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/feature_adversaries/test_feature_adversaries_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_adversarial_asr.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_adversarial_asr.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_adversarial_texture_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_adversarial_texture_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_auto_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_auto_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_auto_projected_gradient_descent.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_auto_projected_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_boundary.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_boundary.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_brendel_and_bethge.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_brendel_and_bethge.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_dpatch.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_dpatch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_dpatch_robust.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_dpatch_robust.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_fast_gradient.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_fast_gradient.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_frame_saliency.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_frame_saliency.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_geometric_decision_based_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_geometric_decision_based_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr_pytorch.json` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr_pytorch.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_imperceptible_asr_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_imperceptible_asr_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_laser_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_laser_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_lowprofool.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_lowprofool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_over_the_air.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_over_the_air.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_pe_malware_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_pe_malware_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_shadow_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_shadow_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/evasion/test_square_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/evasion/test_square_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_baseline.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_baseline.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_black_box.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_black_box.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_meminf_based.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_meminf_based.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_true_label_baseline.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_true_label_baseline.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_white_box_decision_tree.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_white_box_decision_tree.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/attribute_inference/test_white_box_lifestyle_decision_tree.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/attribute_inference/test_white_box_lifestyle_decision_tree.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_black_box.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_black_box.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_black_box_rule_based.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_black_box_rule_based.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_label_only_boundary_distance.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_label_only_boundary_distance.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_label_only_gap_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_label_only_gap_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/membership_inference/test_shadow_models.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/membership_inference/test_shadow_models.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/model_inversion/test_mi_face.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/model_inversion/test_mi_face.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/inference/test_reconstruction.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/inference/test_reconstruction.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_bullseye_polytope_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_bullseye_polytope_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_clean_label_backdoor_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_clean_label_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/poison/test_image_perturbations.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/poison/test_image_perturbations.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_adversarial_embedding.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_adversarial_embedding.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_adversarial_patch.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_adversarial_patch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_backdoor_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_backdoor_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_carlini.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_carlini.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_copycat_cnn.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_copycat_cnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_decision_tree_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_decision_tree_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_deepfool.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_deepfool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_elastic_net.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_elastic_net.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_feature_collision.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_feature_collision.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_functionally_equivalent_extraction.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_functionally_equivalent_extraction.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_hclu.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_hclu.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_hop_skip_jump.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_hop_skip_jump.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_input_filter.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_input_filter.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_iterative_method.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_iterative_method.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_knockoff_nets.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_knockoff_nets.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_newtonfool.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_newtonfool.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_pixel_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_pixel_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_poisoning_attack_svm.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_poisoning_attack_svm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_projected_gradient_descent.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_projected_gradient_descent.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_saliency_map.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_saliency_map.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_shapeshifter.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_shapeshifter.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_simba.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_simba.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_spatial_transformation.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_spatial_transformation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_targeted_universal_perturbation.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_targeted_universal_perturbation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_threshold_attack.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_threshold_attack.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_universal_perturbation.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_universal_perturbation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_virtual_adversarial.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_virtual_adversarial.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_wasserstein.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_wasserstein.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/test_zoo.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/test_zoo.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/attacks/utils.py` & `adversarial-robustness-toolbox-1.9.1/tests/attacks/utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/classifiersFrameworks/test_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/classifiersFrameworks/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/classifiersFrameworks/test_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/tests/classifiersFrameworks/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/subsetscanning/test_detector.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/subsetscanning/test_detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/evasion/test_detector.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/evasion/test_detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_activation_defence.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_activation_defence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_clustering_analyzer.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_clustering_analyzer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_ground_truth_evaluator.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_ground_truth_evaluator.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_provenance_defence.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_provenance_defence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_roni.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_roni.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/detector/poison/test_spectral_signature_defense.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/detector/poison/test_spectral_signature_defense.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/conftest.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/conftest.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_inverse_gan.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_inverse_gan.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_jpeg_compression.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_jpeg_compression.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_mp3_compression.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_mp3_compression.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_mp3_compression_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_mp3_compression_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_preprocessor.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_resample.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_resample.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_spatial_smoothing_tensorflow.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_spatial_smoothing_tensorflow.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_video_compression.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_video_compression.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/preprocessor/test_video_compression_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/preprocessor/test_video_compression_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_adversarial_trainer.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_adversarial_trainer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_adversarial_trainer_madry_pgd.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_adversarial_trainer_madry_pgd.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_class_labels.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_class_labels.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_defensive_distillation.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_defensive_distillation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_feature_squeezing.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_feature_squeezing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_gaussian_augmentation.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_gaussian_augmentation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_gaussian_noise.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_high_confidence.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_high_confidence.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_label_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_label_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_neural_cleanse.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_neural_cleanse.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_pixel_defend.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_pixel_defend.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_reverse_sigmoid.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_reverse_sigmoid.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_rounded.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_rounded.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_thermometer_encoding.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_thermometer_encoding.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/test_variance_minimization.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/test_variance_minimization.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/trainer/test_adversarial_trainer_FBF.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/trainer/test_adversarial_trainer_FBF.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/defences/transformer/poisoning/test_strip.py` & `adversarial-robustness-toolbox-1.9.1/tests/defences/transformer/poisoning/test_strip.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/certification/test_randomized_smoothing.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/certification/test_randomized_smoothing.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_GPy.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_GPy.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_blackbox.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_blackbox.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_blackbox_existing_predictions.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_blackbox_existing_predictions.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_catboost.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_catboost.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_classifier.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_classifier.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deep_partition_ensemble.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deep_partition_ensemble.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_common.json` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_common.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_common.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_common.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_specific.json` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_specific.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_deeplearning_specific.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_deeplearning_specific.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_detector_classifier.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_detector_classifier.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_ensemble.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_input_filter.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_input_filter.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_jax.json` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_jax.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_jax.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_jax.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_lightgbm.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_lightgbm.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_query_efficient_bb.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_query_efficient_bb.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_scikitlearn.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_scikitlearn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/classification/test_xgboost.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/classification/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_pytorch_faster_rcnn.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_pytorch_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_pytorch_object_detector.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_pytorch_object_detector.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/object_detection/test_tensorflow_faster_rcnn.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/object_detection/test_tensorflow_faster_rcnn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/object_tracking/test_pytorch_goturn.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/object_tracking/test_pytorch_goturn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/regression/test_scikitlearn.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/regression/test_scikitlearn.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/conftest.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/conftest.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_deep_speech.json` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_deep_speech.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_deep_speech.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_deep_speech.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_espresso.json` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_espresso.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_pytorch_espresso.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_pytorch_espresso.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/estimators/speech_recognition/test_tensorflow_lingvo.py` & `adversarial-robustness-toolbox-1.9.1/tests/estimators/speech_recognition/test_tensorflow_lingvo.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/evaluations/test_security_curve.py` & `adversarial-robustness-toolbox-1.9.1/tests/evaluations/test_security_curve.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/metrics/privacy/test_membership_leakage.py` & `adversarial-robustness-toolbox-1.9.1/tests/metrics/privacy/test_membership_leakage.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/metrics/test_gradient_check.py` & `adversarial-robustness-toolbox-1.9.1/tests/metrics/test_gradient_check.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/metrics/test_metrics.py` & `adversarial-robustness-toolbox-1.9.1/tests/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/metrics/test_verification_decision_trees.py` & `adversarial-robustness-toolbox-1.9.1/tests/metrics/test_verification_decision_trees.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter.json` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter_pytorch.json` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter_pytorch.json`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/audio/test_l_filter_pytorch.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/audio/test_l_filter_pytorch.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_brightness.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_brightness.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_contrast.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_contrast.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_gaussian_noise.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_shot_noise.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_shot_noise.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_zoom_blur.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/natural_corruptions/test_zoom_blur.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/expectation_over_transformation/test_image_rotation.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/expectation_over_transformation/test_image_rotation.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/preprocessing/test_standardisation_mean_std.py` & `adversarial-robustness-toolbox-1.9.1/tests/preprocessing/test_standardisation_mean_std.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/test_data_generators.py` & `adversarial-robustness-toolbox-1.9.1/tests/test_data_generators.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/test_optimizers.py` & `adversarial-robustness-toolbox-1.9.1/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/test_summary_writer.py` & `adversarial-robustness-toolbox-1.9.1/tests/test_summary_writer.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/test_utils.py` & `adversarial-robustness-toolbox-1.9.1/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,14 +383,24 @@
         (x_train, y_train), (x_test, y_test), min_, max_ = load_dataset("stl10")
         self.assertAlmostEqual(min_, 0.0, places=6)
         self.assertEqual(max_, 1.0)
         self.assertEqual(x_train.shape[0], y_train.shape[0])
         self.assertEqual(x_test.shape[0], y_test.shape[0])
 
     def test_nursery(self):
+        (x_train, y_train), (x_test, y_test), min_, max_ = load_nursery(raw=True)
+        self.assertEqual(x_train.shape[0], y_train.shape[0])
+        self.assertEqual(x_test.shape[0], y_test.shape[0])
+
+        (x_train, y_train), (x_test, y_test), min_, max_ = load_nursery(scaled=False)
+        self.assertEqual(min_, 0.0)
+        self.assertEqual(max_, 4.0)
+        self.assertEqual(x_train.shape[0], y_train.shape[0])
+        self.assertEqual(x_test.shape[0], y_test.shape[0])
+
         (x_train, y_train), (x_test, y_test), min_, max_ = load_nursery()
         self.assertAlmostEqual(min_, -1.3419307411337875, places=6)
         self.assertEqual(max_, 2.0007720517562224)
         self.assertEqual(x_train.shape[0], y_train.shape[0])
         self.assertEqual(x_test.shape[0], y_test.shape[0])
 
         (x_train, y_train), (x_test, y_test), min_, max_ = load_dataset("nursery")
```

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/test_visualization.py` & `adversarial-robustness-toolbox-1.9.1/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/utils/test_utils.py` & `adversarial-robustness-toolbox-1.9.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `adversarial-robustness-toolbox-1.9.0/tests/utils.py` & `adversarial-robustness-toolbox-1.9.1/tests/utils.py`

 * *Files identical despite different names*

