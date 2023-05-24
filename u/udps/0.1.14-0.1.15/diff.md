# Comparing `tmp/udps-0.1.14.tar.gz` & `tmp/udps-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udps-0.1.14.tar", max compression
+gzip compressed data, was "udps-0.1.15.tar", max compression
```

## Comparing `udps-0.1.14.tar` & `udps-0.1.15.tar`

### file list

```diff
@@ -1,249 +1,249 @@
--rw-r--r--   0        0        0    11357 2023-05-02 09:23:48.736507 udps-0.1.14/LICENSE
--rw-r--r--   0        0        0     2471 2023-05-02 09:23:48.736507 udps-0.1.14/README.md
--rw-r--r--   0        0        0     3071 2023-05-02 09:23:48.740507 udps-0.1.14/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-02 09:23:48.740507 udps-0.1.14/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.740507 udps-0.1.14/tests/mocks/__init__.py
--rw-r--r--   0        0        0      721 2023-05-02 09:23:48.740507 udps-0.1.14/tests/mocks/mock_writers.py
--rw-r--r--   0        0        0     1028 2023-05-02 09:23:48.740507 udps-0.1.14/tests/test_authz_analyzer.py
--rw-r--r--   0        0        0     5112 2023-05-02 09:23:48.740507 udps-0.1.14/tests/test_cli.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.740507 udps-0.1.14/tests/test_writers/__init__.py
--rw-r--r--   0        0        0     1355 2023-05-02 09:23:48.740507 udps-0.1.14/tests/test_writers/test_csv_writer.py
--rw-r--r--   0        0        0      953 2023-05-02 09:23:48.740507 udps-0.1.14/tests/test_writers/test_multijson_writer.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/__init__.py
--rw-r--r--   0        0        0        1 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/__init__.py
--rw-r--r--   0        0        0    14110 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
--rw-r--r--   0        0        0    11644 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
--rw-r--r--   0        0        0    14917 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
--rw-r--r--   0        0        0     9884 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
--rw-r--r--   0        0        0    20662 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
--rw-r--r--   0        0        0    31812 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
--rw-r--r--   0        0        0    18235 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
--rw-r--r--   0        0        0    17618 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
--rw-r--r--   0        0        0     7529 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
--rw-r--r--   0        0        0     7744 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
--rw-r--r--   0        0        0     4073 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
--rw-r--r--   0        0        0    24204 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
--rw-r--r--   0        0        0    20163 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
--rw-r--r--   0        0        0    13494 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
--rw-r--r--   0        0        0     8446 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
--rw-r--r--   0        0        0    16466 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
--rw-r--r--   0        0        0    16126 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
--rw-r--r--   0        0        0    14831 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
--rw-r--r--   0        0        0     3066 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
--rw-r--r--   0        0        0     5550 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
--rw-r--r--   0        0        0     5906 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
--rw-r--r--   0        0        0     4446 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
--rw-r--r--   0        0        0     8937 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
--rw-r--r--   0        0        0    20162 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
--rw-r--r--   0        0        0    10324 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
--rw-r--r--   0        0        0     6886 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
--rw-r--r--   0        0        0    23422 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
--rw-r--r--   0        0        0     2358 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
--rw-r--r--   0        0        0     7124 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
--rw-r--r--   0        0        0     4549 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
--rw-r--r--   0        0        0     5215 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
--rw-r--r--   0        0        0     5987 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
--rw-r--r--   0        0        0     5862 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
--rw-r--r--   0        0        0     3396 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
--rw-r--r--   0        0        0     2298 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
--rw-r--r--   0        0        0     5264 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
--rw-r--r--   0        0        0     4596 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
--rw-r--r--   0        0        0     3653 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
--rw-r--r--   0        0        0     4392 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
--rw-r--r--   0        0        0    26158 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
--rw-r--r--   0        0        0    10097 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
--rw-r--r--   0        0        0     8580 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
--rw-r--r--   0        0        0    33775 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
--rw-r--r--   0        0        0    16439 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
--rw-r--r--   0        0        0    13955 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
--rw-r--r--   0        0        0    18162 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
--rw-r--r--   0        0        0     3040 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
--rw-r--r--   0        0        0     5254 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
--rw-r--r--   0        0        0     3569 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
--rw-r--r--   0        0        0     4436 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
--rw-r--r--   0        0        0    14441 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
--rw-r--r--   0        0        0     3582 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
--rw-r--r--   0        0        0     4890 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
--rw-r--r--   0        0        0     4842 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0     2831 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
--rw-r--r--   0        0        0     1595 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
--rw-r--r--   0        0        0     3805 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
--rw-r--r--   0        0        0     2597 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
--rw-r--r--   0        0        0     2321 2023-05-02 09:23:48.740507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
--rw-r--r--   0        0        0     4018 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
--rw-r--r--   0        0        0     5298 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
--rw-r--r--   0        0        0     1579 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/aws/test_exporter.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/aws/utils/__init__.py
--rw-r--r--   0        0        0     1731 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/bigquery/__init__.py
--rw-r--r--   0        0        0     5596 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/bigquery/generate_authz_entry.py
--rw-r--r--   0        0        0     6936 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/bigquery/mocks.py
--rw-r--r--   0        0        0    15539 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/bigquery/test_bigquery.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/databricks/__init__.py
--rw-r--r--   0        0        0    17596 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/databricks/generate_authz_entry.py
--rw-r--r--   0        0        0     9136 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/databricks/mocks.py
--rw-r--r--   0        0        0    13149 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/databricks/test_analyzer.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    14532 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/mongodb/test_atlas_organization_users.py
--rw-r--r--   0        0        0     7391 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/mongodb/test_mongodb.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/postgres/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/postgres/mocks/__init__.py
--rw-r--r--   0        0        0     1195 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
--rw-r--r--   0        0        0    12910 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/postgres/test_postgress_analyzer.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/redshift/__init__.py
--rw-r--r--   0        0        0    12179 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/redshift/test_redshift.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    14330 2023-05-02 09:23:48.744507 udps-0.1.14/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
--rw-r--r--   0        0        0     1086 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/__init__.py
--rw-r--r--   0        0        0     9737 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/cli.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/__init__.py
--rw-r--r--   0        0        0      626 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/__init__.py
--rw-r--r--   0        0        0      113 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
--rw-r--r--   0        0        0     3252 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
--rw-r--r--   0        0        0     7808 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
--rw-r--r--   0        0        0    13042 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
--rw-r--r--   0        0        0       90 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
--rw-r--r--   0        0        0      141 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
--rw-r--r--   0        0        0      111 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
--rw-r--r--   0        0        0       14 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
--rw-r--r--   0        0        0      125 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
--rw-r--r--   0        0        0      893 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
--rw-r--r--   0        0        0      262 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
--rw-r--r--   0        0        0     5539 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
--rw-r--r--   0        0        0     3524 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
--rw-r--r--   0        0        0      660 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
--rw-r--r--   0        0        0      120 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
--rw-r--r--   0        0        0     2045 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
--rw-r--r--   0        0        0     5682 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
--rw-r--r--   0        0        0     3505 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
--rw-r--r--   0        0        0     2481 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
--rw-r--r--   0        0        0     6201 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
--rw-r--r--   0        0        0     3963 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
--rw-r--r--   0        0        0      254 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
--rw-r--r--   0        0        0       87 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
--rw-r--r--   0        0        0      263 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
--rw-r--r--   0        0        0      415 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
--rw-r--r--   0        0        0     6232 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
--rw-r--r--   0        0        0    10500 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
--rw-r--r--   0        0        0      373 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
--rw-r--r--   0        0        0      261 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
--rw-r--r--   0        0        0      263 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
--rw-r--r--   0        0        0      261 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
--rw-r--r--   0        0        0     5655 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
--rw-r--r--   0        0        0     1961 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
--rw-r--r--   0        0        0     1824 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
--rw-r--r--   0        0        0     2502 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
--rw-r--r--   0        0        0     1046 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
--rw-r--r--   0        0        0      263 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
--rw-r--r--   0        0        0    18760 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
--rw-r--r--   0        0        0      172 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
--rw-r--r--   0        0        0    12130 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
--rw-r--r--   0        0        0     1267 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
--rw-r--r--   0        0        0    12938 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
--rw-r--r--   0        0        0     3704 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
--rw-r--r--   0        0        0    10597 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
--rw-r--r--   0        0        0    12040 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
--rw-r--r--   0        0        0     8007 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
--rw-r--r--   0        0        0    15325 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
--rw-r--r--   0        0        0    26419 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
--rw-r--r--   0        0        0     6471 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
--rw-r--r--   0        0        0      513 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
--rw-r--r--   0        0        0     8549 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.744507 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
--rw-r--r--   0        0        0     5233 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
--rw-r--r--   0        0        0     4475 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
--rw-r--r--   0        0        0     1644 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
--rw-r--r--   0        0        0     2905 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
--rw-r--r--   0        0        0     6158 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
--rw-r--r--   0        0        0     2185 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
--rw-r--r--   0        0        0     2147 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
--rw-r--r--   0        0        0     7453 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
--rw-r--r--   0        0        0     2289 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
--rw-r--r--   0        0        0     2594 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
--rw-r--r--   0        0        0     3377 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
--rw-r--r--   0        0        0      936 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
--rw-r--r--   0        0        0    17633 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
--rw-r--r--   0        0        0     7562 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
--rw-r--r--   0        0        0     1894 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
--rw-r--r--   0        0        0      398 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
--rw-r--r--   0        0        0     1973 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
--rw-r--r--   0        0        0     3041 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
--rw-r--r--   0        0        0      397 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
--rw-r--r--   0        0        0      561 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
--rw-r--r--   0        0        0     2501 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
--rw-r--r--   0        0        0     9989 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
--rw-r--r--   0        0        0      482 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
--rw-r--r--   0        0        0      879 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
--rw-r--r--   0        0        0     1000 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
--rw-r--r--   0        0        0     2747 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
--rw-r--r--   0        0        0      173 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
--rw-r--r--   0        0        0      131 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/__init__.py
--rw-r--r--   0        0        0    11747 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
--rw-r--r--   0        0        0    12689 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
--rw-r--r--   0        0        0     7524 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/service.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/__init__.py
--rw-r--r--   0        0        0     5601 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/analyzer.py
--rw-r--r--   0        0        0       53 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/exceptions.py
--rw-r--r--   0        0        0     8187 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/identities.py
--rw-r--r--   0        0        0     1331 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/model.py
--rw-r--r--   0        0        0    10555 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
--rw-r--r--   0        0        0     2448 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/service/model.py
--rw-r--r--   0        0        0     1425 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/service/scim.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
--rw-r--r--   0        0        0    17422 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
--rw-r--r--   0        0        0     6172 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
--rw-r--r--   0        0        0     2527 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
--rw-r--r--   0        0        0     5892 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
--rw-r--r--   0        0        0     2394 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
--rw-r--r--   0        0        0     2197 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/model.py
--rw-r--r--   0        0        0     1553 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
--rw-r--r--   0        0        0     1448 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/service.py
--rw-r--r--   0        0        0     1196 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/service_model.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/__init__.py
--rw-r--r--   0        0        0    10604 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/analyzer.py
--rw-r--r--   0        0        0       71 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
--rw-r--r--   0        0        0      369 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
--rw-r--r--   0        0        0      272 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
--rw-r--r--   0        0        0      313 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
--rw-r--r--   0        0        0     2404 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
--rw-r--r--   0        0        0      822 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/deployment.py
--rw-r--r--   0        0        0     2687 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/exporter.py
--rw-r--r--   0        0        0     1891 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/model.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/__init__.py
--rw-r--r--   0        0        0    11532 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
--rw-r--r--   0        0        0      389 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
--rw-r--r--   0        0        0       20 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
--rw-r--r--   0        0        0       11 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
--rw-r--r--   0        0        0      535 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
--rw-r--r--   0        0        0     5827 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/exporter.py
--rw-r--r--   0        0        0     4685 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/model.py
--rw-r--r--   0        0        0     1048 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/service.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/errors/__init__.py
--rw-r--r--   0        0        0       45 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/errors/failed_connection_errors.py
--rw-r--r--   0        0        0     6861 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/main.py
--rw-r--r--   0        0        0      195 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/models/__init__.py
--rw-r--r--   0        0        0     7583 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/models/model.py
--rw-r--r--   0        0        0        0 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/utils/__init__.py
--rw-r--r--   0        0        0      651 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/utils/logger.py
--rw-r--r--   0        0        0      452 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/writers/__init__.py
--rw-r--r--   0        0        0     1020 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/writers/base_writers.py
--rw-r--r--   0        0        0      728 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/writers/csv_writer.py
--rw-r--r--   0        0        0     1138 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/writers/get_writers.py
--rw-r--r--   0        0        0     2090 2023-05-02 09:23:48.748508 udps-0.1.14/universal_data_permissions_scanner/writers/multi_json_exporter.py
--rw-r--r--   0        0        0     5181 1970-01-01 00:00:00.000000 udps-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-24 12:19:37.775359 udps-0.1.15/LICENSE
+-rw-r--r--   0        0        0     2471 2023-05-24 12:19:37.775359 udps-0.1.15/README.md
+-rw-r--r--   0        0        0     3071 2023-05-24 12:19:37.779359 udps-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-24 12:19:37.779359 udps-0.1.15/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.779359 udps-0.1.15/tests/mocks/__init__.py
+-rw-r--r--   0        0        0      721 2023-05-24 12:19:37.779359 udps-0.1.15/tests/mocks/mock_writers.py
+-rw-r--r--   0        0        0     1028 2023-05-24 12:19:37.779359 udps-0.1.15/tests/test_authz_analyzer.py
+-rw-r--r--   0        0        0     5931 2023-05-24 12:19:37.779359 udps-0.1.15/tests/test_cli.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.779359 udps-0.1.15/tests/test_writers/__init__.py
+-rw-r--r--   0        0        0     1355 2023-05-24 12:19:37.779359 udps-0.1.15/tests/test_writers/test_csv_writer.py
+-rw-r--r--   0        0        0      953 2023-05-24 12:19:37.779359 udps-0.1.15/tests/test_writers/test_multijson_writer.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0    14110 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json
+-rw-r--r--   0        0        0    11644 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json
+-rw-r--r--   0        0        0    14917 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json
+-rw-r--r--   0        0        0     9884 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json
+-rw-r--r--   0        0        0    20662 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json
+-rw-r--r--   0        0        0    31812 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json
+-rw-r--r--   0        0        0    18235 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json
+-rw-r--r--   0        0        0    17618 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json
+-rw-r--r--   0        0        0     7529 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json
+-rw-r--r--   0        0        0     7744 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json
+-rw-r--r--   0        0        0     4073 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json
+-rw-r--r--   0        0        0    24204 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json
+-rw-r--r--   0        0        0    20163 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json
+-rw-r--r--   0        0        0    13494 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json
+-rw-r--r--   0        0        0     8446 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json
+-rw-r--r--   0        0        0    16466 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json
+-rw-r--r--   0        0        0    16126 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json
+-rw-r--r--   0        0        0    14831 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json
+-rw-r--r--   0        0        0     3066 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json
+-rw-r--r--   0        0        0     5550 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json
+-rw-r--r--   0        0        0     5906 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json
+-rw-r--r--   0        0        0     4446 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json
+-rw-r--r--   0        0        0     8937 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json
+-rw-r--r--   0        0        0    20162 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json
+-rw-r--r--   0        0        0    10324 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json
+-rw-r--r--   0        0        0     6886 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json
+-rw-r--r--   0        0        0    23422 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json
+-rw-r--r--   0        0        0     2358 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json
+-rw-r--r--   0        0        0     7124 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json
+-rw-r--r--   0        0        0     4549 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json
+-rw-r--r--   0        0        0     5215 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json
+-rw-r--r--   0        0        0     5987 2023-05-24 12:19:37.779359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json
+-rw-r--r--   0        0        0     5862 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json
+-rw-r--r--   0        0        0     3396 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json
+-rw-r--r--   0        0        0     2298 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json
+-rw-r--r--   0        0        0     5264 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json
+-rw-r--r--   0        0        0     4596 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json
+-rw-r--r--   0        0        0     3653 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json
+-rw-r--r--   0        0        0     4392 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json
+-rw-r--r--   0        0        0    26158 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json
+-rw-r--r--   0        0        0    10097 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json
+-rw-r--r--   0        0        0     8580 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json
+-rw-r--r--   0        0        0    33775 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json
+-rw-r--r--   0        0        0    16439 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json
+-rw-r--r--   0        0        0    13955 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json
+-rw-r--r--   0        0        0    18162 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json
+-rw-r--r--   0        0        0     3040 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json
+-rw-r--r--   0        0        0     5254 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json
+-rw-r--r--   0        0        0     3569 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json
+-rw-r--r--   0        0        0     4436 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json
+-rw-r--r--   0        0        0    14441 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json
+-rw-r--r--   0        0        0     3582 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py
+-rw-r--r--   0        0        0     4890 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py
+-rw-r--r--   0        0        0     4842 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0     2831 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py
+-rw-r--r--   0        0        0     1595 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json
+-rw-r--r--   0        0        0     3805 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json
+-rw-r--r--   0        0        0     2597 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json
+-rw-r--r--   0        0        0     2321 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json
+-rw-r--r--   0        0        0     4018 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json
+-rw-r--r--   0        0        0     5298 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json
+-rw-r--r--   0        0        0     1579 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/test_exporter.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/utils/__init__.py
+-rw-r--r--   0        0        0     1731 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0     5596 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/bigquery/generate_authz_entry.py
+-rw-r--r--   0        0        0     7137 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/bigquery/mocks.py
+-rw-r--r--   0        0        0    15539 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/bigquery/test_bigquery.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/databricks/__init__.py
+-rw-r--r--   0        0        0    17596 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/databricks/generate_authz_entry.py
+-rw-r--r--   0        0        0     9136 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/databricks/mocks.py
+-rw-r--r--   0        0        0    13149 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/databricks/test_analyzer.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    14532 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/mongodb/test_atlas_organization_users.py
+-rw-r--r--   0        0        0     7391 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/mongodb/test_mongodb.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/postgres/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/postgres/mocks/__init__.py
+-rw-r--r--   0        0        0     1195 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py
+-rw-r--r--   0        0        0    12910 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/postgres/test_postgress_analyzer.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/redshift/__init__.py
+-rw-r--r--   0        0        0    12179 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/redshift/test_redshift.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    18443 2023-05-24 12:19:37.783359 udps-0.1.15/tests/tests_datastores/snowflake/test_snowflake_analyzer.py
+-rw-r--r--   0        0        0     1086 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/__init__.py
+-rw-r--r--   0        0        0    10292 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/cli.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/__init__.py
+-rw-r--r--   0        0        0      626 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/__init__.py
+-rw-r--r--   0        0        0      113 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/__init__.py
+-rw-r--r--   0        0        0     3252 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py
+-rw-r--r--   0        0        0     7808 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/__init__.py
+-rw-r--r--   0        0        0    13042 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py
+-rw-r--r--   0        0        0       90 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_databases.sql
+-rw-r--r--   0        0        0      141 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/all_tables.sql
+-rw-r--r--   0        0        0      111 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_consumers.sql
+-rw-r--r--   0        0        0       14 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashare_desc.sql
+-rw-r--r--   0        0        0      125 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/datashares.sql
+-rw-r--r--   0        0        0      893 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql
+-rw-r--r--   0        0        0      262 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities_privileges.sql
+-rw-r--r--   0        0        0     5539 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py
+-rw-r--r--   0        0        0     3524 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py
+-rw-r--r--   0        0        0      660 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py
+-rw-r--r--   0        0        0      120 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/__init__.py
+-rw-r--r--   0        0        0     3041 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py
+-rw-r--r--   0        0        0     2045 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/__init__.py
+-rw-r--r--   0        0        0     5682 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py
+-rw-r--r--   0        0        0     3505 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py
+-rw-r--r--   0        0        0     2481 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py
+-rw-r--r--   0        0        0     6201 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py
+-rw-r--r--   0        0        0     3963 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py
+-rw-r--r--   0        0        0      254 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/__init__.py
+-rw-r--r--   0        0        0       87 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/effect.py
+-rw-r--r--   0        0        0      263 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/group_policy.py
+-rw-r--r--   0        0        0      415 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy.py
+-rw-r--r--   0        0        0     6232 2023-05-24 12:19:37.783359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py
+-rw-r--r--   0        0        0    10500 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py
+-rw-r--r--   0        0        0      373 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_utils.py
+-rw-r--r--   0        0        0      261 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/user_policy.py
+-rw-r--r--   0        0        0      263 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/public_block_access_config.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/__init__.py
+-rw-r--r--   0        0        0      261 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/role/role_policy.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/__init__.py
+-rw-r--r--   0        0        0     5655 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py
+-rw-r--r--   0        0        0     1961 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py
+-rw-r--r--   0        0        0     1824 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py
+-rw-r--r--   0        0        0     2502 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py
+-rw-r--r--   0        0        0     1046 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py
+-rw-r--r--   0        0        0      263 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/__init__.py
+-rw-r--r--   0        0        0    18760 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py
+-rw-r--r--   0        0        0      172 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/__init__.py
+-rw-r--r--   0        0        0    12130 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py
+-rw-r--r--   0        0        0     1267 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py
+-rw-r--r--   0        0        0    12938 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py
+-rw-r--r--   0        0        0     3704 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py
+-rw-r--r--   0        0        0    10597 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/__init__.py
+-rw-r--r--   0        0        0    12040 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py
+-rw-r--r--   0        0        0     8007 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py
+-rw-r--r--   0        0        0    15325 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py
+-rw-r--r--   0        0        0    26419 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py
+-rw-r--r--   0        0        0     6471 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py
+-rw-r--r--   0        0        0      513 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py
+-rw-r--r--   0        0        0     8549 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/__init__.py
+-rw-r--r--   0        0        0     5233 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py
+-rw-r--r--   0        0        0     4475 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py
+-rw-r--r--   0        0        0     1644 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/__init__.py
+-rw-r--r--   0        0        0     2905 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py
+-rw-r--r--   0        0        0     6158 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py
+-rw-r--r--   0        0        0     2185 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/__init__.py
+-rw-r--r--   0        0        0     2147 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py
+-rw-r--r--   0        0        0     7453 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py
+-rw-r--r--   0        0        0     2289 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py
+-rw-r--r--   0        0        0     2594 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/__init__.py
+-rw-r--r--   0        0        0     3377 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py
+-rw-r--r--   0        0        0      936 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py
+-rw-r--r--   0        0        0    17633 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py
+-rw-r--r--   0        0        0     7562 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py
+-rw-r--r--   0        0        0     1894 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py
+-rw-r--r--   0        0        0      398 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_base.py
+-rw-r--r--   0        0        0     1973 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py
+-rw-r--r--   0        0        0     3041 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py
+-rw-r--r--   0        0        0      397 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_base.py
+-rw-r--r--   0        0        0      561 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py
+-rw-r--r--   0        0        0     2501 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py
+-rw-r--r--   0        0        0     9989 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/__init__.py
+-rw-r--r--   0        0        0      482 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/assume_role.py
+-rw-r--r--   0        0        0      879 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py
+-rw-r--r--   0        0        0     1000 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py
+-rw-r--r--   0        0        0     2747 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py
+-rw-r--r--   0        0        0      173 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/serde.py
+-rw-r--r--   0        0        0      131 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/__init__.py
+-rw-r--r--   0        0        0    11747 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/analyzer.py
+-rw-r--r--   0        0        0    12689 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py
+-rw-r--r--   0        0        0     7740 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/service.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/__init__.py
+-rw-r--r--   0        0        0     5601 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/analyzer.py
+-rw-r--r--   0        0        0       53 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/exceptions.py
+-rw-r--r--   0        0        0     8187 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/identities.py
+-rw-r--r--   0        0        0     1331 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/model.py
+-rw-r--r--   0        0        0    10555 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/policy_tree.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/service/__init__.py
+-rw-r--r--   0        0        0     2448 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/service/model.py
+-rw-r--r--   0        0        0     1425 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/service/scim.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/analyzer.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/__init__.py
+-rw-r--r--   0        0        0    17422 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py
+-rw-r--r--   0        0        0     6172 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py
+-rw-r--r--   0        0        0     2527 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py
+-rw-r--r--   0        0        0     5892 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py
+-rw-r--r--   0        0        0     2394 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py
+-rw-r--r--   0        0        0     2197 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/model.py
+-rw-r--r--   0        0        0     1553 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/resolvers.py
+-rw-r--r--   0        0        0     1448 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/service.py
+-rw-r--r--   0        0        0     1196 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/service_model.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/__init__.py
+-rw-r--r--   0        0        0    10604 2023-05-24 12:19:37.787359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/analyzer.py
+-rw-r--r--   0        0        0       71 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/commands/all_databases.sql
+-rw-r--r--   0        0        0      369 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/commands/all_tables.sql
+-rw-r--r--   0        0        0      272 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/commands/roles.sql
+-rw-r--r--   0        0        0      313 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/commands/roles_grants.sql
+-rw-r--r--   0        0        0     2404 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/database_query_results.py
+-rw-r--r--   0        0        0      822 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/deployment.py
+-rw-r--r--   0        0        0     2687 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/exporter.py
+-rw-r--r--   0        0        0     1891 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/model.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/__init__.py
+-rw-r--r--   0        0        0    12641 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/analyzer.py
+-rw-r--r--   0        0        0      389 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/commands/grants_roles.sql
+-rw-r--r--   0        0        0       20 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/commands/grants_to_share.sql
+-rw-r--r--   0        0        0       11 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/commands/shares.sql
+-rw-r--r--   0        0        0      535 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql
+-rw-r--r--   0        0        0     5827 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/exporter.py
+-rw-r--r--   0        0        0     4685 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/model.py
+-rw-r--r--   0        0        0     1048 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/service.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/errors/__init__.py
+-rw-r--r--   0        0        0       45 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/errors/failed_connection_errors.py
+-rw-r--r--   0        0        0     6980 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/main.py
+-rw-r--r--   0        0        0      195 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/models/__init__.py
+-rw-r--r--   0        0        0     7583 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/models/model.py
+-rw-r--r--   0        0        0        0 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/utils/__init__.py
+-rw-r--r--   0        0        0      651 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/utils/logger.py
+-rw-r--r--   0        0        0      452 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/writers/__init__.py
+-rw-r--r--   0        0        0     1020 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/writers/base_writers.py
+-rw-r--r--   0        0        0      728 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/writers/csv_writer.py
+-rw-r--r--   0        0        0     1138 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/writers/get_writers.py
+-rw-r--r--   0        0        0     2090 2023-05-24 12:19:37.791359 udps-0.1.15/universal_data_permissions_scanner/writers/multi_json_exporter.py
+-rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 udps-0.1.15/PKG-INFO
```

### Comparing `udps-0.1.14/LICENSE` & `udps-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/README.md` & `udps-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/pyproject.toml` & `udps-0.1.15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "udps"
-version = "0.1.14"
+version = "0.1.15"
 homepage = "https://github.com/satoricyber/universal-data-permissions-scanner"
 description = "Analyze authorization."
 authors = ["SatoriCyber"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
```

### Comparing `udps-0.1.14/tests/mocks/mock_writers.py` & `udps-0.1.15/tests/mocks/mock_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/test_authz_analyzer.py` & `udps-0.1.15/tests/test_authz_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/test_cli.py` & `udps-0.1.15/tests/test_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,52 @@
             'host',
             '--warehouse',
             'warehouse',
         ],
     )
 
 
+@patch('universal_data_permissions_scanner.cli.run_snowflake', MagicMock())
+def test_snowflake_private_key():
+    invoke(
+        cli.snowflake,
+        [
+            '--username',
+            'user',
+            '--rsa-key',
+            '-',
+            '--rsa-pass',
+            'rsa-pass',
+            '--account',
+            'account',
+            '--host',
+            'host',
+            '--warehouse',
+            'warehouse',
+        ],
+    )
+
+
+@patch('universal_data_permissions_scanner.cli.run_snowflake', MagicMock())
+def test_snowflake_no_pass_no_key():
+    invoke(
+        cli.snowflake,
+        [
+            '--username',
+            'user',
+            '--account',
+            'account',
+            '--host',
+            'host',
+            '--warehouse',
+            'warehouse',
+        ],
+    )
+
+
 @pytest.mark.parametrize('additional_args', [[], ['--key-file', 'key_file_path']], ids=['basic', 'key-file'])
 @patch('universal_data_permissions_scanner.cli.run_bigquery', MagicMock())
 def test_bigquery(additional_args: List[str]):
     args = ['--project', 'proj1']
     args.extend(additional_args)
     invoke(cli.bigquery, args)
```

### Comparing `udps-0.1.14/tests/test_writers/test_csv_writer.py` & `udps-0.1.15/tests/test_writers/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/test_writers/test_multijson_writer.py` & `udps-0.1.15/tests/test_writers/test_multijson_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/action_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/action/assume_role_actions_for_principal_type.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/deny_with_condition/deny_with_condition_on_s3_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/federated_user_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/federated_user/iam_user_to_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_2_groups_includng_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_and_attached_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_groups/iam_user_with_group_simple_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_identity_center/iam_identity_center_with_users_and_groups.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_cross_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_to_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/assume_role_via_resourve_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/simple_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_roles/valid_assume_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_attached_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_and_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/iam_user_to_s3_bucket/iam_user_with_inline_policy_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/iam_users_to_s3_cross_account_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/multi_iam_users_to_multi_s3_buckets/multi_iam_users_to_multi_s3_buckets.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/assume_role_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/federated_users_with_not_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_combinations_in_both_allow_and_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_in_all_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_including_wildcard_object_regex_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_multiple_wildcard_regexes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/no_resource/iam_user_with_not_resource_on_no_valid_resource_arn_deny.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_allowed_no_action_s3_complement.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_multiple_actions_in_no_action_resource.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_simple.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_action/iam_user_with_resource_no_action_wildcard_action_set.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_roles_and_federated_with_deny_not_principal_single_account.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/not_principal/iam_users_with_deny_not_principal_cross_accounts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/irrelevant_principal_types.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/principal/principal_resolving_via_resource_based.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_assume_role.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/resource/resouce_resolving_s3.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_default.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_on_object_multi_stmts.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_and_allow_with_one_resource_in_deny_that_is_a_subgroup_of_all_in_allow.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/deny_on_object_and_allow_bucket.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/resolve_permissions_test_inputs/s3_resource_regex/valid_actions_objects_and_actions_resources.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_create_session_with_assume_role.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_resolve_permissions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/test_satori_dev_account_ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py` & `udps-0.1.15/tests/tests_datastores/aws/aws_ptrp/utils/aws_ptrp_load_from_dict.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_basic_iam_user_and_policy_path.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_iam_identity_center_user_and_group.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_multiple_roles_in_path_and_all_principals.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_federated_user.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_iam_group_and_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json` & `udps-0.1.15/tests/tests_datastores/aws/exporter_test_inputs/ptrp_line_with_notes.json`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/test_exporter.py` & `udps-0.1.15/tests/tests_datastores/aws/test_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py` & `udps-0.1.15/tests/tests_datastores/aws/utils/test_aws_regex_full_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/bigquery/generate_authz_entry.py` & `udps-0.1.15/tests/tests_datastores/bigquery/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/bigquery/mocks.py` & `udps-0.1.15/tests/tests_datastores/bigquery/mocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,15 +135,17 @@
             iam_client=iam_client,
             org_iam_client=org_iam_client,
             project_iam_client=project_iam_client,
         )
         return service
 
     def _side_effect_get_iam_policy_project(self, request: iam_policy_pb2.GetIamPolicyRequest) -> MockedIam:
-        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(resource=f"projects/{self.project.project_id}")
+        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(
+            resource=f"projects/{self.project.project_id}"
+        )  # pyright: ignore [reportGeneralTypeIssues]
         if request == expected_iam_policy:
             return MockedIam(bindings=self.project_bindings)
         raise ValueError(f"Unexpected request: {request}")
 
     def _side_effect_get_iam_policy_bq_client(self, request: str) -> MockedTableIamPolicy:
         return self.tables_policies.get(request, MockedTableIamPolicy(bindings=[]))
 
@@ -164,27 +166,31 @@
         assert self.folder is not None
         expected = resourcemanager_v3.GetFolderRequest(name=self.folder.name)
         assert request == expected
         return self.folder
 
     def _side_effect_get_iam_policy_folder(self, request: iam_policy_pb2.GetIamPolicyRequest) -> MockedIam:
         assert self.folder is not None
-        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(resource=f"{self.folder.name}")
+        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(
+            resource=f"{self.folder.name}"
+        )  # pyright: ignore [reportGeneralTypeIssues]
         assert request == expected_iam_policy
         return MockedIam(bindings=self.folder.bindings)
 
     def _side_effect_get_organization(self, request: resourcemanager_v3.GetOrganizationRequest) -> MockedOrganization:
         assert self.organization is not None
         expected = resourcemanager_v3.GetOrganizationRequest(name=self.organization.name)
         assert request == expected
         return self.organization
 
     def _side_effect_get_iam_policy_organization(self, request: iam_policy_pb2.GetIamPolicyRequest) -> MockedIam:
         assert self.organization is not None
-        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(resource=f"{self.organization.name}")
+        expected_iam_policy = iam_policy_pb2.GetIamPolicyRequest(
+            resource=f"{self.organization.name}"
+        )  # pyright: ignore [reportGeneralTypeIssues]
         assert request == expected_iam_policy
         return MockedIam(bindings=self.organization.bindings)
 
     def _side_effect_iam_client_roles(self):
         roles = MagicMock()
         roles.get = MagicMock(side_effect=self._side_effect_iam_client_get_role)
         return roles
```

### Comparing `udps-0.1.14/tests/tests_datastores/bigquery/test_bigquery.py` & `udps-0.1.15/tests/tests_datastores/bigquery/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/databricks/generate_authz_entry.py` & `udps-0.1.15/tests/tests_datastores/databricks/generate_authz_entry.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/databricks/mocks.py` & `udps-0.1.15/tests/tests_datastores/databricks/mocks.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/databricks/test_analyzer.py` & `udps-0.1.15/tests/tests_datastores/databricks/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/mongodb/test_atlas_organization_users.py` & `udps-0.1.15/tests/tests_datastores/mongodb/test_atlas_organization_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/mongodb/test_mongodb.py` & `udps-0.1.15/tests/tests_datastores/mongodb/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py` & `udps-0.1.15/tests/tests_datastores/postgres/mocks/postgres_mock_connector.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/postgres/test_postgress_analyzer.py` & `udps-0.1.15/tests/tests_datastores/postgres/test_postgress_analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/tests/tests_datastores/redshift/test_redshift.py` & `udps-0.1.15/tests/tests_datastores/redshift/test_redshift.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/__init__.py` & `udps-0.1.15/universal_data_permissions_scanner/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for authz-analyzer."""
 
 __author__ = """SatoriCyber"""
 __email__ = 'contact@satoricyber.com'
-__version__ = '0.1.14'
+__version__ = '0.1.15'
 
 from universal_data_permissions_scanner.datastores.aws.analyzer import AwsAssumeRoleInput, AWSAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.aws.analyzer.redshift.analyzer import RedshiftAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.bigquery.analyzer import BigQueryAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.analyzer import MongoDBAuthzAnalyzer  # type: ignore
 from universal_data_permissions_scanner.datastores.mongodb.atlas.analyzer import MongoDBAtlasAuthzAnalyzer  # type: ignore
```

### Comparing `udps-0.1.14/universal_data_permissions_scanner/cli.py` & `udps-0.1.15/universal_data_permissions_scanner/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Console script for authz_analyzer."""
 import os
 import re
 import sys
 from pathlib import Path
-from typing import List, Optional
+from typing import List, Optional, TextIO
 
 import click
 
 if sys.executable != sys.argv[0]:
     sys.path.insert(0, (os.path.join(os.path.dirname(__file__), "..")))
 
 
@@ -55,22 +55,43 @@
     logger = get_logger(debug)
     ctx.obj['LOGGER'] = logger
 
 
 @main.command()
 @click.pass_context
 @click.option('--username', '-u', required=True, type=str, help="Username")
-@click.option('--password', '-p', required=True, type=str, help="Password")
+@click.option('--password', '-p', required=False, type=str, help="Password")
+@click.option('--rsa-key', '-r', required=False, type=click.File('r'), help="Path to RSA private key")
+@click.option('--rsa-pass', required=False, type=str, help="RSA key password")
 @click.option('--account', '-a', required=True, type=str, help="Account")
 @click.option('--host', '-t', required=False, type=str, help="Hostname")
 @click.option('--warehouse', '-w', required=False, type=str, help="Warehouse")
-def snowflake(ctx: click.Context, username: str, password: str, account: str, host: str, warehouse: str):
+def snowflake(
+    ctx: click.Context,
+    username: str,
+    password: Optional[str],
+    account: str,
+    host: str,
+    warehouse: str,
+    rsa_key: Optional[TextIO],
+    rsa_pass: Optional[str],
+):
     """Analyze Snowflake Authorization"""
+    if not any([password, rsa_key]):
+        click.echo('Error: Required at least one of the options: --password / -p or --rsa / -r')
+        return
+
+    rsa: Optional[str] = None
+    if rsa_key is not None:
+        rsa = rsa_key.read()
+
     output_path = Path(ctx.obj['OUT'])
-    run_snowflake(ctx.obj['LOGGER'], username, password, account, host, warehouse, ctx.obj["FORMAT"], output_path)
+    run_snowflake(
+        ctx.obj['LOGGER'], username, password, account, host, warehouse, ctx.obj["FORMAT"], output_path, rsa, rsa_pass
+    )
 
 
 @main.command()
 @click.pass_context
 @click.option('--project', '-p', required=True, type=str, help="GCP project ID, for example: acme-webapp-prod")
 @click.option('--key-file', '-k', required=False, type=str, help="Path to GCP service account file")
 def bigquery(ctx: click.Context, project: str, key_file: Optional[str] = None):
```

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/__init__.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/commands/identities.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/analyzer/redshift/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/actions_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/actions/aws_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_policies.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_roles.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/iam_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam/policy/policy_document_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_entities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_groups.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/iam_identity_center_users.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/iam_identity_center/permission_sets.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/policy_evaluation/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/aws_principals.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/no_entity_principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principal.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/principals/principals_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_node_notes.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_line_nodes_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_allowed_lines/allowed_lines_resolver_result.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/ptrp_models/ptrp_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/account_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/resources/resources_resolver.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/__init__.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/assume_role/assume_role_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/federated_user/federated_user_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/resolved_stmt.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/bucket_acl.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_actions.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_resources.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/s3/s3_service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_action_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_actions_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resource_type.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/services/service_resources_resolver_base.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/create_session.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/aws/aws_ptrp_package/aws_ptrp/utils/regex_subset.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/bigquery/service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/bigquery/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from typing import Any, Callable, List, Optional
 
 import googleapiclient.discovery  # pylint: disable=import-error
 from google.cloud import bigquery, resourcemanager_v3  # pylint: disable=no-name-in-module
+from google.api_core.iam import Policy
 from google.cloud.resourcemanager_v3.types import Project  # pylint: disable=no-name-in-module
 from google.iam.v1 import iam_policy_pb2  # type: ignore
 
 from universal_data_permissions_scanner.datastores.bigquery.policy_tree import CustomPermission, IamPolicyNode
 
 
 @dataclass
@@ -52,31 +53,33 @@
 
     @staticmethod
     def _get_project(projects_client: resourcemanager_v3.ProjectsClient, project_id: str):
         request = resourcemanager_v3.GetProjectRequest(name=f"projects/{project_id}")
         return projects_client.get_project(request=request)  # type: ignore
 
     def _get_project_iam(self):
-        request = iam_policy_pb2.GetIamPolicyRequest(resource=f"projects/{self.project_id}")
+        request = iam_policy_pb2.GetIamPolicyRequest(
+            resource=f"projects/{self.project_id}"
+        )  # pyright: ignore [reportGeneralTypeIssues]
         return self.projects_client.get_iam_policy(request=request)  # type: ignore
 
     def _get_folder(self, folder_id: str):
         request = resourcemanager_v3.GetFolderRequest(name=folder_id)
         return self.folders_client.get_folder(request=request)  # type: ignore
 
-    def _get_folder_iam(self, folder_id: str):
-        request = iam_policy_pb2.GetIamPolicyRequest(resource=folder_id)
+    def _get_folder_iam(self, folder_id: str) -> Policy:
+        request = iam_policy_pb2.GetIamPolicyRequest(resource=folder_id)  # pyright: ignore [reportGeneralTypeIssues]
         return self.folders_client.get_iam_policy(request=request)  # type: ignore
 
     def _get_organization(self, org_id: str):
         request = resourcemanager_v3.GetOrganizationRequest(name=org_id)
         return self.org_client.get_organization(request=request)  # type: ignore
 
-    def _get_organization_iam(self, org_id: str):
-        request = iam_policy_pb2.GetIamPolicyRequest(resource=org_id)
+    def _get_organization_iam(self, org_id: str) -> Policy:
+        request = iam_policy_pb2.GetIamPolicyRequest(resource=org_id)  # pyright: ignore [reportGeneralTypeIssues]
         return self.org_client.get_iam_policy(request=request)  # type: ignore
 
     def list_datasets(self) -> List[str]:
         """List all datasets in the GCP project
 
         Returns:
             List[str]: A list of all dataset IDs
```

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/identities.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/identities.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/policy_tree.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/policy_tree.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/service/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/service/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/databricks/service/scim.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/databricks/service/scim.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/permission_resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/atlas/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/resolvers.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/resolvers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/mongodb/service_model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/mongodb/service_model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/analyzer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/database_query_results.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/database_query_results.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/deployment.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/deployment.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/exporter.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/postgres/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/postgres/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/analyzer.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/analyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 
 from dataclasses import dataclass
 from logging import Logger
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 import snowflake.connector
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import serialization
 
 from universal_data_permissions_scanner.datastores.snowflake import exporter
 from universal_data_permissions_scanner.datastores.snowflake.model import (
     PERMISSION_LEVEL_MAP,
     AuthorizationModel,
     DataShare,
     DataShareKind,
@@ -56,50 +58,55 @@
     """Analyze authorization for Snowflake."""
 
     service: SnowflakeService
     writer: BaseWriter
     logger: Logger
 
     @classmethod
-    def connect(
+    def connect(  # pylint: disable=too-many-locals
         cls,
         host: str,
         account: str,
         username: str,
-        password: str,
         warehouse: str,
         logger: Optional[Logger] = None,
         output_format: OutputFormat = OutputFormat.CSV,
         output_path: Union[Path, str] = Path.cwd() / DEFAULT_OUTPUT_FILE,
+        rsa_key: Optional[str] = None,
+        rsa_pass: Optional[str] = None,
         **snowflake_connection_kwargs: Any,
     ):
         """Connect to Snowflake and return an analyzer.
 
         Args:
             host (str): Snowflake host
             account (str): Snowflake account
             username (str): Snowflake username to connect with
-            password (str): Snowflake password to connect with
+            password (Optional[str]): Snowflake password to connect with
+            rsa_key: (Optional[str]): Snowflake rsa key to connect with
+            rsa_pass: (Optional[str]): RSA password to decrypt rsa key
             warehouse (str): Snowflake warehouse to use
             logger (Optional[Logger], optional): Python logger. Defaults to None.
             output_path (Union[Path, str], optional): Path to write the file. Defaults to ./authz-analyzer-export.
             output_format (OutputFormat, optional): Output format. Defaults to OutputFormat.CSV.
         """
         if logger is None:
             logger = get_logger(False)
 
         writer = get_writer(filename=output_path, output_format=output_format)
 
         # Handle case sensitive warehouse name, wrap with quotes
         warehouse = f'"{warehouse}"'
 
+        if rsa_key is not None:
+            snowflake_connection_kwargs["private_key"] = SnowflakeAuthzAnalyzer._read_private_key(rsa_key, rsa_pass)
+
         try:
             connector = snowflake.connector.connect(  # type: ignore
                 user=username,
-                password=password,
                 host=host,
                 account=account,
                 warehouse=warehouse,
                 **snowflake_connection_kwargs,
             )
         except Exception as err:
             raise ConnectionFailure from err
@@ -137,14 +144,30 @@
             if role_name is not None:
                 role = DBRole.new(name=role_name, roles=set())
                 roles.add(role)
             roles.add(DBRole(name="PUBLIC", roles=set()))
         return results
 
     @staticmethod
+    def _read_private_key(key: str, password: Optional[str]):
+        """Convert private key to pkcs8 format - based on snowflake example"""
+        password_bytes: Optional[bytes] = None
+        if password is not None:
+            password_bytes = password.encode()
+
+        p_key = serialization.load_pem_private_key(key.encode(), password=password_bytes, backend=default_backend())
+
+        pkb = p_key.private_bytes(
+            encoding=serialization.Encoding.DER,
+            format=serialization.PrivateFormat.PKCS8,
+            encryption_algorithm=serialization.NoEncryption(),
+        )
+        return pkb
+
+    @staticmethod
     def _add_role_to_roles(role_name: str, granted_role_name: str, role_to_roles: Dict[str, Set[DBRole]]):
         role = role_to_roles.setdefault(role_name, set())
         granted_role = DBRole.new(name=granted_role_name, roles=set())
         role.add(granted_role)
 
     @staticmethod
     def _is_the_same_resource(
```

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql` & `udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/commands/user_grants.sql`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/exporter.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/model.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/datastores/snowflake/service.py` & `udps-0.1.15/universal_data_permissions_scanner/datastores/snowflake/service.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/main.py` & `udps-0.1.15/universal_data_permissions_scanner/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 
 from universal_data_permissions_scanner.datastores.databricks.analyzer import DatabricksAuthzAnalyzer
 
 
 def run_snowflake(
     logger: Logger,
     username: str,
-    password: str,
+    password: Optional[str],
     account: str,
     host: str,
     warehouse: str,
     output_format: OutputFormat,
     output_path: Path,
+    rsa_key: Optional[str],
+    rsa_pass: Optional[str],
 ):
     """Run snowflake analyzer.
 
     Args:
         logger (Logger): Logger
         username (str): Username
         password (str): Password
@@ -45,14 +47,16 @@
         username=username,
         password=password,
         warehouse=warehouse,
         account=account,
         output_path=output_path,
         output_format=output_format,
         logger=logger,
+        rsa_key=rsa_key,
+        rsa_pass=rsa_pass,
     )
     snowflake_analyzer.run()
 
 
 # AWS S3 runner
 def run_aws_s3(
     logger: Logger,
```

### Comparing `udps-0.1.14/universal_data_permissions_scanner/models/model.py` & `udps-0.1.15/universal_data_permissions_scanner/models/model.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/utils/logger.py` & `udps-0.1.15/universal_data_permissions_scanner/utils/logger.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/writers/base_writers.py` & `udps-0.1.15/universal_data_permissions_scanner/writers/base_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/writers/csv_writer.py` & `udps-0.1.15/universal_data_permissions_scanner/writers/csv_writer.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/writers/get_writers.py` & `udps-0.1.15/universal_data_permissions_scanner/writers/get_writers.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/universal_data_permissions_scanner/writers/multi_json_exporter.py` & `udps-0.1.15/universal_data_permissions_scanner/writers/multi_json_exporter.py`

 * *Files identical despite different names*

### Comparing `udps-0.1.14/PKG-INFO` & `udps-0.1.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: udps
-Version: 0.1.14
+Version: 0.1.15
 Summary: Analyze authorization.
 Home-page: https://github.com/satoricyber/universal-data-permissions-scanner
 Author: SatoriCyber
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: release
 Provides-Extra: test
 Requires-Dist: black (>=22.12.0,<23.0.0) ; extra == "test"
 Requires-Dist: boto3 (>=1.26.27,<2.0.0)
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "test"
 Requires-Dist: click (==8.1.3)
 Requires-Dist: databricks-cli (>=0.17.4,<0.18.0)
```

