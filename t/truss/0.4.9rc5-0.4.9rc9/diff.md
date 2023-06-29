# Comparing `tmp/truss-0.4.9rc5.tar.gz` & `tmp/truss-0.4.9rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.9rc5.tar", max compression
+gzip compressed data, was "truss-0.4.9rc9.tar", max compression
```

## Comparing `truss-0.4.9rc5.tar` & `truss-0.4.9rc9.tar`

### file list

```diff
@@ -1,184 +1,187 @@
--rw-r--r--   0        0        0     5483 2023-06-16 19:49:28.511391 truss-0.4.9rc5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-06-16 19:49:28.511391 truss-0.4.9rc5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-06-16 19:49:28.511391 truss-0.4.9rc5/LICENSE
--rw-r--r--   0        0        0     5958 2023-06-16 19:49:28.511391 truss-0.4.9rc5/README.md
--rw-r--r--   0        0        0      933 2023-06-16 19:49:28.511391 truss-0.4.9rc5/context_builder.Dockerfile
--rw-r--r--   0        0        0     2482 2023-06-16 19:49:28.623398 truss-0.4.9rc5/pyproject.toml
--rw-r--r--   0        0        0      330 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/build.py
--rw-r--r--   0        0        0    11326 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     8411 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1893 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2111 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     4715 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/local_server_loader.py
--rw-r--r--   0        0        0     2239 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0      951 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/truss_file_syncer.py
--rw-r--r--   0        0        0     5801 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/errors.py
--rw-r--r--   0        0        0      824 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     5565 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-06-16 19:49:28.623398 truss-0.4.9rc5/truss/notebook.py
--rw-r--r--   0        0        0    10744 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/signature.py
--rw-r--r--   0        0        0     3087 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/truss_dir_patch_applier.py
--rw-r--r--   0        0        0      937 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/__init__.py
--rw-r--r--   0        0        0     1925 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2559 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4272 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      955 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5859 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     3015 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2450 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     1352 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/logging.py
--rw-r--r--   0        0        0      998 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
--rw-r--r--   0        0        0     4483 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
--rw-r--r--   0        0        0      551 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
--rw-r--r--   0        0        0      208 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/system_packages.py
--rw-r--r--   0        0        0     3070 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1875 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/control/server.py
--rw-r--r--   0        0        0      126 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     2382 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     9977 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0     1445 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      727 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0      496 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/local_inference_server.py
--rw-r--r--   0        0        0     6219 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      250 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2769 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0      739 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/model_load_failure_test/config.yaml
--rw-r--r--   0        0        0      552 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/model_load_failure_test/model/model.py
--rw-r--r--   0        0        0     1267 2023-06-16 19:49:28.627398 truss-0.4.9rc5/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     1550 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/__init__.py
--rw-r--r--   0        0        0    20811 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0     1929 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_truss_dir_patch_applier.py
--rw-r--r--   0        0        0      273 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     2065 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
--rw-r--r--   0        0        0      964 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
--rw-r--r--   0        0        0     6977 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_build.py
--rw-r--r--   0        0        0     3181 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_docker.py
--rw-r--r--   0        0        0     7062 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33928 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/tests/test_validation.py
--rw-r--r--   0        0        0    13164 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_config.py
--rw-r--r--   0        0        0     2698 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41382 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/types.py
--rw-r--r--   0        0        0      227 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/jinja.py
--rw-r--r--   0        0        0     2612 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-06-16 19:49:28.631399 truss-0.4.9rc5/truss/validation.py
--rw-r--r--   0        0        0     7725 1970-01-01 00:00:00.000000 truss-0.4.9rc5/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-06-23 00:29:26.573512 truss-0.4.9rc9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-06-23 00:29:26.573512 truss-0.4.9rc9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-06-23 00:29:26.573512 truss-0.4.9rc9/LICENSE
+-rw-r--r--   0        0        0     5958 2023-06-23 00:29:26.573512 truss-0.4.9rc9/README.md
+-rw-r--r--   0        0        0      933 2023-06-23 00:29:26.573512 truss-0.4.9rc9/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2539 2023-06-23 00:29:26.661514 truss-0.4.9rc9/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/build.py
+-rw-r--r--   0        0        0    11326 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/cli.py
+-rw-r--r--   0        0        0     2873 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     8649 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1893 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2111 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     4980 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/local_server_loader.py
+-rw-r--r--   0        0        0     2239 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     3123 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/truss_file_syncer.py
+-rw-r--r--   0        0        0     5801 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1230 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2403 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1225 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     5425 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/notebook.py
+-rw-r--r--   0        0        0    10642 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/hash.py
+-rw-r--r--   0        0        0     2942 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/local_truss_patch_applier.py
+-rw-r--r--   0        0        0      468 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/signature.py
+-rw-r--r--   0        0        0     3087 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      937 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     3275 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4202 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      955 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5859 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     3015 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2691 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     1352 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/logging.py
+-rw-r--r--   0        0        0      998 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py
+-rw-r--r--   0        0        0     4483 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py
+-rw-r--r--   0        0        0      551 2023-06-23 00:29:26.661514 truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py
+-rw-r--r--   0        0        0      208 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/system_packages.py
+-rw-r--r--   0        0        0     3070 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1497 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0      140 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     2382 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     6540 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      727 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0      496 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/local_inference_server.py
+-rw-r--r--   0        0        0     6219 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      250 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2769 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/logging.py
+-rw-r--r--   0        0        0     1430 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0     3318 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/serialization.py
+-rw-r--r--   0        0        0     1445 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/util.py
+-rw-r--r--   0        0        0     1958 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/shared/uvicorn_config.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0      739 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/model_load_failure_test/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/model_load_failure_test/model/model.py
+-rw-r--r--   0        0        0     1267 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20811 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0     1929 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_truss_dir_patch_applier.py
+-rw-r--r--   0        0        0      273 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     2065 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py
+-rw-r--r--   0        0        0      964 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py
+-rw-r--r--   0        0        0     7427 2023-06-23 00:29:26.665514 truss-0.4.9rc9/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_build.py
+-rw-r--r--   0        0        0     3181 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0    14306 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_control_truss_patching.py
+-rw-r--r--   0        0        0      517 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     7062 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    29166 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    13164 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/truss_config.py
+-rw-r--r--   0        0        0     2698 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41534 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/truss_spec.py
+-rw-r--r--   0        0        0     2782 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/types.py
+-rw-r--r--   0        0        0      227 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/util/jinja.py
+-rw-r--r--   0        0        0     2612 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-06-23 00:29:26.669514 truss-0.4.9rc9/truss/validation.py
+-rw-r--r--   0        0        0     7634 1970-01-01 00:00:00.000000 truss-0.4.9rc9/PKG-INFO
```

### Comparing `truss-0.4.9rc5/CODE_OF_CONDUCT.md` & `truss-0.4.9rc9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/CONTRIBUTING.md` & `truss-0.4.9rc9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/LICENSE` & `truss-0.4.9rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/README.md` & `truss-0.4.9rc9/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/context_builder.Dockerfile` & `truss-0.4.9rc9/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/pyproject.toml` & `truss-0.4.9rc9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.9rc5"
+version = "0.4.9rc9"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
@@ -27,20 +27,18 @@
 python-on-whales = "^0.46.0"
 tenacity = "^8.0.1"
 single-source = "^0.3.0"
 cloudpickle = "^2.2.0"
 blake3 = "^0.3.3"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
+httpx = "^0.24.1"
 psutil = "^5.9.4"
 joblib = "^1.2.0"
-dockerfile = "^3.2.0"
-virtualenv = "^20.23.0"
-watchfiles = "^0.19.0"
-yaspin = "^2.3.0"
+pydantic = "^1.10.9"
 
 [tool.poetry.group.builder.dependencies]
 python = ">=3.8,<3.12"
 packaging = "^20.9"
 python-json-logger = ">=2.0.2"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
@@ -48,14 +46,15 @@
 cloudpickle = "^2.2.0"
 single-source = "^0.3.0"
 click = "^8.0.3"
 requests = "^2.28.1"
 blake3 = "^0.3.3"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
+httpx = "^0.24.1"
 psutil = "^5.9.4"
 dockerfile = "^3.2.0"
 virtualenv = "^20.23.0"
 watchfiles = "^0.19.0"
 yaspin = "^2.3.0"
 
 [tool.poetry.dev-dependencies]
@@ -75,14 +74,18 @@
 pytest-cov = "^3.0.0"
 xgboost = "^1.6.1"
 lightgbm = "^3.3.2"
 transformers = "^4.20.1"
 black = "^22.6.0"
 nbconvert = "^7.2.1"
 ipykernel = "^6.16.0"
+dockerfile = "^3.2.0"
+virtualenv = "^20.23.0"
+watchfiles = "^0.19.0"
+yaspin = "^2.3.0"
 
 [tool.poetry.scripts]
 truss = 'truss.cli:cli_group'
 
 [tool.poetry.group.dev.dependencies]
 mlflow = "^1.29.0"
 mypy = "^1.0.0"
```

### Comparing `truss-0.4.9rc5/truss/blob/blob_backend_registry.py` & `truss-0.4.9rc9/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/blob/http_public_blob_backend.py` & `truss-0.4.9rc9/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/build.py` & `truss-0.4.9rc9/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/cli.py` & `truss-0.4.9rc9/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/constants.py` & `truss-0.4.9rc9/truss/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 )
 SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME = "shared"
 SHARED_SERVING_AND_TRAINING_CODE_DIR: pathlib.Path = (
     TEMPLATES_DIR / SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME
 )
 CONTROL_SERVER_CODE_DIR: pathlib.Path = TEMPLATES_DIR / "control"
 
+SUPPORTED_PYTHON_VERSIONS = {"3.8", "3.9", "3.10", "3.11"}
+
 
 # Alias for TEMPLATES_DIR
 SERVING_DIR: pathlib.Path = TEMPLATES_DIR
 
 REQUIREMENTS_TXT_FILENAME = "requirements.txt"
 BASE_SERVER_REQUIREMENTS_TXT_FILENAME = "base_server_requirements.txt"
 SERVER_REQUIREMENTS_TXT_FILENAME = "server_requirements.txt"
```

### Comparing `truss-0.4.9rc5/truss/contexts/image_builder/image_builder.py` & `truss-0.4.9rc9/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.9rc9/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,14 +88,20 @@
             SHARED_SERVING_AND_TRAINING_CODE_DIR,
             BUILD_SERVER_DIR_NAME + "/" + SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
         )
 
         # Copy control server code
         if config.live_reload:
             copy_into_build_dir(CONTROL_SERVER_CODE_DIR, BUILD_CONTROL_SERVER_DIR_NAME)
+            copy_into_build_dir(
+                SHARED_SERVING_AND_TRAINING_CODE_DIR,
+                BUILD_CONTROL_SERVER_DIR_NAME
+                + "/control/"
+                + SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
+            )
 
         # Copy base TrussServer requirements if supplied custom base image
         if config.base_image:
             base_truss_server_reqs_filepath = (
                 SERVER_CODE_DIR / REQUIREMENTS_TXT_FILENAME
             )
             copy_into_build_dir(
```

### Comparing `truss-0.4.9rc5/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.9rc9/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/image_builder/util.py` & `truss-0.4.9rc9/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.4.9rc9/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.9rc9/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/local_server_loader.py` & `truss-0.4.9rc9/truss/contexts/local_loader/local_server_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
+import logging
 import subprocess
 import sys
 import venv
 from pathlib import Path
 from typing import Any, List, Optional
 
 from truss.contexts.image_builder.serving_image_builder import ServingImageBuilder
 from truss.contexts.local_loader.docker_build_emulator import DockerBuildEmulator
 from truss.contexts.local_loader.truss_file_syncer import TrussFilesSyncer
+from truss.patch.local_truss_patch_applier import LocalTrussPatchApplier
 from truss.util.path import build_truss_shadow_target_directory
 from yaspin import yaspin
 
 
 class VenvBuilder(venv.EnvBuilder):
     """Virtual Environment Builder
 
@@ -99,15 +101,15 @@
                 location = build_truss_shadow_target_directory(stub, self.truss_path)
             else:
                 if not location.exists():
                     location.mkdir(parents=True)
             return location
 
         build_dir = _prep_or_create_dir(build_dir, "build")
-        venv_dir = _prep_or_create_dir(build_dir, "server_venv")
+        venv_dir = _prep_or_create_dir(venv_dir, "server_venv")
 
         with yaspin(text="Preparing truss context") as spinner:
             self.context_builder.prepare_image_build_dir(build_dir)
             dockerfile_path = build_dir / "Dockerfile"
             docker_build_emulator = DockerBuildEmulator(dockerfile_path, build_dir)
             build_result = docker_build_emulator.run(venv_dir)
             spinner.ok("✅")
@@ -115,15 +117,22 @@
         venv_builder = VenvBuilder(venv_dir, with_pip=True)
         requirements_files = [
             "app/requirements.txt",
             "requirements.txt",
         ]
         venv_builder.create_with_requirements(requirements_files)
 
-        TrussFilesSyncer(self.truss_path, venv_dir / "app/").start()
+        TrussFilesSyncer(
+            self.truss_path,
+            LocalTrussPatchApplier(
+                venv_dir / "app/",
+                venv_builder.context.env_exe,
+                logging.Logger(__name__),
+            ),
+        ).start()
 
         subprocess.check_call(
             [
                 venv_builder.context.env_exe,
                 "-m",
                 "uvicorn",
                 "local_inference_server:app",
```

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/train_local.py` & `truss-0.4.9rc9/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.9rc9/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/contexts/local_loader/utils.py` & `truss-0.4.9rc9/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/docker.py` & `truss-0.4.9rc9/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/environment_inference/requirements_inference.py` & `truss-0.4.9rc9/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/errors.py` & `truss-0.4.9rc9/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/local/local_config.py` & `truss-0.4.9rc9/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/local/local_config_handler.py` & `truss-0.4.9rc9/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_framework.py` & `truss-0.4.9rc9/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_frameworks/__init__.py` & `truss-0.4.9rc9/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.9rc9/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_frameworks/keras.py` & `truss-0.4.9rc9/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_frameworks/lightgbm.py` & `truss-0.4.9rc9/truss/model_frameworks/lightgbm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, Dict, Set
 
 from truss.constants import LIGHTGBM_REQ_MODULE_NAMES
 from truss.model_framework import ModelFramework
-from truss.templates.server.common.util import model_supports_predict_proba
+from truss.templates.shared.util import model_supports_predict_proba
 from truss.types import ModelFrameworkType
 
 MODEL_FILENAME = "model.joblib"
 
 
 class LightGBM(ModelFramework):
     def typ(self) -> ModelFrameworkType:
```

### Comparing `truss-0.4.9rc5/truss/model_frameworks/mlflow.py` & `truss-0.4.9rc9/truss/model_frameworks/mlflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, Dict, Set
 
 from truss.constants import MLFLOW_REQ_MODULE_NAMES
 from truss.model_framework import ModelFramework
-from truss.templates.server.common.util import model_supports_predict_proba
+from truss.templates.shared.util import model_supports_predict_proba
 from truss.truss_handle import TrussHandle
 from truss.types import ModelFrameworkType
 
 MODEL_FILENAME = "model.joblib"
 
 
 class Mlflow(ModelFramework):
```

### Comparing `truss-0.4.9rc5/truss/model_frameworks/pytorch.py` & `truss-0.4.9rc9/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_frameworks/sklearn.py` & `truss-0.4.9rc9/truss/model_frameworks/sklearn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import Any, Dict, Set
 
 from truss.constants import SKLEARN_REQ_MODULE_NAMES
 from truss.model_framework import ModelFramework
-from truss.templates.server.common.util import model_supports_predict_proba
+from truss.templates.shared.util import model_supports_predict_proba
 from truss.types import ModelFrameworkType
 
 MODEL_FILENAME = "model.joblib"
 
 
 class SKLearn(ModelFramework):
     def typ(self) -> ModelFrameworkType:
```

### Comparing `truss-0.4.9rc5/truss/model_frameworks/xgboost.py` & `truss-0.4.9rc9/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/model_inference.py` & `truss-0.4.9rc9/truss/model_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,14 @@
     PYTORCH,
     SKLEARN,
     TENSORFLOW,
     XGBOOST,
 )
 from truss.errors import FrameworkNotSupportedError
 
-# lists of versions supported by the truss+base_images
-PYTHON_VERSIONS = {
-    "py37",
-    "py38",
-    "py39",
-    "py310",
-    "py311",
-}
-
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _infer_model_framework(model_class: Any):
     model_framework, _, _ = model_class.__module__.partition(".")
     if model_framework == "transformers":
         return HUGGINGFACE_TRANSFORMER
```

### Comparing `truss-0.4.9rc5/truss/patch/calc_patch.py` & `truss-0.4.9rc9/truss/patch/calc_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,24 +107,24 @@
             action = Action.ADD if path in changed_paths["added"] else Action.UPDATE
             patches.append(
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=action,
                         path=_relative_to(path, model_module_path),
-                        content=_file_content(full_path),
+                        content=full_path.read_text(),
                     ),
                 )
             )
         elif path == CONFIG_FILE:
             new_config = TrussConfig.from_yaml(truss_dir / CONFIG_FILE)
             prev_config = TrussConfig.from_dict(
                 yaml.safe_load(previous_truss_signature.config)
             )
-            config_patches = _calc_config_patches(prev_config, new_config)
+            config_patches = calc_config_patches(prev_config, new_config)
             if config_patches is None:
                 logger.info(f"Unable to patch update to {path}")
                 return None
             patches.extend(config_patches)
         elif _under_unsupported_patch_dir(path):
             logger.info(f"Patching not supported for updating {path}")
             return None
@@ -182,15 +182,15 @@
                 (str(path.relative_to(root)) for path in root.glob(ignore_pattern))
             )
             root_relative_ignored_paths.update(ignored_paths_for_pattern)
 
     return root_relative_paths - root_relative_ignored_paths
 
 
-def _calc_config_patches(
+def calc_config_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> Optional[List[Patch]]:
     """Calculate patch based on changes to config.
 
     Returns None if patch cannot be calculated. Empty list means no relevant
     differences found.
     """
@@ -299,12 +299,7 @@
     Checks if given path is under one of the given paths, but not the same as
     them. Assumes that parent paths themselves are not under each other.
     """
     for dir_path in parent_paths:
         if path.startswith(dir_path) and not path == dir_path:
             return True
     return False
-
-
-def _file_content(path: Path) -> str:
-    with path.open() as file:
-        return file.read()
```

### Comparing `truss-0.4.9rc5/truss/patch/dir_signature.py` & `truss-0.4.9rc9/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/patch/hash.py` & `truss-0.4.9rc9/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/patch/truss_dir_patch_applier.py` & `truss-0.4.9rc9/truss/patch/truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/patch/types.py` & `truss-0.4.9rc9/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/readme_generator.py` & `truss-0.4.9rc9/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/README.md.jinja` & `truss-0.4.9rc9/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/base.Dockerfile.jinja` & `truss-0.4.9rc9/truss/templates/base.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/application.py` & `truss-0.4.9rc9/truss/templates/control/control/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+import asyncio
 import logging
 import re
 from pathlib import Path
 from typing import Dict
 
+import httpx
 from endpoints import control_app
 from fastapi import FastAPI
 from fastapi.responses import JSONResponse
 from helpers.errors import ModelLoadFailed, PatchApplicatonError
 from helpers.inference_server_controller import InferenceServerController
 from helpers.inference_server_process_controller import InferenceServerProcessController
+from helpers.inference_server_starter import async_inference_server_startup_flow
 from helpers.logging import setup_logging
 from helpers.truss_patch.model_container_patch_applier import ModelContainerPatchApplier
+from starlette.datastructures import State
 
 
 async def handle_patch_error(_, exc):
     error_type = _camel_to_snake_case(type(exc).__name__)
     return JSONResponse(
         content={
             "error": {
@@ -38,54 +42,73 @@
 
 async def handle_model_load_failed(_, error):
     # Model load failures should result in 503 status
     return JSONResponse({"error": str(error)}, 503)
 
 
 def create_app(base_config: Dict):
-    app = FastAPI(
-        title="Truss Live Reload Server",
-        exception_handlers={
-            PatchApplicatonError: handle_patch_error,
-            ModelLoadFailed: handle_model_load_failed,
-            Exception: generic_error_handler,
-        },
-    )
+    app_state = State()
 
     setup_logging()
 
     app_logger = logging.getLogger(__name__)
 
-    app.state.logger = app_logger
+    app_state.logger = app_logger
 
     for k, v in base_config.items():
-        setattr(app.state, k, v)
+        setattr(app_state, k, v)
 
-    app.state.inference_server_process_controller = InferenceServerProcessController(
-        app.state.inference_server_home,
-        app.state.inference_server_process_args,
-        app.state.inference_server_port,
+    app_state.inference_server_process_controller = InferenceServerProcessController(
+        app_state.inference_server_home,
+        app_state.inference_server_process_args,
+        app_state.inference_server_port,
         app_logger=app_logger,
     )
 
-    pip_path = getattr(app.state, "pip_path", None)
+    limits = httpx.Limits(max_keepalive_connections=8, max_connections=32)
+
+    app_state.proxy_client = httpx.AsyncClient(
+        base_url=f"http://localhost:{app_state.inference_server_port}", limits=limits
+    )
+
+    pip_path = getattr(app_state, "pip_path", None)
 
     patch_applier = ModelContainerPatchApplier(
-        Path(app.state.inference_server_home),
+        Path(app_state.inference_server_home),
         app_logger,
         pip_path,
     )
 
-    oversee_inference_server = getattr(app.state, "oversee_inference_server", True)
+    oversee_inference_server = getattr(app_state, "oversee_inference_server", True)
 
-    app.state.inference_server_controller = InferenceServerController(
-        app.state.inference_server_process_controller,
+    app_state.inference_server_controller = InferenceServerController(
+        app_state.inference_server_process_controller,
         patch_applier,
         app_logger,
         oversee_inference_server,
     )
+
+    async def start_background_inference_startup():
+        asyncio.create_task(
+            async_inference_server_startup_flow(
+                app_state.inference_server_controller,
+                app_logger,
+            )
+        )
+
+    app = FastAPI(
+        title="Truss Live Reload Server",
+        on_startup=[start_background_inference_startup],
+        exception_handlers={
+            PatchApplicatonError: handle_patch_error,
+            ModelLoadFailed: handle_model_load_failed,
+            Exception: generic_error_handler,
+        },
+    )
+    app.state = app_state
+
     app.include_router(control_app)
     return app
 
 
 def _camel_to_snake_case(camel_cased: str) -> str:
     return re.sub(r"(?<!^)(?=[A-Z])", "_", camel_cased).lower()
```

### Comparing `truss-0.4.9rc5/truss/templates/control/control/endpoints.py` & `truss-0.4.9rc9/truss/templates/control/control/endpoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 from typing import Any, Dict
 
-import requests
-from fastapi import APIRouter, Request, Response
+from fastapi import APIRouter
 from fastapi.responses import JSONResponse
 from helpers.errors import ModelLoadFailed, ModelNotReady
-from requests.exceptions import ConnectionError
+from httpx import URL, ConnectError
+from starlette.requests import Request
+from starlette.responses import Response
 from tenacity import Retrying, retry_if_exception_type, stop_after_attempt, wait_fixed
 
 INFERENCE_SERVER_START_WAIT_SECS = 60
 
 
 control_app = APIRouter()
 
 
 @control_app.get("/")
 def index():
     return {}
 
 
-@control_app.get("/v1/{full_path:path}")
-@control_app.post("/v1/{full_path:path}")
-async def proxy(full_path: str, request: Request):
-    inference_server_port = request.app.state.inference_server_port
+async def proxy(request: Request):
     inference_server_process_controller = (
         request.app.state.inference_server_process_controller
     )
+    client = request.app.state.proxy_client
+    url = URL(path=request.url.path, query=request.url.query.encode("utf-8"))
+    rp_req = client.build_request(
+        request.method, url, headers=request.headers.raw, content=await request.body()
+    )
 
     # Wait a bit for inference server to start
     for attempt in Retrying(
         retry=(
-            retry_if_exception_type(ConnectionError)
+            retry_if_exception_type(ConnectError)
             | retry_if_exception_type(ModelNotReady)
         ),
         stop=stop_after_attempt(INFERENCE_SERVER_START_WAIT_SECS),
         wait=wait_fixed(1),
     ):
         with attempt:
             try:
                 if (
                     inference_server_process_controller.is_inference_server_intentionally_stopped()
                 ):
                     raise ModelLoadFailed("Model load failed")
+                resp = await client.send(rp_req)
 
-                resp = requests.request(
-                    method=request.method,
-                    url=f"http://localhost:{inference_server_port}/v1/{full_path}",
-                    data=await request.body(),
-                    cookies=request.cookies,
-                    headers=request.headers,
-                )
                 if _is_model_not_ready(resp):
                     raise ModelNotReady("Model has started running, but not ready yet.")
             except ConnectionError as exp:
                 # This check is a bit expensive so we don't do it before every request, we
                 # do it only if request fails with connection error. If the inference server
                 # process is running then we continue waiting for it to start (by retrying),
                 # otherwise we bail.
@@ -65,46 +62,49 @@
                     return JSONResponse(error_msg, 503)
                 raise exp
 
     response = Response(resp.content, resp.status_code, resp.headers)
     return response
 
 
+control_app.add_route("/v1/{path:path}", proxy, ["GET", "POST"])
+
+
 @control_app.post("/control/patch")
 async def patch(request: Request) -> Dict[str, str]:
     request.app.state.logger.info("Patch request received.")
     patch_request = await request.json()
     request.app.state.inference_server_controller.apply_patch(patch_request)
     request.app.state.logger.info("Patch applied successfully")
     return {"msg": "Patch applied successfully"}
 
 
 @control_app.get("/control/truss_hash")
-def truss_hash(request: Request) -> Dict[str, Any]:
+async def truss_hash(request: Request) -> Dict[str, Any]:
     t_hash = request.app.state.inference_server_controller.truss_hash()
     return {"result": t_hash}
 
 
 @control_app.post("/control/restart_inference_server")
-def restart_inference_server(request: Request) -> Dict[str, str]:
+async def restart_inference_server(request: Request) -> Dict[str, str]:
     request.app.state.inference_server_controller.restart()
 
     return {"msg": "Inference server started successfully"}
 
 
 @control_app.get("/control/has_partially_applied_patch")
-def has_partially_applied_patch(request: Request) -> Dict[str, Any]:
+async def has_partially_applied_patch(request: Request) -> Dict[str, Any]:
     app_has_partially_applied_patch = (
         request.app.state.inference_server_controller.has_partially_applied_patch()
     )
     return {"result": app_has_partially_applied_patch}
 
 
 @control_app.post("/control/stop_inference_server")
-def stop_inference_server(request: Request) -> Dict[str, str]:
+async def stop_inference_server(request: Request) -> Dict[str, str]:
     request.app.state.inference_server_controller.stop()
     return {"msg": "Inference server stopped successfully"}
 
 
 def _is_model_not_ready(resp) -> bool:
     return (
         resp.status_code == 503
```

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/errors.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+import asyncio
 import os
+from logging import Logger
 
 import requests
-from fastapi import FastAPI
+from helpers.inference_server_controller import InferenceServerController
 from tenacity import Retrying, stop_after_attempt, wait_exponential
 
 
-def inference_server_startup_flow(application: FastAPI) -> None:
+def inference_server_startup_flow(
+    inference_server_controller: InferenceServerController,
+    logger: Logger,
+) -> None:
     """
     Perform the inference server startup flow
 
     Inference server startup flow supports checking for patches. If a patch ping
     url is provided then we hit that url to start the sync mechanism. The ping
     calls with current truss hash. The patch ping endpoint should return a
     response indicating, either that the supplied hash is current or that the
@@ -21,41 +26,46 @@
 
     The goal is to start the inference server as soon as we have the latest
     code, but not before.
     Example responses:
     {"is_current": true}
     {"accepted": true}
     """
-    inference_server_controller = application.state.inference_server_controller
     patch_ping_url = os.environ.get("PATCH_PING_URL_TRUSS")
     if patch_ping_url is None:
         inference_server_controller.start()
         return
 
     truss_hash = inference_server_controller.truss_hash()
     payload = {"truss_hash": truss_hash}
 
     for attempt in Retrying(
         stop=stop_after_attempt(15),
         wait=wait_exponential(multiplier=2, min=1, max=4),
     ):
         with attempt:
             try:
-                application.state.logger.info(
+                logger.info(
                     f"Pinging {patch_ping_url} for patch with hash {truss_hash}"
                 )
                 resp = requests.post(patch_ping_url, json=payload)
                 resp.raise_for_status()
                 resp_body = resp.json()
 
                 # If hash is current start inference server, otherwise delay that
                 # for when patch is applied.
                 if "is_current" in resp_body and resp_body["is_current"] is True:
-                    application.state.logger.info(
-                        "Hash is current, starting inference server"
-                    )
+                    logger.info("Hash is current, starting inference server")
                     inference_server_controller.start()
             except Exception as exc:  # noqa
-                application.state.logger.warning(
-                    f"Patch ping attempt failed with error {exc}"
-                )
+                logger.warning(f"Patch ping attempt failed with error {exc}")
                 raise exc
+
+
+async def async_inference_server_startup_flow(
+    inference_server_controller: InferenceServerController,
+    logger: Logger,
+) -> None:
+    loop = asyncio.get_event_loop()
+    return await loop.run_in_executor(
+        None, lambda: inference_server_startup_flow(inference_server_controller, logger)
+    )
```

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/logging.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/__init__.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/model_code_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/truss_patch/requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/helpers/types.py` & `truss-0.4.9rc9/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/control/control/server.py` & `truss-0.4.9rc9/truss/templates/control/control/server.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 from pathlib import Path
-from threading import Thread
 
 from application import create_app
-from helpers.inference_server_starter import inference_server_startup_flow
 
 CONTROL_SERVER_PORT = int(os.environ.get("CONTROL_SERVER_PORT", "8080"))
 INFERENCE_SERVER_PORT = int(os.environ.get("INFERENCE_SERVER_PORT", "8090"))
 PYTHON_EXECUTABLE_LOOKUP_PATHS = [
     "/usr/local/bin/python",
     "/usr/local/bin/python3",
     "/usr/bin/python",
@@ -20,41 +18,33 @@
         if Path(path).exists():
             return path
 
     raise RuntimeError("Unable to find python, make sure it's installed.")
 
 
 if __name__ == "__main__":
-    import uvicorn
+    from shared.uvicorn_config import start_uvicorn_server
 
     inf_serv_home: str = os.environ["APP_HOME"]
     python_executable_path: str = _identify_python_executable_path()
     application = create_app(
         {
             "inference_server_home": inf_serv_home,
             "inference_server_process_args": [
                 python_executable_path,
                 f"{inf_serv_home}/inference_server.py",
             ],
-            "control_server_host": "*",
+            "control_server_host": "0.0.0.0",
             "control_server_port": CONTROL_SERVER_PORT,
             "inference_server_port": INFERENCE_SERVER_PORT,
         }
     )
 
-    # Perform inference server startup flow in background
-    Thread(target=inference_server_startup_flow, args=(application,)).start()
-
     application.state.logger.info(
         f"Starting live reload server on port {CONTROL_SERVER_PORT}"
     )
-    uvicorn.run(
+
+    start_uvicorn_server(
         application,
         host=application.state.control_server_host,
         port=application.state.control_server_port,
-        loop="uvloop",
-        reload=False,
-        # TODO(pankaj): change this back to info once things are stable
-        log_level="debug",
-        workers=1,
-        limit_concurrency=32,
     )
```

### Comparing `truss-0.4.9rc5/truss/templates/custom/model/model.py` & `truss-0.4.9rc9/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.9rc9/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/keras/model/model.py` & `truss-0.4.9rc9/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/lightgbm/model/model.py` & `truss-0.4.9rc9/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/mlflow/model/model.py` & `truss-0.4.9rc9/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/pytorch/model/model.py` & `truss-0.4.9rc9/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/errors.py` & `truss-0.4.9rc9/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/logging.py` & `truss-0.4.9rc9/truss/templates/shared/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.4.9rc9/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/patches.py` & `truss-0.4.9rc9/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/retry.py` & `truss-0.4.9rc9/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/serialization.py` & `truss-0.4.9rc9/truss/templates/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/common/util.py` & `truss-0.4.9rc9/truss/templates/shared/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server/inference_server.py` & `truss-0.4.9rc9/truss/templates/server/inference_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from typing import Dict
 
 import yaml
-from common.logging import setup_logging
 from common.truss_server import TrussServer  # noqa: E402
+from shared.logging import setup_logging
 
 CONFIG_FILE = "config.yaml"
 
 setup_logging()
 
 
 class ConfiguredTrussServer:
```

### Comparing `truss-0.4.9rc5/truss/templates/server/model_wrapper.py` & `truss-0.4.9rc9/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/server.Dockerfile.jinja` & `truss-0.4.9rc9/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/shared/secrets_resolver.py` & `truss-0.4.9rc9/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/sklearn/model/model.py` & `truss-0.4.9rc9/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/training/job.py` & `truss-0.4.9rc9/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/templates/xgboost/model/model.py` & `truss-0.4.9rc9/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/auto-mpg.data` & `truss-0.4.9rc9/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/happy.ipynb` & `truss-0.4.9rc9/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/model_load_failure_test/config.yaml` & `truss-0.4.9rc9/truss/test_data/model_load_failure_test/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/model_load_failure_test/model/model.py` & `truss-0.4.9rc9/truss/test_data/model_load_failure_test/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.9rc9/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.9rc9/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/readme_int_example.md` & `truss-0.4.9rc9/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/readme_no_example.md` & `truss-0.4.9rc9/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/readme_str_example.md` & `truss-0.4.9rc9/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/server.Dockerfile` & `truss-0.4.9rc9/truss/test_data/server.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.4.9rc9/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.4.9rc9/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/test_truss/config.yaml` & `truss-0.4.9rc9/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/test_data/test_truss/model/model.py` & `truss-0.4.9rc9/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/conftest.py` & `truss-0.4.9rc9/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.9rc9/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.9rc9/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.9rc9/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.9rc9/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/local/test_local_config_handler.py` & `truss-0.4.9rc9/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.9rc9/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/patch/test_calc_patch.py` & `truss-0.4.9rc9/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/patch/test_hash.py` & `truss-0.4.9rc9/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/patch/test_truss_dir_patch_applier.py` & `truss-0.4.9rc9/truss/tests/patch/test_truss_dir_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/samples.py` & `truss-0.4.9rc9/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py` & `truss-0.4.9rc9/truss/tests/templates/control/control/helpers/test_model_container_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py` & `truss-0.4.9rc9/truss/tests/templates/control/control/helpers/test_requirement_name_identifier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/control/control/test_server.py` & `truss-0.4.9rc9/truss/tests/templates/control/control/test_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import os
 import sys
 from contextlib import contextmanager
 from pathlib import Path
 from typing import Dict, List
 
 import pytest
-from fastapi.testclient import TestClient
+from httpx import AsyncClient
+from truss.types import PatchRequest
 
 # Needed to simulate the set up on the model docker container
 sys.path.append(
     str(
         Path(__file__).parent.parent.parent.parent.parent
         / "templates"
         / "control"
         / "control"
     )
 )
 
+sys.path.append(
+    str(Path(__file__).parent.parent.parent.parent.parent / "templates" / "shared")
+)
+
 from truss.templates.control.control.application import create_app  # noqa
 from truss.templates.control.control.helpers.types import (  # noqa
     Action,
     ModelCodePatch,
     Patch,
     PatchType,
     PythonRequirementPatch,
@@ -51,53 +56,67 @@
         try:
             inference_server_controller.start()
             yield control_app
         finally:
             inference_server_controller.stop()
 
 
+@pytest.fixture(
+    params=[
+        pytest.param(("asyncio", {"use_uvloop": True}), id="asyncio+uvloop"),
+        pytest.param(("asyncio", {"use_uvloop": False}), id="asyncio"),
+    ]
+)
+def anyio_backend(request):
+    return request.param
+
+
 @pytest.fixture()
-def client(app):
-    return TestClient(app)
+async def client(app):
+    async with AsyncClient(app=app, base_url="http://localhost:8080") as async_client:
+        yield async_client
 
 
-def test_restart_server(client):
-    resp = client.post("/control/stop_inference_server")
+@pytest.mark.anyio
+async def test_restart_server(client):
+    resp = await client.post("/control/stop_inference_server")
     assert resp.status_code == 200
     assert "error" not in resp.json()
     assert "msg" in resp.json()
 
     # Try second restart
-    resp = client.post("/control/stop_inference_server")
+    resp = await client.post("/control/stop_inference_server")
     assert resp.status_code == 200
     assert "error" not in resp.json()
     assert "msg" in resp.json()
 
 
-def test_patch_model_code_update_existing(app, client):
+@pytest.mark.anyio
+async def test_patch_model_code_update_existing(app, client):
     mock_model_file_content = """
 class Model:
     def predict(self, request):
         return {'prediction': [1]}
 """
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="model.py",
             content=mock_model_file_content,
         ),
     )
-    _verify_apply_patch_success(client, patch)
+    await _verify_apply_patch_success(client, patch)
     with (app.state.inference_server_home / "model" / "model.py").open() as model_file:
         new_model_file_content = model_file.read()
     assert new_model_file_content == mock_model_file_content
 
 
-def test_patch_model_code_update_predict_on_long_load_time(app, client):
+@pytest.mark.anyio
+async def test_patch_model_code_update_predict_on_long_load_time(app, client):
     mock_model_file_content = """
 class Model:
     def load(self):
         import time
         time.sleep(3)
 
     def predict(self, request):
@@ -107,133 +126,117 @@
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="model.py",
             content=mock_model_file_content,
         ),
     )
-    _verify_apply_patch_success(client, patch)
-    resp = client.post("/v1/models/model:predict", json={})
+    await _verify_apply_patch_success(client, patch)
+    resp = await client.post("/v1/models/model:predict", json={})
     resp.status_code == 200
     assert resp.json() == {"prediction": [1]}
 
 
-def test_patch_model_code_create_new(app, client):
+@pytest.mark.anyio
+async def test_patch_model_code_create_new(app, client):
     empty_content = ""
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="touched",
             content=empty_content,
         ),
     )
-    _verify_apply_patch_success(client, patch)
+    await _verify_apply_patch_success(client, patch)
     assert (app.state.inference_server_home / "model" / "touched").exists()
 
 
-def test_patch_model_code_create_in_new_dir(app, client):
+@pytest.mark.anyio
+async def test_patch_model_code_create_in_new_dir(app, client):
     empty_content = ""
     patch = Patch(
         type=PatchType.MODEL_CODE,
         body=ModelCodePatch(
             action=Action.UPDATE,
             path="new_directory/touched",
             content=empty_content,
         ),
     )
-    _verify_apply_patch_success(client, patch)
+    await _verify_apply_patch_success(client, patch)
     assert (
         app.state.inference_server_home / "model" / "new_directory" / "touched"
     ).exists()
 
 
-def test_404(client):
-    resp = client.post("/control/nonexitant")
+@pytest.mark.anyio
+async def test_404(client):
+    resp = await client.post("/control/nonexitant")
     assert resp.status_code == 404
 
 
-def test_invalid_patch(client):
-    patch_request = {
-        "hash": "dummy",
-        "prev_hash": "invalid",
-        "patches": [],
-    }
-    resp = client.post("/control/patch", json=patch_request)
+@pytest.mark.anyio
+async def test_invalid_patch(client):
+    patch_request = PatchRequest(hash="dummy", prev_hash="invalid", patches=[])
+    resp = await client.post("/control/patch", json=patch_request.to_dict())
     assert resp.status_code == 200
     assert "error" in resp.json()
     assert resp.json()["error"]["type"] == "inadmissible_patch"
     assert "msg" not in resp.json()
 
 
-def test_unsupported_patch(client):
-    unsupported_patch = {
-        "type": "unsupported",
-        "body": {},
-    }
-    resp = _apply_patches(client, [unsupported_patch])
-    assert resp.status_code == 200
-    assert "error" in resp.json()
-    assert resp.json()["error"]["type"] == "unsupported_patch"
-
-
-def test_patch_failed_recoverable(client):
+@pytest.mark.anyio
+async def test_patch_failed_recoverable(client):
     will_fail_patch = Patch(
         type=PatchType.PYTHON_REQUIREMENT,
         body=PythonRequirementPatch(
             action=Action.ADD, requirement="not_a_valid_python_requirement"
         ),
     )
-    resp = _apply_patches(client, [will_fail_patch.to_dict()])
+    resp = await _apply_patches(client, [will_fail_patch])
     assert resp.status_code == 200
     assert "error" in resp.json()
     assert resp.json()["error"]["type"] == "patch_failed_recoverable"
 
 
-def test_patch_failed_unrecoverable(client):
+@pytest.mark.anyio
+async def test_patch_failed_unrecoverable(client):
     will_pass_patch = Patch(
         type=PatchType.PYTHON_REQUIREMENT,
         body=PythonRequirementPatch(action=Action.ADD, requirement="requests"),
     )
     will_fail_patch = Patch(
         type=PatchType.PYTHON_REQUIREMENT,
         body=PythonRequirementPatch(
             action=Action.ADD, requirement="not_a_valid_python_requirement"
         ),
     )
-    resp = _apply_patches(
-        client, [will_pass_patch.to_dict(), will_fail_patch.to_dict()]
-    )
+    resp = await _apply_patches(client, [will_pass_patch, will_fail_patch])
     assert resp.status_code == 200
     assert "error" in resp.json()
     assert resp.json()["error"]["type"] == "patch_failed_unrecoverable"
 
 
-def _verify_apply_patch_success(client, patch: Patch):
-    original_hash = client.get("/control/truss_hash").json()["result"]
-    patch_request = {
-        "hash": "dummy",
-        "prev_hash": original_hash,
-        "patches": [patch.to_dict()],
-    }
-    resp = client.post("/control/patch", json=patch_request)
-    resp = _apply_patches(client, [patch.to_dict()])
+async def _verify_apply_patch_success(client, patch: Patch):
+    resp = await client.get("/control/truss_hash")
+    original_hash = resp.json()["result"]
+    print(f"ORIGINAL HASH: {original_hash}")
+    patch_request = PatchRequest(hash="dummy", prev_hash=original_hash, patches=[patch])
+    resp = await client.post("/control/patch", json=patch_request.to_dict())
+    resp = await _apply_patches(client, [patch])
     assert resp.status_code == 200
     assert "error" not in resp.json()
     assert "msg" in resp.json()
 
 
-def _apply_patches(client, patches: List[dict]):
-    original_hash = client.get("/control/truss_hash").json()["result"]
-    patch_request = {
-        "hash": "dummy",
-        "prev_hash": original_hash,
-        "patches": patches,
-    }
-    return client.post("/control/patch", json=patch_request)
+async def _apply_patches(client, patches: List[Patch]):
+    resp = await client.get("/control/truss_hash")
+    original_hash = resp.json()["result"]
+    patch_request = PatchRequest(hash="dummy", prev_hash=original_hash, patches=patches)
+    return await client.post("/control/patch", json=patch_request.to_dict())
 
 
 @contextmanager
 def _env_var(kvs: Dict[str, str]):
     orig_env = os.environ.copy()
     try:
         os.environ.update(kvs)
```

### Comparing `truss-0.4.9rc5/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.9rc9/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.9rc9/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.9rc9/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.9rc9/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_backward.py` & `truss-0.4.9rc9/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_build.py` & `truss-0.4.9rc9/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_config.py` & `truss-0.4.9rc9/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_context_builder_image.py` & `truss-0.4.9rc9/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_docker.py` & `truss-0.4.9rc9/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_model_inference.py` & `truss-0.4.9rc9/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_notebooks.py` & `truss-0.4.9rc9/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.9rc9/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_truss_gatherer.py` & `truss-0.4.9rc9/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/tests/test_truss_handle.py` & `truss-0.4.9rc9/truss/tests/test_truss_handle.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     PatchType,
 )
 from truss.tests.test_testing_utilities_for_other_tests import (
     ensure_kill_all,
     kill_all_with_retries,
 )
 from truss.truss_handle import TrussHandle, wait_for_truss
-from truss.types import Example
+from truss.types import Example, PatchRequest
 
 
 def test_spec(custom_model_truss_dir_with_pre_and_post):
     dir_path = custom_model_truss_dir_with_pre_and_post
     th = TrussHandle(dir_path)
     spec = th.spec
     assert spec.truss_dir == dir_path
@@ -128,26 +128,17 @@
     )
     th.build_training_docker_image()
 
 
 @pytest.mark.integration
 def test_docker_predict_custom_base_image(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
-    th.set_base_image("pytorch/pytorch", "/opt/conda/bin/python")
-    with ensure_kill_all():
-        result = th.docker_predict([1, 2])
-        assert result == {"predictions": [4, 5]}
-
-
-@pytest.mark.integration
-def test_docker_predict_custom_base_image_with_python_executable_path(
-    custom_model_truss_dir_with_pre_and_post,
-):
-    th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
-    th.set_base_image("pytorch/pytorch", "/opt/conda/bin/python")
+    th.set_base_image(
+        "wallies/python-cuda:3.10-cuda11.7-runtime", "/usr/local/bin/python"
+    )
     with ensure_kill_all():
         result = th.docker_predict([1, 2])
         assert result == {"predictions": [4, 5]}
 
 
 @pytest.mark.integration
 def test_build_docker_image_gpu(custom_model_truss_dir_for_gpu, tmp_path):
@@ -204,15 +195,15 @@
 @pytest.mark.integration
 def get_docker_containers_from_labels(custom_model_truss_dir_with_pre_and_post):
     with ensure_kill_all():
         t1 = TrussHandle(custom_model_truss_dir_with_pre_and_post)
         assert len(t1.get_serving_docker_containers_from_labels()) == 0
         t1.docker_run()
         assert len(t1.get_serving_docker_containers_from_labels()) == 1
-        t1.docker_run(port=3000)
+        t1.docker_run(local_port=3000)
         assert len(t1.get_serving_docker_containers_from_labels()) == 2
         t1.kill_container()
         assert len(t1.get_serving_docker_containers_from_labels()) == 0
 
 
 @pytest.mark.integration
 def test_predict_use_docker(custom_model_truss_dir_with_pre_and_post):
@@ -413,30 +404,30 @@
 def test_custom_python_requirement(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     th.add_python_requirement("theano")
     th.add_python_requirement("scipy")
     tag = "test-custom-python-req-tag:0.0.1"
     container = th.docker_run(tag=tag)
     try:
-        _verify_python_requirement_installed_on_container(container, "theano")
-        _verify_python_requirement_installed_on_container(container, "scipy")
+        verify_python_requirement_installed_on_container(container, "theano")
+        verify_python_requirement_installed_on_container(container, "scipy")
     finally:
         Docker.client().kill(container)
 
 
 @pytest.mark.integration
 def test_custom_system_package(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     th.add_system_package("jq")
     th.add_system_package("fzf")
     tag = "test-custom-system-package-tag:0.0.1"
     container = th.docker_run(tag=tag)
     try:
-        _verify_system_package_installed_on_container(container, "jq")
-        _verify_system_package_installed_on_container(container, "fzf")
+        verify_system_package_installed_on_container(container, "jq")
+        verify_system_package_installed_on_container(container, "fzf")
     finally:
         Docker.client().kill(container)
 
 
 def test_enable_gpu(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     th.enable_gpu()
@@ -497,15 +488,15 @@
 @pytest.mark.integration
 def test_add_environment_variable(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     th.add_environment_variable("test_env", "test_value")
     tag = "test-add-env-var-tag:0.0.1"
     container = th.docker_run(tag=tag)
     try:
-        _verify_environment_variable_on_container(container, "test_env", "test_value")
+        verify_environment_variable_on_container(container, "test_env", "test_value")
     finally:
         Docker.client().kill(container)
 
 
 def test_add_data_file(custom_model_truss_dir_with_pre_and_post, tmp_path):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     data_filepath = tmp_path / "test_data.txt"
@@ -607,28 +598,28 @@
 
         running_hash = th.truss_hash_on_serving_container()
         new_model_code = """
 class Model:
     def predict(self, model_input):
         return [2 for i in model_input]
 """
-        patch_request = {
-            "hash": "dummy",
-            "prev_hash": running_hash,
-            "patches": [
+        patch_request = PatchRequest(
+            hash="dummy",
+            prev_hash=running_hash,
+            patches=[
                 Patch(
                     type=PatchType.MODEL_CODE,
                     body=ModelCodePatch(
                         action=Action.UPDATE,
                         path="model.py",
                         content=new_model_code,
                     ),
-                ).to_dict(),
+                ),
             ],
-        }
+        )
 
         th.patch_container(patch_request)
         result = th.docker_predict([1], tag=tag)
         assert result[0] == 2
 
 
 @pytest.mark.integration
@@ -691,124 +682,14 @@
 def test_container_stuck_in_created(container_state_mock):
     container_state_mock.return_value = DockerStates.CREATED
     with pytest.raises(ContainerIsDownError):
         wait_for_truss(url="localhost:8000", container=MagicMock())
 
 
 @pytest.mark.integration
-@pytest.mark.parametrize(
-    "binary, python_version",
-    [
-        (binary, python_version)
-        for binary in [True, False]
-        for python_version in ["3.8", "3.9"]
-    ],
-)
-def test_control_truss_local_update_flow(binary, python_version, custom_model_control):
-    th = TrussHandle(custom_model_control)
-    th.update_python_version(python_version)
-    tag = "test-docker-custom-model-control-tag:0.0.1"
-
-    def predict_with_updated_model_code():
-        new_model_code = """
-class Model:
-    def predict(self, model_input):
-        return [2 for i in model_input]
-"""
-        model_code_file_path = custom_model_control / "model" / "model.py"
-        with model_code_file_path.open("w") as model_code_file:
-            model_code_file.write(new_model_code)
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_added_empty_directory():
-        # Adding empty directory should work
-        (custom_model_control / "model" / "dir").mkdir()
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_unpatchable_change():
-        # Changes that are not expressible with patch should also work
-        # Changes to data dir are not currently patch expressible
-        (custom_model_control / "data" / "dummy").touch()
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_python_requirement_added(req: str):
-        th.add_python_requirement(req)
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_python_requirement_removed(req):
-        th.remove_python_requirement(req)
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_system_requirement_added(pkg):
-        th.add_system_package(pkg)
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_system_requirement_removed(pkg):
-        th.remove_system_package(pkg)
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def predict_with_ignored_changes():
-        top_pycache_path = custom_model_control / "__pycache__"
-        top_pycache_path.mkdir()
-        (top_pycache_path / "bla.pyc").touch()
-        model_pycache_path = custom_model_control / "model" / "__pycache__"
-        model_pycache_path.mkdir()
-        (model_pycache_path / "foo.pyc").touch()
-        return th.docker_predict([1], tag=tag, binary=binary)
-
-    def current_num_docker_images() -> int:
-        return len(th.get_all_docker_images())
-
-    with ensure_kill_all():
-        result = th.docker_predict([1], tag=tag, binary=binary)
-        assert result[0] == 1
-        orig_num_truss_images = len(th.get_all_docker_images())
-
-        result = predict_with_updated_model_code()
-        assert result[0] == 2
-        assert orig_num_truss_images == current_num_docker_images()
-
-        result = predict_with_added_empty_directory()
-        assert result[0] == 2
-        assert orig_num_truss_images == current_num_docker_images()
-
-        container = th._get_running_serving_container_ignore_hash()
-
-        python_req = "pydot"
-        result = predict_with_python_requirement_added(python_req)
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images
-        _verify_python_requirement_installed_on_container(container, python_req)
-
-        result = predict_with_python_requirement_removed(python_req)
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images
-        _verify_python_requirement_not_installed_on_container(container, python_req)
-
-        system_pkg = "jq"
-        result = predict_with_system_requirement_added(system_pkg)
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images
-        _verify_system_package_installed_on_container(container, system_pkg)
-
-        result = predict_with_system_requirement_removed(system_pkg)
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images
-        _verify_system_requirement_not_installed_on_container(container, system_pkg)
-
-        result = predict_with_unpatchable_change()
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images + 1
-
-        result = predict_with_ignored_changes()
-        assert result[0] == 2
-        assert current_num_docker_images() == orig_num_truss_images + 1
-
-
-@pytest.mark.integration
 def test_control_truss_huggingface(
     huggingface_truss_handle_small_model,
 ):
     th = TrussHandle(huggingface_truss_handle_small_model)
     th.live_reload()
     tag = "test-docker-huggingface-model-control-tag:0.0.1"
     with ensure_kill_all():
@@ -920,39 +801,39 @@
 def _container_exists(container) -> bool:
     for row in Docker.client().ps():
         if row.id.startswith(container.id):
             return True
     return False
 
 
-def _verify_system_package_installed_on_container(container, pkg: str):
+def verify_system_package_installed_on_container(container, pkg: str):
     resp = container.execute(["which", pkg])
     assert resp.strip() == f"/usr/bin/{pkg}"
 
 
-def _verify_system_requirement_not_installed_on_container(container, pkg: str):
+def verify_system_requirement_not_installed_on_container(container, pkg: str):
     try:
         container.execute(["dpkg", "-l", pkg])
     except DockerException as excp:
         assert "no packages found" in str(excp)
 
 
-def _verify_python_requirement_installed_on_container(container, req: str):
+def verify_python_requirement_installed_on_container(container, req: str):
     resp = container.execute(["pip", "show", req])
     assert resp.splitlines()[0].lower() == f"Name: {req}".lower()
 
 
-def _verify_python_requirement_not_installed_on_container(container, req: str):
+def verify_python_requirement_not_installed_on_container(container, req: str):
     try:
         container.execute(["pip", "show", req])
     except DockerException as excp:
         assert "not found" in str(excp)
 
 
-def _verify_environment_variable_on_container(
+def verify_environment_variable_on_container(
     container,
     env_var_name: str,
     env_var_value: str,
 ):
     resp = container.execute(["env"])
     needle = f"{env_var_name}={env_var_value}"
     assert needle in resp.splitlines()
```

### Comparing `truss-0.4.9rc5/truss/tests/test_validation.py` & `truss-0.4.9rc9/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/truss_config.py` & `truss-0.4.9rc9/truss/truss_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/truss_gatherer.py` & `truss-0.4.9rc9/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/truss_handle.py` & `truss-0.4.9rc9/truss/truss_handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,21 @@
 from truss.local.local_config_handler import LocalConfigHandler
 from truss.notebook import is_notebook_or_ipython
 from truss.patch.calc_patch import calc_truss_patch
 from truss.patch.hash import directory_content_hash
 from truss.patch.signature import calc_truss_signature
 from truss.patch.types import TrussSignature
 from truss.readme_generator import generate_readme
-from truss.templates.server.common.serialization import (
+from truss.templates.shared.serialization import (
     truss_msgpack_deserialize,
     truss_msgpack_serialize,
 )
 from truss.truss_config import BaseImage, ExternalData, ExternalDataItem, TrussConfig
 from truss.truss_spec import TrussSpec
-from truss.types import Example, PatchDetails
+from truss.types import Example, PatchDetails, PatchRequest
 from truss.util.path import copy_file_path, copy_tree_path, get_max_modified_time_of_dir
 from truss.validation import validate_secret_name
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 if is_notebook_or_ipython():
     logger.setLevel(logging.INFO)
@@ -447,14 +447,18 @@
                 environment_variables={
                     **conf.environment_variables,
                     env_var_name: env_var_value,
                 },
             )
         )
 
+    def clear_environment_variables(self):
+        """Remove environment variables from truss model's config."""
+        self._update_config(lambda conf: replace(conf, environment_variables={}))
+
     def add_secret(self, secret_name: str, default_secret_value: str = ""):
         validate_secret_name(secret_name)
         self._update_config(
             lambda conf: replace(
                 conf,
                 secrets={
                     **conf.secrets,
@@ -658,15 +662,15 @@
                 TRUSS: True,
                 TRAINING_LABEL: False,
                 **labels,
             }
 
         return sorted(get_containers(labels, all=all), key=lambda c: c.created)
 
-    def _get_running_serving_container_ignore_hash(self):
+    def get_running_serving_container_ignore_hash(self):
         containers = self.get_serving_docker_containers_from_labels(
             labels={TRUSS_DIR: str(self._truss_dir)}
         )
         if containers is not None and len(containers) > 0:
             return containers[0]
 
     @proxy_to_shadow_if_scattered
@@ -722,32 +726,33 @@
                 python_executable_path,
             )
             return replace(conf, base_image=new_base_image)
 
         self._update_config(define_base_image_fn)
 
     @proxy_to_shadow_if_scattered
-    def patch_container(self, patch_request: Dict):
+    def patch_container(self, patch_request: PatchRequest):
         """Patch changes onto the container running this Truss.
 
         Useful for local incremental development.
-        TODO(pankaj): Turn patch_request into a dataclass
         """
         if not self.spec.live_reload:
             raise ValueError("Not a control truss: applying patch is not supported.")
 
         # Note that we match on only the truss directory, not hash.
-        container = self._get_running_serving_container_ignore_hash()
+        container = self.get_running_serving_container_ignore_hash()
         if not container:
             raise ValueError(
                 "Only running trusses can be patched: no running containers found for this truss."
             )
 
         model_base_url = _get_url_from_container(container)
-        resp = requests.post(f"{model_base_url}/control/patch", json=patch_request)
+        resp = requests.post(
+            f"{model_base_url}/control/patch", json=patch_request.to_dict()
+        )
         resp.raise_for_status()
         return resp.json()
 
     def truss_hash_on_container(self) -> Optional[str]:
         """[Deprecated] Use truss_hash_on_serving_container."""
         return self.truss_hash_on_serving_container()
 
@@ -755,15 +760,15 @@
     def truss_hash_on_serving_container(self) -> Optional[str]:
         """Get content hash of truss running on container."""
         if not self.spec.live_reload:
             raise ValueError(
                 "Not a control truss fetching truss hash is not supported."
             )
 
-        container = self._get_running_serving_container_ignore_hash()
+        container = self.get_running_serving_container_ignore_hash()
         model_base_url = _get_url_from_container(container)
         resp = requests.get(f"{model_base_url}/control/truss_hash")
         resp.raise_for_status()
         respj = resp.json()
         if "error" in respj:
             logger.error("Unable to get hash of running container.")
             return None
@@ -784,15 +789,15 @@
         )
 
     def _control_serving_container_has_partially_applied_patch(self) -> Optional[bool]:
         """Check if there is a partially applied patch on the running live_reload capable container."""
         if not self.spec.live_reload:
             raise ValueError("Not a control truss, operation not supported.")
 
-        container = self._get_running_serving_container_ignore_hash()
+        container = self.get_running_serving_container_ignore_hash()
         model_base_url = _get_url_from_container(container)
         resp = requests.get(f"{model_base_url}/control/has_partially_applied_patch")
         resp.raise_for_status()
         respj = resp.json()
         if "error" in respj:
             logger.error(
                 "Unable to check if control truss container has partially applied patch."
@@ -975,15 +980,15 @@
         # reload spec
         self._spec = TrussSpec(self._truss_dir)
 
     def _try_patch(self):
         if not self.is_control_truss:
             return None
 
-        container = self._get_running_serving_container_ignore_hash()
+        container = self.get_running_serving_container_ignore_hash()
         if container is None:
             return None
 
         running_truss_hash = self.truss_hash_on_serving_container()
         if running_truss_hash is None:
             return None
 
@@ -1009,19 +1014,19 @@
         if patch_details.is_empty():
             logger.info(
                 "While truss has changed, no serving related "
                 "changes were found, skipping patching."
             )
             return container
 
-        patch_request = {
-            "hash": current_hash,
-            "prev_hash": running_truss_hash,
-            "patches": [patch.to_dict() for patch in patch_details.patch_ops],
-        }
+        patch_request = PatchRequest(
+            hash=current_hash,
+            prev_hash=running_truss_hash,
+            patches=patch_details.patch_ops,
+        )
         resp = self.patch_container(patch_request)
         if "error" in resp:
             raise RuntimeError(f'Failed to patch control truss {resp["error"]}')
         self._store_signature()
         return container
 
     def _serving_hash(self) -> str:
```

### Comparing `truss-0.4.9rc5/truss/truss_spec.py` & `truss-0.4.9rc9/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/types.py` & `truss-0.4.9rc9/truss/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, List
 
+from pydantic import BaseModel
 from truss.patch.types import TrussSignature
 from truss.templates.control.control.helpers.types import Patch
 
 
 class ModelFrameworkType(Enum):
     SKLEARN = "sklearn"
     TENSORFLOW = "tensorflow"
@@ -67,7 +68,29 @@
             prev_signature=TrussSignature.from_dict(patch_details["prev_signature"]),
             next_hash=patch_details["next_hash"],
             next_signature=TrussSignature.from_dict(patch_details["next_signature"]),
             patch_ops=[
                 Patch.from_dict(patch_op) for patch_op in patch_details["patch_ops"]
             ],
         )
+
+
+class PatchRequest(BaseModel):
+    """Request to patch running container"""
+
+    hash: str
+    prev_hash: str
+    patches: List[Patch]
+
+    def to_dict(self):
+        return {
+            "hash": self.hash,
+            "prev_hash": self.prev_hash,
+            "patches": [patch.to_dict() for patch in self.patches],
+        }
+
+    @staticmethod
+    def from_dict(patch_request_dict: Dict):
+        current_hash = patch_request_dict["hash"]
+        prev_hash = patch_request_dict["prev_hash"]
+        patches = patch_request_dict["patches"]
+        return PatchRequest(hash=current_hash, prev_hash=prev_hash, patches=patches)
```

### Comparing `truss-0.4.9rc5/truss/util/gpu.py` & `truss-0.4.9rc9/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/util/path.py` & `truss-0.4.9rc9/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/truss/validation.py` & `truss-0.4.9rc9/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.9rc5/PKG-INFO` & `truss-0.4.9rc9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.9rc5
+Version: 0.4.9rc9
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
@@ -14,30 +14,28 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
-Requires-Dist: dockerfile (>=3.2.0,<4.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.2)
 Requires-Dist: msgpack-numpy (>=0.4.7.1)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: packaging (>=20.9,<21.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: python-json-logger (>=2.0.2)
 Requires-Dist: python-on-whales (>=0.46.0,<0.47.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
-Requires-Dist: virtualenv (>=20.23.0,<21.0.0)
-Requires-Dist: watchfiles (>=0.19.0,<0.20.0)
-Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Project-URL: Bug Reports, https://github.com/basetenlabs/truss/issues
 Project-URL: Baseten, https://baseten.co
 Project-URL: Documentation, https://truss.baseten.co
 Project-URL: Homepage, https://truss.baseten.co
 Project-URL: Repository, https://github.com/basetenlabs/truss
 Description-Content-Type: text/markdown
```

