# Comparing `tmp/servicefoundry-0.9.9rc1.tar.gz` & `tmp/servicefoundry-0.9.9rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.9rc1.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.9rc2.tar", max compression
```

## Comparing `servicefoundry-0.9.9rc1.tar` & `servicefoundry-0.9.9rc2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0      672 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/README.md
--rw-r--r--   0        0        0     2119 2023-06-28 07:32:02.656684 servicefoundry-0.9.9rc1/pyproject.toml
--rw-r--r--   0        0        0     1365 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/__init__.py
--rw-r--r--   0        0        0    40410 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1506 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6381 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     7019 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1232 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     3536 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     4462 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0     1012 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     4134 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2970 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/json_util.py
--rw-r--r--   0        0        0     4513 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/langchain.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-28 07:31:51.812665 servicefoundry-0.9.9rc1/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    25229 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1292 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0    10866 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5921 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8988 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-06-28 07:31:51.816665 servicefoundry-0.9.9rc1/servicefoundry/version.py
--rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.9rc1/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/README.md
+-rw-r--r--   0        0        0     2119 2023-06-30 10:23:39.214676 servicefoundry-0.9.9rc2/pyproject.toml
+-rw-r--r--   0        0        0     1431 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    44796 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1506 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6381 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     7019 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     3536 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     4462 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0     1012 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     4134 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2970 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.766660 servicefoundry-0.9.9rc2/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/json_util.py
+-rw-r--r--   0        0        0     4513 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/langchain.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    25229 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1292 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0    10866 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     2208 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     6353 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8988 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-06-30 10:23:26.770660 servicefoundry-0.9.9rc2/servicefoundry/version.py
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.9rc2/PKG-INFO
```

### Comparing `servicefoundry-0.9.9rc1/README.md` & `servicefoundry-0.9.9rc2/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/pyproject.toml` & `servicefoundry-0.9.9rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.9rc1"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.9rc2"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     list_workspaces,
 )
 from servicefoundry.v2.lib.deployable_patched_models import (
     Application,
     Job,
     ModelDeployment,
     Service,
+    Notebook,
 )
 from servicefoundry.v2.lib.patched_models import (
     Autoscaling,
     BasicAuthCreds,
     BlueGreen,
     Build,
     CPUUtilizationMetric,
@@ -58,9 +59,11 @@
     SecretMount,
     StringDataMount,
     VolumeMount,
     TruefoundryModelRegistry,
     NodepoolSelector,
     NodeSelector,
     Endpoint,
+    TruefoundryImageFull,
+    TruefoundryImageBase,
 )
 from servicefoundry.version import __version__
```

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.9rc2/servicefoundry/auto_gen/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-06-15T07:25:29+00:00
+#   timestamp: 2023-06-30T10:08:10+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, PositiveInt, confloat, conint, constr
@@ -448,19 +448,19 @@
         200,
         description="+label=Memory Request\n+usage=Requested memory which determines the minimum cost incurred. The unit of memory is in megabytes(MB).\nSo 1 means 1 MB and 2000 means 2GB.\n+sort=3",
     )
     memory_limit: conint(ge=1, le=2000000) = Field(
         500,
         description="+label=Memory Limit\n+usage=Memory limit after which the application will be killed with an OOM error. The unit of memory is\nin megabytes(MB). So 1 means 1 MB and 2000 means 2GB. MemoryLimit should be greater than memory request.\n+sort=4",
     )
-    ephemeral_storage_request: conint(ge=1, le=500000) = Field(
+    ephemeral_storage_request: conint(ge=1, le=2000000) = Field(
         1000,
         description="+label=Storage Request\n+usage=Requested disk storage. The unit of memory is in megabytes(MB).\nThis is ephemeral storage and will be wiped out on pod restarts or eviction\n+sort=5",
     )
-    ephemeral_storage_limit: conint(ge=1, le=500000) = Field(
+    ephemeral_storage_limit: conint(ge=1, le=2000000) = Field(
         2000,
         description="+label=Storage Limit\n+usage=Disk storage limit. The unit of memory is in megabytes(MB). Exceeding this limit will result in eviction.\nIt should be greater than the request. This is ephemeral storage and will be wiped out on pod restarts or eviction\n+sort=6",
     )
     gpu_count: conint(ge=0, le=16) = Field(
         0,
         description="+label=GPU Count\n+usage=Count of GPUs to provide to the application\nNote the exact count and max count available for a given GPU type depends on cloud provider and cluster type.",
     )
@@ -550,14 +550,54 @@
     mount_path: constr(regex=r"^\/(?:[^/\n]+\/*)*[^/\n]+(\.[^/\n]+)?$") = Field(
         ...,
         description="+label=File Path\n+usage=Absolute file path where the file will be created.\n+message=Please enter a valid file path",
     )
     data: str = Field(..., description="+label=Data\n+usage=The file content.")
 
 
+class TruefoundryImageBase(BaseModel):
+    """
+    +usage=JupyterLab with persistent python environment (Python 3.8.10)
+    """
+
+    type: Literal["truefoundrybase"] = Field(..., description="+value=truefoundrybase")
+    enable_sudo: bool = Field(
+        False,
+        description="+label=Enable Root Access\n+usage=Enable root access to the container\n> Note: Changes made to the root directory `/` will not be persisted across notebook restarts",
+    )
+    apt_packages: Optional[List[str]] = Field(
+        None,
+        description='+label=List of Debian packages to install.\n+usage=Debian packages to install via `apt get`.\nIn Python/YAML E.g. ["git", "ffmpeg", "htop"]\n+placeholder=Enter a debian package name E.g. ffmpeg',
+    )
+    docker_registry: Optional[str] = Field(
+        None,
+        description="+docs=FQN of the container registry. You can the FQN of your desired container registry (or add one)\nin the  Integrations page[Integrations](https://app.truefoundry.tech/integrations?tab=docker-registry) page\n+label=Docker Registry\n+usage=FQN of the container registry. If you can't find your registry here,\nadd it through the [Integrations](/integrations?tab=docker-registry) page",
+    )
+
+
+class TruefoundryImageFull(BaseModel):
+    """
+    +usage=JupyterLab + All Common ML Libraries with persistent environment (Python 3.8.10)
+    """
+
+    type: Literal["truefoundryfull"] = Field(..., description="+value=truefoundryfull")
+    enable_sudo: bool = Field(
+        False,
+        description="+label=Enable Root Access\n> Note: Changes made to the root directory `/` will not be persisted across notebook restarts",
+    )
+    apt_packages: Optional[List[str]] = Field(
+        None,
+        description='+label=List of Debian packages to install.\n+usage=Debian packages to install via `apt get`.\nIn Python/YAML E.g. ["git", "ffmpeg", "htop"]\n+placeholder=Enter a debian package name E.g. ffmpeg',
+    )
+    docker_registry: Optional[str] = Field(
+        None,
+        description="+docs=FQN of the container registry. You can the FQN of your desired container registry (or add one)\nin the  Integrations page[Integrations](https://app.truefoundry.tech/integrations?tab=docker-registry) page\n+label=Docker Registry\n+usage=FQN of the container registry. If you can't find your registry here,\nadd it through the [Integrations](/integrations?tab=docker-registry) page",
+    )
+
+
 class TruefoundryModelRegistry(BaseModel):
     """
     +docs=Truefoundry model registry (deploy a model from TFY model registry)
     +label=Truefoundry model registry
     +usage=Deploy a model from TFY model registry
     """
 
@@ -744,14 +784,51 @@
         description="+usage=Configure data to be mounted to model pod(s)\n+ignore\n+sort=10011",
     )
     labels: Optional[Dict[str, str]] = Field(
         None, description="+label=Labels\n+usage=Add labels to service metadata"
     )
 
 
+class Notebook(BaseModel):
+    """
+    +docs=Describes the configuration for the service
+    """
+
+    type: constr(regex=r"^notebook$") = Field(..., description="+value=notebook")
+    name: constr(regex=r"^[a-z][a-z0-9\-]{1,23}[a-z0-9]$") = Field(
+        ...,
+        description="+usage=Name of the notebook. This uniquely identifies this notebook in the workspace.\n> Name can only contain alphanumeric characters and '-' and can be atmost 25 characters long\n+sort=1\n+message=3 to 25 lower case characters long alphanumeric word, may contain - in between, cannot start with a number",
+    )
+    image: Union[TruefoundryImageBase, TruefoundryImageFull] = Field(
+        ..., description="+usage=Pick a notebook image to deploy\n+sort=2"
+    )
+    endpoint: Endpoint
+    auth: Optional[BasicAuthCreds] = None
+    cull_timeout: conint(ge=5) = Field(
+        30,
+        description="+usage=Stop the notebook instance after this much time in minutes of inactivity.\nThe notebook instance will be stopped even if the notebook is open in your browser, but nothing is running on the notebook.\n+sort=5\n+label=Stop after (minutes of inactivity)",
+    )
+    resources: Optional[Resources] = None
+    home_directory_size: conint(ge=5, le=1000) = Field(
+        10,
+        description="+usage=Size of the home directory for the notebook (Persistent Storage)\n+sort=7\n+label=Home Directory Size in GB (Persistent)",
+    )
+    service_account: Optional[str] = Field(
+        None, description="+usage=Service account that this workload should use"
+    )
+    mounts: Optional[List[Union[SecretMount, StringDataMount, VolumeMount]]] = Field(
+        None,
+        description="+usage=Configure data to be mounted to notebook pod(s)\n+ignore\n+sort=10011",
+    )
+    env: Optional[Dict[str, str]] = Field(
+        None,
+        description="+label=Environment Variables\n+usage=Configure environment variables to be set in the notebook pod(s)\n+ignore\n+sort=10012",
+    )
+
+
 class Service(BaseModel):
     """
     +docs=Describes the configuration for the service
     """
 
     type: constr(regex=r"^service$") = Field(..., description="+value=service")
     name: constr(regex=r"^[a-z][a-z0-9\-]{1,23}[a-z0-9]$") = Field(
@@ -795,8 +872,8 @@
         False,
         description="+label=Allow intercepts\n+usage=Whether to allow intercepts to be applied for this service.\nThis would inject an additional sidecar in each pod of the service. Not recommended on production",
     )
     kustomize: Optional[Kustomize] = None
 
 
 class Application(BaseModel):
-    __root__: Union[Service, Job, ModelDeployment]
+    __root__: Union[Service, Job, ModelDeployment, Notebook]
```

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.9rc2/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/display_util.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/cli/util.py` & `servicefoundry-0.9.9rc2/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/app.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/build.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/route.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/service.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.9rc2/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.9rc2/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.9rc2/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.9rc2/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/langchain.py` & `servicefoundry-0.9.9rc2/servicefoundry/langchain.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/const.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.9rc2/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.9rc2/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.9rc2/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/messages.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/session.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/util.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/lib/win32.py` & `servicefoundry-0.9.9rc2/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/logger.py` & `servicefoundry-0.9.9rc2/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.9rc2/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,24 @@
     class Config:
         extra = "forbid"
 
     def deploy(self, workspace_fqn: str, wait: bool = True) -> Deployment:
         return deploy_component(component=self, workspace_fqn=workspace_fqn, wait=wait)
 
 
+class Notebook(models.Notebook):
+    type: constr(regex=r"^notebook$") = Field("notebook", description="+value=notebook")
+
+    class Config:
+        extra = "forbid"
+
+    def deploy(self, workspace_fqn: str, wait: bool = True) -> Deployment:
+        return deploy_component(component=self, workspace_fqn=workspace_fqn, wait=wait)
+
+
 class Application(models.Application):
     class Config:
         extra = "forbid"
 
     def deploy(self, workspace_fqn: str, wait: bool = True) -> Deployment:
         return deploy_component(
             component=self.__root__, workspace_fqn=workspace_fqn, wait=wait
```

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/lib/patched_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
 import re
-from typing import Dict, Optional, Union
+from typing import Optional, Union
 
 from pydantic import Field, constr, root_validator, validator
 from typing_extensions import Literal
 
 from servicefoundry.auto_gen import models
 
 # TODO (chiragjn): Setup a base class for auto_gen.models to make `extra = "forbid"` default
@@ -249,7 +249,25 @@
 
     type: Literal["nodepool_selector"] = "nodepool_selector"
 
 
 class Endpoint(models.Endpoint):
     class Config:
         extra = "forbid"
+
+
+class TruefoundryImageBase(models.TruefoundryImageBase):
+    type: Literal["truefoundrybase"] = Field(
+        "truefoundrybase", description="+value=truefoundrybase"
+    )
+
+    class Config:
+        extra = "forbid"
+
+
+class TruefoundryImageFull(models.TruefoundryImageFull):
+    type: Literal["truefoundryfull"] = Field(
+        "truefoundryfull", description="+value=truefoundryfull"
+    )
+
+    class Config:
+        extra = "forbid"
```

### Comparing `servicefoundry-0.9.9rc1/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.9rc2/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.9rc1/PKG-INFO` & `servicefoundry-0.9.9rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.9rc1
+Version: 0.9.9rc2
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

