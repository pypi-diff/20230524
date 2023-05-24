# Comparing `tmp/servicefoundry-0.8.7.tar.gz` & `tmp/servicefoundry-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.8.7.tar", max compression
+gzip compressed data, was "servicefoundry-0.8.8.tar", max compression
```

## Comparing `servicefoundry-0.8.7.tar` & `servicefoundry-0.8.8.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0      672 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/README.md
--rw-r--r--   0        0        0     2116 2023-05-08 06:54:49.631181 servicefoundry-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     1269 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/__init__.py
--rw-r--r--   0        0        0    36574 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4159 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      531 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1357 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6479 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6458 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     2795 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     3587 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     3863 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2492 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-05-08 06:54:38.707267 servicefoundry-0.8.7/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    23939 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     5624 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0     9147 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0     9914 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5196 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8890 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-05-08 06:54:38.711267 servicefoundry-0.8.7/servicefoundry/version.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-05-10 18:59:02.812336 servicefoundry-0.8.8/README.md
+-rw-r--r--   0        0        0     2116 2023-05-10 18:59:16.052476 servicefoundry-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     1269 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    36861 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4159 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1364 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1357 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6479 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6458 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1042 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     2795 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     3587 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     3863 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2492 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    23939 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     5624 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-05-10 18:59:02.816336 servicefoundry-0.8.8/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0     9147 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0     9914 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5196 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8890 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-05-10 18:59:02.820336 servicefoundry-0.8.8/servicefoundry/version.py
+-rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.8.8/PKG-INFO
```

### Comparing `servicefoundry-0.8.7/README.md` & `servicefoundry-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/pyproject.toml` & `servicefoundry-0.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.8.7"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.8.8"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.8.7/servicefoundry/__init__.py` & `servicefoundry-0.8.8/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/auto_gen/models.py` & `servicefoundry-0.8.8/servicefoundry/auto_gen/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-04-27T20:26:32+00:00
+#   timestamp: 2023-05-09T19:01:41+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, confloat, conint, constr
@@ -15,19 +15,19 @@
     """
     +label=Username and password for service auth
     """
 
     type: Literal["basic_auth"]
     username: constr(regex=r"^[a-z0-9-@\.]{1,64}$") = Field(
         ...,
-        description="+label=Username for service auth\n+message=Upto 64 lower case alphanumeric character long",
+        description="+label=Username for service auth\n+message=Upto 64 lower case alphanumeric character long\n+sort=1",
     )
     password: constr(regex=r"^[a-zA-Z0-9\.!@#$%^&*()_+=\-]{1,64}$") = Field(
         ...,
-        description="+label=Password for service auth\n+message=Password should not be more than 64 characters",
+        description="+label=Password for service auth\n+message=Password should not be more than 64 characters\n+sort=2",
     )
 
 
 class BlueGreen(BaseModel):
     """
     +docs=This strategy brings up the new release completely before switching the complete load to the new release.
     This minimizes the time that two versions are serving traffic at the same time.
@@ -371,27 +371,27 @@
     +docs=Describes the resource constraints for the application so that it can be deployed accordingly on the cluster
     To learn more you can go [here](https://docs.truefoundry.com/docs/resources)
     +icon=fa-microchip
     +label=Resources
     +usage=Set resource constraints for the application. [Docs](https://docs.truefoundry.com/docs/resources)
     """
 
-    cpu_request: confloat(ge=0.001, le=16.0) = Field(
+    cpu_request: confloat(ge=0.001, le=128.0) = Field(
         0.2,
         description="+label=CPU Request\n+sort=1\n+usage=Requested CPU which determines the minimum cost incurred. The CPU usage can exceed the requested\namount, but not the value specified in the limit. 1 CPU means 1 CPU core. Fractional CPU can be requested\nlike `0.5` or `0.05`",
     )
-    cpu_limit: confloat(ge=0.001, le=16.0) = Field(
+    cpu_limit: confloat(ge=0.001, le=128.0) = Field(
         0.5,
         description="+label=CPU Limit\n+usage=CPU limit beyond which the usage cannot be exceeded. 1 CPU means 1 CPU core. Fractional CPU can be requested\nlike `0.5`. CPU limit should be >= cpu request.\n+sort=2",
     )
-    memory_request: conint(ge=1, le=32000) = Field(
+    memory_request: conint(ge=1, le=2000000) = Field(
         200,
         description="+label=Memory Request\n+usage=Requested memory which determines the minimum cost incurred. The unit of memory is in megabytes(MB).\nSo 1 means 1 MB and 2000 means 2GB.\n+sort=3",
     )
-    memory_limit: conint(ge=1, le=32000) = Field(
+    memory_limit: conint(ge=1, le=2000000) = Field(
         500,
         description="+label=Memory Limit\n+usage=Memory limit after which the application will be killed with an OOM error. The unit of memory is\nin megabytes(MB). So 1 means 1 MB and 2000 means 2GB. MemoryLimit should be greater than memory request.\n+sort=4",
     )
     ephemeral_storage_request: conint(ge=1, le=500000) = Field(
         1000,
         description="+label=Storage Request\n+usage=Requested disk storage. The unit of memory is in megabytes(MB).\nThis is ephemeral storage and will be wiped out on pod restarts or eviction\n+sort=5",
     )
@@ -400,14 +400,18 @@
         description="+label=Storage Limit\n+usage=Disk storage limit. The unit of memory is in megabytes(MB). Exceeding this limit will result in eviction.\nIt should be greater than the request. This is ephemeral storage and will be wiped out on pod restarts or eviction\n+sort=6",
     )
     gpu: Optional[GPU] = None
     instance_family: Optional[List[str]] = Field(
         None,
         description="+label=Instance family\n+usage=Instance family of the underlying machine to use. Multiple instance families can be supplied.\nThe workload is guaranteed to be scheduled on one of them.",
     )
+    nodepools: Optional[List[str]] = Field(
+        None,
+        description="+label=Nodepools\n+usage=Nodepools where you want to run your workload. Multiple nodepools can be selected.\n The workload is guaranteed to be scheduled on one of the nodepool",
+    )
     shared_memory_size: Optional[conint(ge=64, le=32000)] = Field(
         None,
         description="+label=Shared Memory Size\n+usage=Define the shared memory requirements for your workload. Machine learning libraries like Pytorch can use Shared Memory\nfor inter-process communication. If you use this, we will mount a `tmpfs` backed volume at the `/dev/shm` directory.\nAny usage will also count against the workload's memory limit (`resources.memory_limit`) along with your workload's memory usage.\nIf the overall usage goes above `resources.memory_limit` the user process may get killed.\nShared Memory Size cannot be more than the defined Memory Limit for the workload.",
     )
     capacity_type: Optional[CapacityType] = Field(
         None,
         description='+label=Capacity Type\n+usage=Configure what type of nodes to run the app. By default no placement logic is applied.\n"spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.\n"spot" will strictly place the application on spot nodes.\n"on_demand" will strictly place the application on on-demand nodes.',
```

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/__init__.py` & `servicefoundry-0.8.8/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.8.8/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.8.8/servicefoundry/builder/builders/dockerfile.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.8.8/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.8.8/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/builder/docker_service.py` & `servicefoundry-0.8.8/servicefoundry/builder/docker_service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/cli_main.py` & `servicefoundry-0.8.8/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/build_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.8.8/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/display_util.py` & `servicefoundry-0.8.8/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/cli/util.py` & `servicefoundry-0.8.8/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/__main__.py` & `servicefoundry-0.8.8/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/app.py` & `servicefoundry-0.8.8/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/build.py` & `servicefoundry-0.8.8/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.8.8/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.8.8/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.8.8/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/route.py` & `servicefoundry-0.8.8/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/service.py` & `servicefoundry-0.8.8/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/function_service/utils.py` & `servicefoundry-0.8.8/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/internal/experimental.py` & `servicefoundry-0.8.8/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/io/output_callback.py` & `servicefoundry-0.8.8/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.8.8/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.8.8/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.8.8/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.8.8/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.8.8/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.8.8/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.8.8/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.8.8/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.8.8/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.8.8/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.8.8/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.8.8/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.8.8/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.8.8/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.8.8/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/const.py` & `servicefoundry-0.8.8/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/dao/application.py` & `servicefoundry-0.8.8/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/dao/version.py` & `servicefoundry-0.8.8/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.8.8/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/exceptions.py` & `servicefoundry-0.8.8/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.8.8/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.8.8/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.8.8/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.8.8/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.8.8/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.8.8/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/messages.py` & `servicefoundry-0.8.8/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/model/entity.py` & `servicefoundry-0.8.8/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/session.py` & `servicefoundry-0.8.8/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/util.py` & `servicefoundry-0.8.8/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/lib/win32.py` & `servicefoundry-0.8.8/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/logger.py` & `servicefoundry-0.8.8/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.8.8/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.8.8/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.8.8/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.8.8/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.8.8/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/lib/models.py` & `servicefoundry-0.8.8/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.8.8/servicefoundry/v2/lib/patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/servicefoundry/v2/lib/source.py` & `servicefoundry-0.8.8/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.8.7/PKG-INFO` & `servicefoundry-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.8.7
+Version: 0.8.8
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

