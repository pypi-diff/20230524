# Comparing `tmp/iambic_core-0.7.3.tar.gz` & `tmp/iambic_core-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.7.3.tar", max compression
+gzip compressed data, was "iambic_core-0.7.6.tar", max compression
```

## Comparing `iambic_core-0.7.3.tar` & `iambic_core-0.7.6.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-05-10 20:27:44.608259 iambic_core-0.7.3/LICENSE.md
--rw-r--r--   0        0        0    10551 2023-05-10 20:27:44.612259 iambic_core-0.7.3/README.md
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/config/templates.py
--rw-r--r--   0        0        0     3312 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/config/utils.py
--rw-r--r--   0        0        0    77079 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5516 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/parser.py
--rw-r--r--   0        0        0    46094 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/template_generation.py
--rw-r--r--   0        0        0    26626 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/lambda/app.py
--rw-r--r--   0        0        0    13921 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/__init__.py
--rw-r--r--   0        0        0     2799 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.644259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2149 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2268 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2483 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    16350 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33385 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17683 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15896 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17544 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21304 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20623 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31619 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35514 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28498 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     2973 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-05-10 20:27:44.648259 iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8515 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5247 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-10 20:27:44.652259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2685 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9492 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13610 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-10 20:27:44.656259 iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-05-10 20:27:44.656259 iambic_core-0.7.3/pyproject.toml
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-15 14:23:53.922064 iambic_core-0.7.6/LICENSE.md
+-rw-r--r--   0        0        0    10551 2023-05-15 14:23:53.922064 iambic_core-0.7.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/templates.py
+-rw-r--r--   0        0        0     3312 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/utils.py
+-rw-r--r--   0        0        0    77079 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5516 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/parser.py
+-rw-r--r--   0        0        0    48014 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    28445 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/lambda/app.py
+-rw-r--r--   0        0        0    14239 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-15 14:23:53.950066 iambic_core-0.7.6/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2149 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2268 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2483 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    16350 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33385 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    18144 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15896 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    18077 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21757 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    21076 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35514 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28498 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1291 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     3009 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.954066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5247 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1359 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2685 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1290 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9492 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      173 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-15 14:23:53.958066 iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     2243 2023-05-15 14:23:53.962067 iambic_core-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0    12917 1970-01-01 00:00:00.000000 iambic_core-0.7.6/PKG-INFO
```

### Comparing `iambic_core-0.7.3/LICENSE.md` & `iambic_core-0.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/README.md` & `iambic_core-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/config/dynamic_config.py` & `iambic_core-0.7.6/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/config/utils.py` & `iambic_core-0.7.6/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/config/wizard.py` & `iambic_core-0.7.6/iambic/config/wizard.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/aio_utils/__init__.py` & `iambic_core-0.7.6/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/exceptions.py` & `iambic_core-0.7.6/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/git.py` & `iambic_core-0.7.6/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/iambic_enum.py` & `iambic_core-0.7.6/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/iambic_plugin.py` & `iambic_core-0.7.6/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/logger.py` & `iambic_core-0.7.6/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/models.py` & `iambic_core-0.7.6/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/noq_json.py` & `iambic_core-0.7.6/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/parser.py` & `iambic_core-0.7.6/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/core/template_generation.py` & `iambic_core-0.7.6/iambic/core/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from iambic.core import noq_json as json
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import AccessModelMixin, BaseModel, BaseTemplate, ProviderChild
 from iambic.core.parser import load_templates
 from iambic.core.utils import (
+    IAMBIC_ERR_MSG,
     evaluate_on_provider,
     gather_templates,
     get_provider_value,
     is_regex_match,
     sanitize_string,
 )
 
@@ -894,15 +895,15 @@
                 merge_model(new_model, existing_model, all_provider_children)
             )
         else:
             merged_list.append(new_model.copy())
     return merged_list
 
 
-def merge_model(
+def merge_model(  # noqa: C901
     new_model: BaseModel,
     existing_model: BaseModel,
     all_provider_children: list[ProviderChild],
     should_update_access_attributes=True,
 ) -> Union[BaseModel, list[BaseModel], None]:
     """
     Update the metadata of the new IAMbic model using the existing model.
@@ -986,24 +987,63 @@
                     if isinstance(new_value, str):
                         _cls = type(inner_element)
                         new_value = [_cls.new_instance_from_string(new_value)]
                         value_as_list = True  # because cast it into a list
                     elif not isinstance(new_value, list):
                         new_value = [new_value]
 
-                    new_value = merge_access_model_list(
-                        new_value, existing_value, all_provider_children
-                    )
+                    if all(isinstance(x, AccessModelMixin) for x in new_value):
+                        try:
+                            new_value = merge_access_model_list(
+                                new_value, existing_value, all_provider_children
+                            )
+                        except Exception as err:
+                            log.exception(
+                                f"Failed to merge template attribute. {IAMBIC_ERR_MSG}",
+                                key=key,
+                                new_value=[
+                                    {"value": str(val), "type": type(val)}
+                                    for val in new_value
+                                ],
+                                existing_value=[
+                                    {"value": str(val), "type": type(val)}
+                                    for val in existing_value
+                                ],
+                                err=repr(err),
+                            )
+                            raise
+
                     setattr(
                         merged_model, key, new_value if value_as_list else new_value[0]
                     )
                 elif isinstance(inner_element, BaseModel):
-                    new_value = merge_model_list(
-                        new_value, existing_value, all_provider_children
-                    )
+                    if not isinstance(new_value, list):
+                        new_value = [new_value]
+
+                    if all(isinstance(x, BaseModel) for x in new_value):
+                        try:
+                            new_value = merge_model_list(
+                                new_value, existing_value, all_provider_children
+                            )
+                        except Exception as err:
+                            log.exception(
+                                f"Failed to merge template attribute. {IAMBIC_ERR_MSG}",
+                                key=key,
+                                new_value=[
+                                    {"value": str(val), "type": type(val)}
+                                    for val in new_value
+                                ],
+                                existing_value=[
+                                    {"value": str(val), "type": type(val)}
+                                    for val in existing_value
+                                ],
+                                err=repr(err),
+                            )
+                            raise
+
                     setattr(
                         merged_model, key, new_value if value_as_list else new_value[0]
                     )
                 else:
                     setattr(merged_model, key, new_value)
             else:
                 setattr(merged_model, key, new_value)
@@ -1026,15 +1066,15 @@
             elif new_value is None:
                 # cloud is represented by None, local is a BaseModel.
                 # this will only work if the local BaseModel does not carry
                 # any local metadata that needs to survive outside of cloud.
                 setattr(merged_model, key, new_value)
             else:
                 raise TypeError(
-                    f"Type of {type(new_value)} is not supported. Please file a github issue"
+                    f"Type of {type(new_value)} is not supported. {IAMBIC_ERR_MSG}"
                 )
         elif key not in iambic_fields:
             setattr(merged_model, key, new_value)
     return merged_model
 
 
 def delete_orphaned_templates(
```

### Comparing `iambic_core-0.7.3/iambic/core/utils.py` & `iambic_core-0.7.6/iambic/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 
 if TYPE_CHECKING:
     from iambic.core.models import ProposedChange
 
 
 NOQ_TEMPLATE_REGEX = r".*template_type:\n?.*NOQ::"
 RATE_LIMIT_STORAGE: dict[str, int] = {}
+IAMBIC_ERR_MSG = (
+    "Please file a github issue or message us on the slack community channel. "
+    "Include as much of the traceback and this error message as possible. "
+    "Be sure to redact any sensitive information."
+)
 
 __WRITABLE_DIRECTORY__ = pathlib.Path.home()
 
 
 def init_writable_directory() -> None:
     # use during development
     __WRITABLE_DIRECTORY__ = pathlib.Path.home()
@@ -329,15 +334,22 @@
     return d
 
 
 def transform_comments(yaml_dict):
     comment_dict = {}
     yaml_dict["metadata_commented_dict"] = comment_dict
     for key, comment in yaml_dict.ca.items.items():
-        comment_dict[key] = comment[2].value
+        # flatten comment for now since we do not have
+        # a lot of experience with more complex comment token
+        flatten_comment = None
+        if comment[2]:
+            flatten_comment = comment[2].value
+        elif comment[3] and type(comment[3]) == list:
+            flatten_comment = " ".join([token.value.strip() for token in comment[3]])
+        comment_dict[key] = flatten_comment
         value = yaml_dict[key]
         if isinstance(value, list) and len(value) > 0 and isinstance(value[0], dict):
             yaml_dict[key] = [transform_comments(n) for n in value]
         elif isinstance(value, dict):
             yaml_dict[key] = transform_comments(value)
     return yaml_dict
 
@@ -720,7 +732,40 @@
             )
             if getattr(new_value, "deleted", None) is True:
                 setattr(resource, field_name, None)
             else:
                 setattr(resource, field_name, new_value)
 
     return resource
+
+
+def convert_between_json_and_yaml(input_string: str) -> str:
+    """
+    Convert a string from AWS PascalCase JSON to IAMbic compatible YAML, or visa-versa.
+    When converting from JSON to YAML, dictionary keys are converted from PascalCase to snake_case.
+    When converting from YAML to JSON, dictionary keys are converted from snake_case to PascalCase.
+
+    :param input_string: The input string, which should be valid JSON or YAML.
+    :return: The converted string.
+    """
+    from json import JSONDecodeError
+
+    from stringcase import pascalcase, snakecase
+
+    from iambic.core.utils import yaml
+
+    try:
+        # Try parsing the input as JSON
+        data = json.loads(input_string)
+        # Convert keys from PascalCase/camelCase to snake_case
+        converted_data = normalize_dict_keys(data, snakecase)
+        # Convert to YAML
+        output = yaml.dump(converted_data)
+    except JSONDecodeError:
+        # If the input is not JSON, try parsing it as YAML
+        data = yaml.load(input_string)
+        # Convert keys from snake_case to PascalCase
+        converted_data = normalize_dict_keys(data, pascalcase)
+        # Convert to JSON
+        output = json.dumps(converted_data, indent=2)
+
+    return output
```

### Comparing `iambic_core-0.7.3/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.7.6/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.7.6/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.7.6/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/github/templates/iambic-import.yml` & `iambic_core-0.7.6/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/github/utils.py` & `iambic_core-0.7.6/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/lambda/app.py` & `iambic_core-0.7.6/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/main.py` & `iambic_core-0.7.6/iambic/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from iambic.core.context import ctx
 from iambic.core.git import clone_git_repos
 from iambic.core.iambic_enum import Command, IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import ExecutionMessage, TemplateChangeDetails
 from iambic.core.parser import load_templates
 from iambic.core.utils import (
+    convert_between_json_and_yaml,
     exceptions_in_proposed_changes,
     gather_templates,
     init_writable_directory,
 )
 from iambic.output.text import (
     file_render_resource_changes,
     screen_render_resource_changes,
@@ -470,10 +471,21 @@
     help="If enabled, wizard will ask more questions",
 )
 def setup(repo_dir: str, is_more_options: bool):
     ctx.command = Command.APPLY
     ConfigurationWizard(repo_dir, is_more_options=is_more_options).run()
 
 
+@cli.command()
+def convert():
+    """
+    Convert a string from AWS PascalCase JSON to IAMbic compatible YAML, or visa-versa.
+    """
+    user_input = click.edit()
+    if user_input is not None:
+        output = convert_between_json_and_yaml(user_input)
+        click.echo(output)
+
+
 if __name__ == "__main__":
     init_writable_directory()
     cli()
```

### Comparing `iambic_core-0.7.3/iambic/output/__init__.py` & `iambic_core-0.7.6/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/filters.py` & `iambic_core-0.7.6/iambic/output/filters.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/models.py` & `iambic_core-0.7.6/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.7.6/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.7.6/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.7.6/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/output/text.py` & `iambic_core-0.7.6/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/README.md` & `iambic_core-0.7.6/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     return str(os.path.join(base_dir, "resources", "aws", *RESOURCE_DIR))
 
 
 def get_templated_group_file_path(
     group_dir: str,
     group_name: str,
     included_accounts: list[str],
+    group_path: str = None,
 ) -> str:
     if included_accounts is not None and len(included_accounts) > 1:
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
@@ -72,15 +73,29 @@
         .replace("{{var.", "")
         .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
-    return str(os.path.join(group_dir, separator, f"{file_name}.yaml"))
+
+    # using path components from path attribute
+    if group_path:
+        group_path_components = group_path.split("/")
+        # get rid of empty component
+        group_path_components = [
+            component for component in group_path_components if component
+        ]
+
+    # stitch desired location together
+    os_paths = [group_dir, separator]
+    os_paths.extend(group_path_components)
+    os_paths.append(f"{file_name}.yaml")
+
+    return str(os.path.join(*os_paths))
 
 
 async def generate_account_group_resource_files(
     exe_message: ExecutionMessage,
     aws_account: AWSAccount,
 ) -> dict:
     account_group_response_dir = get_response_dir(exe_message, aws_account)
@@ -299,14 +314,15 @@
             prefer_templatized=prefer_templatized,
         )
 
     file_path = get_templated_group_file_path(
         group_dir,
         group_name,
         group_template_params.get("included_accounts"),
+        group_path=path,
     )
     return create_or_update_template(
         file_path,
         existing_template_map,
         group_name,
         AwsIamGroupTemplate,
         group_template_params,
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 
 def get_templated_managed_policy_file_path(
     managed_policy_dir: str,
     policy_name: str,
     included_accounts: list[str],
     account_map: dict[str, AWSAccount],
+    managed_policy_path: str = None,
 ):
     if len(included_accounts) > 1:
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
@@ -70,15 +71,29 @@
         .replace("{{var.", "")
         .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
-    return str(os.path.join(managed_policy_dir, separator, f"{file_name}.yaml"))
+
+    # using path components from path attribute
+    if managed_policy_path:
+        managed_policy_path_components = managed_policy_path.split("/")
+        # get rid of empty component
+        managed_policy_path_components = [
+            component for component in managed_policy_path_components if component
+        ]
+
+    # stitch desired location together
+    os_paths = [managed_policy_dir, separator]
+    os_paths.extend(managed_policy_path_components)
+    os_paths.append(f"{file_name}.yaml")
+
+    return str(os.path.join(*os_paths))
 
 
 async def generate_account_managed_policy_resource_files(
     exe_message: ExecutionMessage,
     aws_account: AWSAccount,
 ) -> dict:
     account_resource_dir = get_response_dir(exe_message, aws_account)
@@ -286,14 +301,15 @@
         template_properties["tags"] = tags
 
     file_path = get_templated_managed_policy_file_path(
         managed_policy_dir,
         managed_policy_name,
         template_params.get("included_accounts"),
         aws_account_map,
+        managed_policy_path=path,
     )
     return create_or_update_template(
         file_path,
         existing_template_map,
         managed_policy_name,
         AwsIamManagedPolicyTemplate,
         template_params,
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     return str(os.path.join(base_dir, "resources", "aws", *RESOURCE_DIR))
 
 
 def get_templated_role_file_path(
     role_dir: str,
     role_name: str,
     included_accounts: list[str],
+    role_path: str = None,
 ) -> str:
     if included_accounts is not None and len(included_accounts) > 1:
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
@@ -74,15 +75,29 @@
         .replace("{{var.", "")
         .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
-    return str(os.path.join(role_dir, separator, f"{file_name}.yaml"))
+
+    # using path components from path attribute
+    if role_path:
+        role_path_components = role_path.split("/")
+        # get rid of empty component
+        role_path_components = [
+            component for component in role_path_components if component
+        ]
+
+    # stitch desired location together
+    os_paths = [role_dir, separator]
+    os_paths.extend(role_path_components)
+    os_paths.append(f"{file_name}.yaml")
+
+    return str(os.path.join(*os_paths))
 
 
 async def generate_account_role_resource_files(
     exe_message: ExecutionMessage,
     aws_account: AWSAccount,
 ) -> dict:
     account_resource_dir = get_response_dir(exe_message, aws_account)
@@ -405,14 +420,15 @@
 
         role_template_properties["tags"] = tags
 
     file_path = get_templated_role_file_path(
         role_dir,
         role_name,
         role_template_params.get("included_accounts"),
+        role_path=path,
     )
     return create_or_update_template(
         file_path,
         existing_template_map,
         role_name,
         AwsIamRoleTemplate,
         role_template_params,
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     return str(os.path.join(base_dir, "resources", "aws", *RESOURCE_DIR))
 
 
 def get_templated_user_file_path(
     user_dir: str,
     user_name: str,
     included_accounts: list[str],
+    user_path: str = None,
 ) -> str:
     if included_accounts is not None and len(included_accounts) > 1:
         separator = "multi_account"
     elif included_accounts == ["*"] or included_accounts is None:
         separator = "all_accounts"
     else:
         separator = included_accounts[0]
@@ -74,15 +75,29 @@
         .replace("{{var.", "")
         .replace("{{", "")
         .replace("}}_", "_")
         .replace("}}", "_")
         .replace(".", "_")
         .lower()
     )
-    return str(os.path.join(user_dir, separator, f"{file_name}.yaml"))
+
+    # using path components from path attribute
+    if user_path:
+        user_path_components = user_path.split("/")
+        # get rid of empty component
+        user_path_components = [
+            component for component in user_path_components if component
+        ]
+
+    # stitch desired location together
+    os_paths = [user_dir, separator]
+    os_paths.extend(user_path_components)
+    os_paths.append(f"{file_name}.yaml")
+
+    return str(os.path.join(*os_paths))
 
 
 async def generate_account_user_resource_files(
     exe_message: ExecutionMessage,
     aws_account: AWSAccount,
 ) -> dict:
     account_resource_dir = get_response_dir(exe_message, aws_account)
@@ -383,14 +398,15 @@
 
         user_template_properties["tags"] = tags
 
     file_path = get_templated_user_file_path(
         user_dir,
         user_name,
         user_template_params.get("included_accounts"),
+        user_path=path,
     )
     return create_or_update_template(
         file_path,
         existing_template_map,
         user_name,
         AwsIamUserTemplate,
         user_template_params,
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "iambic-aws"
+name = "iambic-google-workspace"
 version = "0.1.0"
-description = "The IAMbic AWS plugin."
+description = "The IAMbic Google Workspace plugin."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 
 [tool.isort]
+known_first_party = ["iambic"]
+src_paths = ["iambic","test","functional_tests","build_utils"]
+known_third_party = ["_pytest", "okta", "github", "pydantic", "rich"]
 profile = "black"
-add_imports = "from __future__ import annotations"
+add_imports = ["from __future__ import annotations"]
+skip_gitignore = true
+line_length = 88
 
 [tool.poetry.dependencies]
 python = "^3.10"
-boto3 = "^1.24.88"
 "ruamel.yaml" = "^0.17.21"
 asgiref = "^3.5.2"
 structlog = "^22.1.0"
 pydantic = "^1.10.2"
 deepdiff = "^5.8.1"
 Jinja2 = "^3.1.2"
 black = "^22.10.0"
@@ -29,14 +33,16 @@
 pytest = "^7.1.3"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.20.0"
 ujson = "^5.5.0"
 aiofiles = "^22.1.0"
 xxhash = "^3.0.0"
+google-api-python-client = "^2.64.0"
+google-auth = "^2.12.0"
 jsonschema2md2 = "^0.6.0"
 GitPython = "^3.1.30"
 PyGithub = "^1.57"
 pydantic-factories = "^1.12.0"
 asyncache = "^0.3.1"
 dateparser = "^1.1.4"
 pytest-mock = "^3.10.0"
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Union
 
 from iambic.core.template_generation import (
     base_group_str_attribute as core_base_group_str_attribute,
 )
 from iambic.core.template_generation import (
     group_dict_attribute as core_group_dict_attribute,
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-name = "iambic-google-workspace"
+name = "iambic-okta"
 version = "0.1.0"
-description = "The IAMbic Google Workspace plugin."
+description = "The IAMbic Okta plugin."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 
 [tool.isort]
+known_first_party = ["iambic"]
+src_paths = ["iambic","test","functional_tests","build_utils"]
+known_third_party = ["_pytest", "okta", "github", "pydantic", "rich"]
 profile = "black"
-add_imports = "from __future__ import annotations"
+add_imports = ["from __future__ import annotations"]
+skip_gitignore = true
+line_length = 88
 
 [tool.poetry.dependencies]
 python = "^3.10"
 "ruamel.yaml" = "^0.17.21"
 asgiref = "^3.5.2"
 structlog = "^22.1.0"
 pydantic = "^1.10.2"
@@ -28,20 +33,19 @@
 pytest = "^7.1.3"
 pytest-asyncio = "^0.20.3"
 pytest-cov = "^4.0.0"
 pre-commit = "^2.20.0"
 ujson = "^5.5.0"
 aiofiles = "^22.1.0"
 xxhash = "^3.0.0"
-google-api-python-client = "^2.64.0"
-google-auth = "^2.12.0"
 jsonschema2md2 = "^0.6.0"
 GitPython = "^3.1.30"
 PyGithub = "^1.57"
 pydantic-factories = "^1.12.0"
+okta = "^2.8.0"
 asyncache = "^0.3.1"
 dateparser = "^1.1.4"
 pytest-mock = "^3.10.0"
 types-dateparser = "^1.1.4.5"
 
 [tool.poetry.group.dev.dependencies]
 types-cachetools = "^5.2.1"
```

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.7.6/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/request_handler/expire_resources.py` & `iambic_core-0.7.6/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/request_handler/git_apply.py` & `iambic_core-0.7.6/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/request_handler/git_plan.py` & `iambic_core-0.7.6/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.7.6/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.7.3/pyproject.toml` & `iambic_core-0.7.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
+[tool.isort]
+# Ensure that all other pyproject.toml files in this repository have the same isort settings
+known_first_party = ["iambic"]
+src_paths = ["iambic","test","functional_tests","build_utils"]
+known_third_party = ["_pytest", "okta", "github", "pydantic", "rich"]
+profile = "black"
+add_imports = ["from __future__ import annotations"]
+skip_gitignore = true
+line_length = 88
+
+
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.7.3"
+version = "0.7.6"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
 
-[tool.isort]
-profile = "black"
-add_imports = "from __future__ import annotations"
-
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = "^1.26.95"
 click = "^8.1.3"
 "ruamel.yaml" = "^0.17.21"
 asgiref = "^3.6.0"
 structlog = "^22.3.0"
@@ -58,14 +65,15 @@
 aws-error-utils = "^2.7.0"
 types-mock = "^5.0.0.5"
 rich = "^13.3.2"
 dictdiffer = "^0.9.0"
 msal = "^1.21.0"
 aiohttp = "^3.8.4"
 pyopenssl = "^23.0.0"
+stringcase = "^1.2.0"
 
 [tool.poetry.scripts]
 iambic = "iambic.main:cli"
 
 [tool.poetry.group.dev.dependencies]
 types-cachetools = "^5.3.0.4"
 types-pyyaml = "^6.0.12.8"
```

### Comparing `iambic_core-0.7.3/PKG-INFO` & `iambic_core-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.7.3
+Version: 0.7.6
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -43,14 +43,15 @@
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0)
 Requires-Dist: pytest-rerunfailures (>=11.1.2,<12.0.0)
 Requires-Dist: pytest-xdist (>=3.2.1,<4.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: slack-bolt (>=1.16.4,<2.0.0)
+Requires-Dist: stringcase (>=1.2.0,<2.0.0)
 Requires-Dist: structlog (>=22.3.0,<23.0.0)
 Requires-Dist: types-dateparser (>=1.1.4.5,<2.0.0.0)
 Requires-Dist: types-mock (>=5.0.0.5,<6.0.0.0)
 Requires-Dist: ujson (>=5.7.0,<6.0.0)
 Requires-Dist: xxhash (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
```

