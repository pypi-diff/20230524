# Comparing `tmp/cloudsmith_api-2.0.3-py2.py3-none-any.whl.zip` & `tmp/cloudsmith_api-2.0.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,413 +1,417 @@
-Zip file size: 723282 bytes, number of entries: 411
--rw-r--r--  2.0 unx    15910 b- defN 23-May-17 09:26 cloudsmith_api/__init__.py
--rw-r--r--  2.0 unx    25067 b- defN 23-May-17 09:26 cloudsmith_api/api_client.py
--rw-r--r--  2.0 unx     8390 b- defN 23-May-17 09:26 cloudsmith_api/configuration.py
--rw-r--r--  2.0 unx    13166 b- defN 23-May-17 09:26 cloudsmith_api/rest.py
--rw-r--r--  2.0 unx     1131 b- defN 23-May-17 09:26 cloudsmith_api/api/__init__.py
--rw-r--r--  2.0 unx    11039 b- defN 23-May-17 09:26 cloudsmith_api/api/audit_log_api.py
--rw-r--r--  2.0 unx    11425 b- defN 23-May-17 09:26 cloudsmith_api/api/badges_api.py
--rw-r--r--  2.0 unx     7978 b- defN 23-May-17 09:26 cloudsmith_api/api/distros_api.py
--rw-r--r--  2.0 unx    54786 b- defN 23-May-17 09:26 cloudsmith_api/api/entitlements_api.py
--rw-r--r--  2.0 unx    26620 b- defN 23-May-17 09:26 cloudsmith_api/api/files_api.py
--rw-r--r--  2.0 unx     7930 b- defN 23-May-17 09:26 cloudsmith_api/api/formats_api.py
--rw-r--r--  2.0 unx    19214 b- defN 23-May-17 09:26 cloudsmith_api/api/metrics_api.py
--rw-r--r--  2.0 unx     8514 b- defN 23-May-17 09:26 cloudsmith_api/api/namespaces_api.py
--rw-r--r--  2.0 unx   195413 b- defN 23-May-17 09:26 cloudsmith_api/api/orgs_api.py
--rw-r--r--  2.0 unx   284986 b- defN 23-May-17 09:26 cloudsmith_api/api/packages_api.py
--rw-r--r--  2.0 unx    16386 b- defN 23-May-17 09:26 cloudsmith_api/api/quota_api.py
--rw-r--r--  2.0 unx     4157 b- defN 23-May-17 09:26 cloudsmith_api/api/rates_api.py
--rw-r--r--  2.0 unx    98642 b- defN 23-May-17 09:26 cloudsmith_api/api/repos_api.py
--rw-r--r--  2.0 unx     4118 b- defN 23-May-17 09:26 cloudsmith_api/api/status_api.py
--rw-r--r--  2.0 unx     8075 b- defN 23-May-17 09:26 cloudsmith_api/api/storage_regions_api.py
--rw-r--r--  2.0 unx     7631 b- defN 23-May-17 09:26 cloudsmith_api/api/user_api.py
--rw-r--r--  2.0 unx     4706 b- defN 23-May-17 09:26 cloudsmith_api/api/users_api.py
--rw-r--r--  2.0 unx    22091 b- defN 23-May-17 09:26 cloudsmith_api/api/vulnerabilities_api.py
--rw-r--r--  2.0 unx    26050 b- defN 23-May-17 09:26 cloudsmith_api/api/webhooks_api.py
--rw-r--r--  2.0 unx    14713 b- defN 23-May-17 09:26 cloudsmith_api/models/__init__.py
--rw-r--r--  2.0 unx     7305 b- defN 23-May-17 09:26 cloudsmith_api/models/allocated_limit.py
--rw-r--r--  2.0 unx     5410 b- defN 23-May-17 09:26 cloudsmith_api/models/allocated_limit_raw.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/alpine_package_upload.py
--rw-r--r--  2.0 unx     7437 b- defN 23-May-17 09:26 cloudsmith_api/models/alpine_package_upload_request.py
--rw-r--r--  2.0 unx     4748 b- defN 23-May-17 09:26 cloudsmith_api/models/architecture.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/cargo_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-May-17 09:26 cloudsmith_api/models/cargo_package_upload_request.py
--rw-r--r--  2.0 unx    59602 b- defN 23-May-17 09:26 cloudsmith_api/models/cocoapods_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-May-17 09:26 cloudsmith_api/models/cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx     6052 b- defN 23-May-17 09:26 cloudsmith_api/models/common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     5636 b- defN 23-May-17 09:26 cloudsmith_api/models/common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx     6052 b- defN 23-May-17 09:26 cloudsmith_api/models/common_downloads_metrics.py
--rw-r--r--  2.0 unx     3526 b- defN 23-May-17 09:26 cloudsmith_api/models/common_downloads_metrics_value.py
--rw-r--r--  2.0 unx     6129 b- defN 23-May-17 09:26 cloudsmith_api/models/common_metrics.py
--rw-r--r--  2.0 unx    59325 b- defN 23-May-17 09:26 cloudsmith_api/models/composer_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-May-17 09:26 cloudsmith_api/models/composer_package_upload_request.py
--rw-r--r--  2.0 unx    61539 b- defN 23-May-17 09:26 cloudsmith_api/models/conan_package_upload.py
--rw-r--r--  2.0 unx    14491 b- defN 23-May-17 09:26 cloudsmith_api/models/conan_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/conda_package_upload.py
--rw-r--r--  2.0 unx     6177 b- defN 23-May-17 09:26 cloudsmith_api/models/conda_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/cran_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/cran_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/dart_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/dart_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/deb_package_upload.py
--rw-r--r--  2.0 unx     9690 b- defN 23-May-17 09:26 cloudsmith_api/models/deb_package_upload_request.py
--rw-r--r--  2.0 unx     6159 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution.py
--rw-r--r--  2.0 unx     8542 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution_full.py
--rw-r--r--  2.0 unx     4497 b- defN 23-May-17 09:26 cloudsmith_api/models/distribution_version.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/docker_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-May-17 09:26 cloudsmith_api/models/docker_package_upload_request.py
--rw-r--r--  2.0 unx     3541 b- defN 23-May-17 09:26 cloudsmith_api/models/entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     3729 b- defN 23-May-17 09:26 cloudsmith_api/models/error_detail.py
--rw-r--r--  2.0 unx     5458 b- defN 23-May-17 09:26 cloudsmith_api/models/eula.py
--rw-r--r--  2.0 unx    11287 b- defN 23-May-17 09:26 cloudsmith_api/models/format.py
--rw-r--r--  2.0 unx     7319 b- defN 23-May-17 09:26 cloudsmith_api/models/format_support.py
--rw-r--r--  2.0 unx     8615 b- defN 23-May-17 09:26 cloudsmith_api/models/geo_ip_location.py
--rw-r--r--  2.0 unx    57663 b- defN 23-May-17 09:26 cloudsmith_api/models/go_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-May-17 09:26 cloudsmith_api/models/go_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/helm_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/helm_package_upload_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/hex_package_upload.py
--rw-r--r--  2.0 unx     6143 b- defN 23-May-17 09:26 cloudsmith_api/models/hex_package_upload_request.py
--rw-r--r--  2.0 unx     7028 b- defN 23-May-17 09:26 cloudsmith_api/models/history.py
--rw-r--r--  2.0 unx     5168 b- defN 23-May-17 09:26 cloudsmith_api/models/history_fieldset.py
--rw-r--r--  2.0 unx     5246 b- defN 23-May-17 09:26 cloudsmith_api/models/history_fieldset_raw.py
--rw-r--r--  2.0 unx    59325 b- defN 23-May-17 09:26 cloudsmith_api/models/luarocks_package_upload.py
--rw-r--r--  2.0 unx     6228 b- defN 23-May-17 09:26 cloudsmith_api/models/luarocks_package_upload_request.py
--rw-r--r--  2.0 unx    61667 b- defN 23-May-17 09:26 cloudsmith_api/models/maven_package_upload.py
--rw-r--r--  2.0 unx    14513 b- defN 23-May-17 09:26 cloudsmith_api/models/maven_package_upload_request.py
--rw-r--r--  2.0 unx     5806 b- defN 23-May-17 09:26 cloudsmith_api/models/namespace.py
--rw-r--r--  2.0 unx    18223 b- defN 23-May-17 09:26 cloudsmith_api/models/namespace_audit_log.py
--rw-r--r--  2.0 unx    11620 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_license_policy.py
--rw-r--r--  2.0 unx    12280 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     9527 b- defN 23-May-17 09:26 cloudsmith_api/models/nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/npm_package_upload.py
--rw-r--r--  2.0 unx     7663 b- defN 23-May-17 09:26 cloudsmith_api/models/npm_package_upload_request.py
--rw-r--r--  2.0 unx    58494 b- defN 23-May-17 09:26 cloudsmith_api/models/nuget_package_upload.py
--rw-r--r--  2.0 unx     7272 b- defN 23-May-17 09:26 cloudsmith_api/models/nuget_package_upload_request.py
--rw-r--r--  2.0 unx     7918 b- defN 23-May-17 09:26 cloudsmith_api/models/organization.py
--rw-r--r--  2.0 unx     8391 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_group_sync.py
--rw-r--r--  2.0 unx     8223 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_group_sync_request.py
--rw-r--r--  2.0 unx    10169 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite.py
--rw-r--r--  2.0 unx    10519 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_extend.py
--rw-r--r--  2.0 unx     5661 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_request.py
--rw-r--r--  2.0 unx     3821 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_update.py
--rw-r--r--  2.0 unx     3929 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx    12300 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_membership.py
--rw-r--r--  2.0 unx    12219 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy.py
--rw-r--r--  2.0 unx     9666 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     9539 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx    12855 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx    10230 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx    10245 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx     8110 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team.py
--rw-r--r--  2.0 unx     3669 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_members.py
--rw-r--r--  2.0 unx     4783 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_membership.py
--rw-r--r--  2.0 unx     7065 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_request.py
--rw-r--r--  2.0 unx     7040 b- defN 23-May-17 09:26 cloudsmith_api/models/organization_team_request_patch.py
--rw-r--r--  2.0 unx    57663 b- defN 23-May-17 09:26 cloudsmith_api/models/p2_package_upload.py
--rw-r--r--  2.0 unx     6126 b- defN 23-May-17 09:26 cloudsmith_api/models/p2_package_upload_request.py
--rw-r--r--  2.0 unx    55965 b- defN 23-May-17 09:26 cloudsmith_api/models/package.py
--rw-r--r--  2.0 unx    57197 b- defN 23-May-17 09:26 cloudsmith_api/models/package_copy.py
--rw-r--r--  2.0 unx     4776 b- defN 23-May-17 09:26 cloudsmith_api/models/package_copy_request.py
--rw-r--r--  2.0 unx     3523 b- defN 23-May-17 09:26 cloudsmith_api/models/package_dependencies.py
--rw-r--r--  2.0 unx     7227 b- defN 23-May-17 09:26 cloudsmith_api/models/package_dependency.py
--rw-r--r--  2.0 unx    12968 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file.py
--rw-r--r--  2.0 unx     6108 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_parts_upload.py
--rw-r--r--  2.0 unx     7841 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_upload.py
--rw-r--r--  2.0 unx     7815 b- defN 23-May-17 09:26 cloudsmith_api/models/package_file_upload_request.py
--rw-r--r--  2.0 unx     6035 b- defN 23-May-17 09:26 cloudsmith_api/models/package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     5198 b- defN 23-May-17 09:26 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    57195 b- defN 23-May-17 09:26 cloudsmith_api/models/package_move.py
--rw-r--r--  2.0 unx     3820 b- defN 23-May-17 09:26 cloudsmith_api/models/package_move_request.py
--rw-r--r--  2.0 unx    58775 b- defN 23-May-17 09:26 cloudsmith_api/models/package_quarantine.py
--rw-r--r--  2.0 unx     3527 b- defN 23-May-17 09:26 cloudsmith_api/models/package_quarantine_request.py
--rw-r--r--  2.0 unx    57651 b- defN 23-May-17 09:26 cloudsmith_api/models/package_resync.py
--rw-r--r--  2.0 unx    15877 b- defN 23-May-17 09:26 cloudsmith_api/models/package_status.py
--rw-r--r--  2.0 unx    57199 b- defN 23-May-17 09:26 cloudsmith_api/models/package_tag.py
--rw-r--r--  2.0 unx     5352 b- defN 23-May-17 09:26 cloudsmith_api/models/package_tag_request.py
--rw-r--r--  2.0 unx     3547 b- defN 23-May-17 09:26 cloudsmith_api/models/package_usage_metrics.py
--rw-r--r--  2.0 unx     2740 b- defN 23-May-17 09:26 cloudsmith_api/models/package_version_badge.py
--rw-r--r--  2.0 unx     5707 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability.py
--rw-r--r--  2.0 unx     7491 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     5318 b- defN 23-May-17 09:26 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    58771 b- defN 23-May-17 09:26 cloudsmith_api/models/python_package_upload.py
--rw-r--r--  2.0 unx     6194 b- defN 23-May-17 09:26 cloudsmith_api/models/python_package_upload_request.py
--rw-r--r--  2.0 unx     3358 b- defN 23-May-17 09:26 cloudsmith_api/models/quota.py
--rw-r--r--  2.0 unx     3463 b- defN 23-May-17 09:26 cloudsmith_api/models/quota_history.py
--rw-r--r--  2.0 unx     7675 b- defN 23-May-17 09:26 cloudsmith_api/models/rate_check.py
--rw-r--r--  2.0 unx    58899 b- defN 23-May-17 09:26 cloudsmith_api/models/raw_package_upload.py
--rw-r--r--  2.0 unx    11674 b- defN 23-May-17 09:26 cloudsmith_api/models/raw_package_upload_request.py
--rw-r--r--  2.0 unx    66229 b- defN 23-May-17 09:26 cloudsmith_api/models/repository.py
--rw-r--r--  2.0 unx    14861 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_audit_log.py
--rw-r--r--  2.0 unx    67555 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_create.py
--rw-r--r--  2.0 unx    52996 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_create_request.py
--rw-r--r--  2.0 unx     4365 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     4488 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx     4424 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     4515 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     4312 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     3733 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     3906 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     7359 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx     8734 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_gpg_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_gpg_key_create.py
--rw-r--r--  2.0 unx     7702 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_dict.py
--rw-r--r--  2.0 unx     3818 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input.py
--rw-r--r--  2.0 unx     3881 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input_request.py
--rw-r--r--  2.0 unx     3790 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx    51807 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_request_patch.py
--rw-r--r--  2.0 unx     7753 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_rsa_key.py
--rw-r--r--  2.0 unx     5133 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_rsa_key_create.py
--rw-r--r--  2.0 unx    40544 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token.py
--rw-r--r--  2.0 unx     2750 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_action.py
--rw-r--r--  2.0 unx    41541 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_refresh.py
--rw-r--r--  2.0 unx    21868 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_refresh_request.py
--rw-r--r--  2.0 unx    22374 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_request.py
--rw-r--r--  2.0 unx    22569 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_request_patch.py
--rw-r--r--  2.0 unx     3505 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_sync.py
--rw-r--r--  2.0 unx     3904 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_token_sync_request.py
--rw-r--r--  2.0 unx    30728 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook.py
--rw-r--r--  2.0 unx    18912 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook_request.py
--rw-r--r--  2.0 unx    18774 b- defN 23-May-17 09:26 cloudsmith_api/models/repository_webhook_request_patch.py
--rw-r--r--  2.0 unx     3523 b- defN 23-May-17 09:26 cloudsmith_api/models/resources_rate_check.py
--rw-r--r--  2.0 unx     2790 b- defN 23-May-17 09:26 cloudsmith_api/models/respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     2825 b- defN 23-May-17 09:26 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx    57940 b- defN 23-May-17 09:26 cloudsmith_api/models/rpm_package_upload.py
--rw-r--r--  2.0 unx     7374 b- defN 23-May-17 09:26 cloudsmith_api/models/rpm_package_upload_request.py
--rw-r--r--  2.0 unx    58217 b- defN 23-May-17 09:26 cloudsmith_api/models/ruby_package_upload.py
--rw-r--r--  2.0 unx     6160 b- defN 23-May-17 09:26 cloudsmith_api/models/ruby_package_upload_request.py
--rw-r--r--  2.0 unx     8234 b- defN 23-May-17 09:26 cloudsmith_api/models/service.py
--rw-r--r--  2.0 unx     6726 b- defN 23-May-17 09:26 cloudsmith_api/models/service_request.py
--rw-r--r--  2.0 unx     6701 b- defN 23-May-17 09:26 cloudsmith_api/models/service_request_patch.py
--rw-r--r--  2.0 unx     4951 b- defN 23-May-17 09:26 cloudsmith_api/models/service_teams.py
--rw-r--r--  2.0 unx     4584 b- defN 23-May-17 09:26 cloudsmith_api/models/status_basic.py
--rw-r--r--  2.0 unx     8478 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_allocated_limit.py
--rw-r--r--  2.0 unx     6140 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx     4670 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_region.py
--rw-r--r--  2.0 unx     6847 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_usage.py
--rw-r--r--  2.0 unx     5048 b- defN 23-May-17 09:26 cloudsmith_api/models/storage_usage_raw.py
--rw-r--r--  2.0 unx     2665 b- defN 23-May-17 09:26 cloudsmith_api/models/tags.py
--rw-r--r--  2.0 unx    59602 b- defN 23-May-17 09:26 cloudsmith_api/models/terraform_package_upload.py
--rw-r--r--  2.0 unx     6245 b- defN 23-May-17 09:26 cloudsmith_api/models/terraform_package_upload_request.py
--rw-r--r--  2.0 unx     5738 b- defN 23-May-17 09:26 cloudsmith_api/models/usage.py
--rw-r--r--  2.0 unx     4147 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_fieldset.py
--rw-r--r--  2.0 unx     4277 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_limits.py
--rw-r--r--  2.0 unx     4334 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_limits_raw.py
--rw-r--r--  2.0 unx     4382 b- defN 23-May-17 09:26 cloudsmith_api/models/usage_raw.py
--rw-r--r--  2.0 unx     3590 b- defN 23-May-17 09:26 cloudsmith_api/models/user_auth_token.py
--rw-r--r--  2.0 unx     4612 b- defN 23-May-17 09:26 cloudsmith_api/models/user_auth_token_request.py
--rw-r--r--  2.0 unx     8019 b- defN 23-May-17 09:26 cloudsmith_api/models/user_brief.py
--rw-r--r--  2.0 unx    11110 b- defN 23-May-17 09:26 cloudsmith_api/models/user_profile.py
--rw-r--r--  2.0 unx    60899 b- defN 23-May-17 09:26 cloudsmith_api/models/vagrant_package_upload.py
--rw-r--r--  2.0 unx     9492 b- defN 23-May-17 09:26 cloudsmith_api/models/vagrant_package_upload_request.py
--rw-r--r--  2.0 unx    13112 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability.py
--rw-r--r--  2.0 unx     5400 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan.py
--rw-r--r--  2.0 unx    10348 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_results.py
--rw-r--r--  2.0 unx     9725 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx     8443 b- defN 23-May-17 09:26 cloudsmith_api/models/vulnerability_scan_version.py
--rw-r--r--  2.0 unx     4751 b- defN 23-May-17 09:26 cloudsmith_api/models/webhook_template.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-17 09:26 test/__init__.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-17 09:26 test/test_allocated_limit.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_allocated_limit_raw.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_alpine_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_alpine_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_architecture.py
--rw-r--r--  2.0 unx     1083 b- defN 23-May-17 09:26 test/test_audit_log_api.py
--rw-r--r--  2.0 unx      883 b- defN 23-May-17 09:26 test/test_badges_api.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_cargo_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_cargo_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_cocoapods_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_cocoapods_package_upload_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_common_bandwidth_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_common_bandwidth_metrics_value.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_common_downloads_metrics.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_common_downloads_metrics_value.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_common_metrics.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_composer_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_composer_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_conan_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_conan_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_conda_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_conda_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_cran_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_cran_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_dart_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_dart_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_deb_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_deb_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_distribution.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_distribution_full.py
--rw-r--r--  2.0 unx      940 b- defN 23-May-17 09:26 test/test_distribution_version.py
--rw-r--r--  2.0 unx     1019 b- defN 23-May-17 09:26 test/test_distros_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_docker_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_docker_package_upload_request.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_entitlement_usage_metrics.py
--rw-r--r--  2.0 unx     2550 b- defN 23-May-17 09:26 test/test_entitlements_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_error_detail.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-17 09:26 test/test_eula.py
--rw-r--r--  2.0 unx     1503 b- defN 23-May-17 09:26 test/test_files_api.py
--rw-r--r--  2.0 unx      834 b- defN 23-May-17 09:26 test/test_format.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_format_support.py
--rw-r--r--  2.0 unx     1022 b- defN 23-May-17 09:26 test/test_formats_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-May-17 09:26 test/test_geo_ip_location.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_go_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_go_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_helm_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_helm_package_upload_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_hex_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_hex_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_history.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_history_fieldset.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_history_fieldset_raw.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_luarocks_package_upload.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_luarocks_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_maven_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_maven_package_upload_request.py
--rw-r--r--  2.0 unx     1335 b- defN 23-May-17 09:26 test/test_metrics_api.py
--rw-r--r--  2.0 unx      858 b- defN 23-May-17 09:26 test/test_namespace.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_namespace_audit_log.py
--rw-r--r--  2.0 unx     1051 b- defN 23-May-17 09:26 test/test_namespaces_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_nested_license_policy.py
--rw-r--r--  2.0 unx      990 b- defN 23-May-17 09:26 test/test_nested_vulnerability_policy.py
--rw-r--r--  2.0 unx     1032 b- defN 23-May-17 09:26 test/test_nested_vulnerability_scan_results.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_npm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_npm_package_upload_request.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_nuget_package_upload.py
--rw-r--r--  2.0 unx      992 b- defN 23-May-17 09:26 test/test_nuget_package_upload_request.py
--rw-r--r--  2.0 unx      882 b- defN 23-May-17 09:26 test/test_organization.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_organization_group_sync.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_organization_group_sync_request.py
--rw-r--r--  2.0 unx      932 b- defN 23-May-17 09:26 test/test_organization_invite.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_organization_invite_extend.py
--rw-r--r--  2.0 unx      990 b- defN 23-May-17 09:26 test/test_organization_invite_request.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_organization_invite_update.py
--rw-r--r--  2.0 unx     1082 b- defN 23-May-17 09:26 test/test_organization_invite_update_request_patch.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-17 09:26 test/test_organization_membership.py
--rw-r--r--  2.0 unx     1048 b- defN 23-May-17 09:26 test/test_organization_package_license_policy.py
--rw-r--r--  2.0 unx     1106 b- defN 23-May-17 09:26 test/test_organization_package_license_policy_request.py
--rw-r--r--  2.0 unx     1148 b- defN 23-May-17 09:26 test/test_organization_package_license_policy_request_patch.py
--rw-r--r--  2.0 unx     1096 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy.py
--rw-r--r--  2.0 unx     1154 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy_request.py
--rw-r--r--  2.0 unx     1196 b- defN 23-May-17 09:26 test/test_organization_package_vulnerability_policy_request_patch.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_organization_team.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_organization_team_members.py
--rw-r--r--  2.0 unx      998 b- defN 23-May-17 09:26 test/test_organization_team_membership.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_organization_team_request.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_organization_team_request_patch.py
--rw-r--r--  2.0 unx     8724 b- defN 23-May-17 09:26 test/test_orgs_api.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_p2_package_upload.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_p2_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_package.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_copy.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_package_copy_request.py
--rw-r--r--  2.0 unx      940 b- defN 23-May-17 09:26 test/test_package_dependencies.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_package_dependency.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_file.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_package_file_parts_upload.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_package_file_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_package_file_upload_request.py
--rw-r--r--  2.0 unx     1050 b- defN 23-May-17 09:26 test/test_package_license_policy_violation_log.py
--rw-r--r--  2.0 unx     1134 b- defN 23-May-17 09:26 test/test_package_license_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_package_move.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_package_move_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_package_quarantine.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_package_quarantine_request.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_package_resync.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_package_status.py
--rw-r--r--  2.0 unx      868 b- defN 23-May-17 09:26 test/test_package_tag.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_package_tag_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_package_usage_metrics.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_package_version_badge.py
--rw-r--r--  2.0 unx      948 b- defN 23-May-17 09:26 test/test_package_vulnerability.py
--rw-r--r--  2.0 unx     1098 b- defN 23-May-17 09:26 test/test_package_vulnerability_policy_violation_log.py
--rw-r--r--  2.0 unx     1182 b- defN 23-May-17 09:26 test/test_package_vulnerability_policy_violation_log_cursor_page.py
--rw-r--r--  2.0 unx    11377 b- defN 23-May-17 09:26 test/test_packages_api.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_python_package_upload.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_python_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-May-17 09:26 test/test_quota.py
--rw-r--r--  2.0 unx     1364 b- defN 23-May-17 09:26 test/test_quota_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_quota_history.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-17 09:26 test/test_rate_check.py
--rw-r--r--  2.0 unx      862 b- defN 23-May-17 09:26 test/test_rates_api.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_raw_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_raw_package_upload_request.py
--rw-r--r--  2.0 unx     4407 b- defN 23-May-17 09:26 test/test_repos_api.py
--rw-r--r--  2.0 unx      866 b- defN 23-May-17 09:26 test/test_repository.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_repository_audit_log.py
--rw-r--r--  2.0 unx      916 b- defN 23-May-17 09:26 test/test_repository_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_repository_create_request.py
--rw-r--r--  2.0 unx      944 b- defN 23-May-17 09:26 test/test_repository_geo_ip_cidr.py
--rw-r--r--  2.0 unx     1002 b- defN 23-May-17 09:26 test/test_repository_geo_ip_country_code.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules_request.py
--rw-r--r--  2.0 unx     1052 b- defN 23-May-17 09:26 test/test_repository_geo_ip_rules_request_patch.py
--rw-r--r--  2.0 unx     1002 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address_response.py
--rw-r--r--  2.0 unx     1102 b- defN 23-May-17 09:26 test/test_repository_geo_ip_test_address_response_dict.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_repository_gpg_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_repository_gpg_key_create.py
--rw-r--r--  2.0 unx      974 b- defN 23-May-17 09:26 test/test_repository_privilege_dict.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_repository_privilege_input.py
--rw-r--r--  2.0 unx     1040 b- defN 23-May-17 09:26 test/test_repository_privilege_input_request.py
--rw-r--r--  2.0 unx     1082 b- defN 23-May-17 09:26 test/test_repository_privilege_input_request_patch.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_request_patch.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_repository_rsa_key.py
--rw-r--r--  2.0 unx      968 b- defN 23-May-17 09:26 test/test_repository_rsa_key_create.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_repository_token.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_repository_token_action.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_token_refresh.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_repository_token_refresh_request.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_repository_token_request.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_repository_token_request_patch.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_repository_token_sync.py
--rw-r--r--  2.0 unx     1000 b- defN 23-May-17 09:26 test/test_repository_token_sync_request.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_repository_webhook.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_repository_webhook_request.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_repository_webhook_request_patch.py
--rw-r--r--  2.0 unx      934 b- defN 23-May-17 09:26 test/test_resources_rate_check.py
--rw-r--r--  2.0 unx     1026 b- defN 23-May-17 09:26 test/test_respository_geo_ip_enable_disable.py
--rw-r--r--  2.0 unx     1084 b- defN 23-May-17 09:26 test/test_respository_geo_ip_enable_disable_request.py
--rw-r--r--  2.0 unx      918 b- defN 23-May-17 09:26 test/test_rpm_package_upload.py
--rw-r--r--  2.0 unx      976 b- defN 23-May-17 09:26 test/test_rpm_package_upload_request.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-17 09:26 test/test_ruby_package_upload.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_ruby_package_upload_request.py
--rw-r--r--  2.0 unx      842 b- defN 23-May-17 09:26 test/test_service.py
--rw-r--r--  2.0 unx      900 b- defN 23-May-17 09:26 test/test_service_request.py
--rw-r--r--  2.0 unx      942 b- defN 23-May-17 09:26 test/test_service_request_patch.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_service_teams.py
--rw-r--r--  2.0 unx      864 b- defN 23-May-17 09:26 test/test_status_api.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_status_basic.py
--rw-r--r--  2.0 unx      958 b- defN 23-May-17 09:26 test/test_storage_allocated_limit.py
--rw-r--r--  2.0 unx      984 b- defN 23-May-17 09:26 test/test_storage_allocated_limit_raw.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_storage_region.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-17 09:26 test/test_storage_regions_api.py
--rw-r--r--  2.0 unx      884 b- defN 23-May-17 09:26 test/test_storage_usage.py
--rw-r--r--  2.0 unx      910 b- defN 23-May-17 09:26 test/test_storage_usage_raw.py
--rw-r--r--  2.0 unx      818 b- defN 23-May-17 09:26 test/test_tags.py
--rw-r--r--  2.0 unx      966 b- defN 23-May-17 09:26 test/test_terraform_package_upload.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_terraform_package_upload_request.py
--rw-r--r--  2.0 unx      826 b- defN 23-May-17 09:26 test/test_usage.py
--rw-r--r--  2.0 unx      892 b- defN 23-May-17 09:26 test/test_usage_fieldset.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_usage_limits.py
--rw-r--r--  2.0 unx      902 b- defN 23-May-17 09:26 test/test_usage_limits_raw.py
--rw-r--r--  2.0 unx      852 b- defN 23-May-17 09:26 test/test_usage_raw.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-17 09:26 test/test_user_api.py
--rw-r--r--  2.0 unx      894 b- defN 23-May-17 09:26 test/test_user_auth_token.py
--rw-r--r--  2.0 unx      952 b- defN 23-May-17 09:26 test/test_user_auth_token_request.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-17 09:26 test/test_user_brief.py
--rw-r--r--  2.0 unx      876 b- defN 23-May-17 09:26 test/test_user_profile.py
--rw-r--r--  2.0 unx      865 b- defN 23-May-17 09:26 test/test_users_api.py
--rw-r--r--  2.0 unx      950 b- defN 23-May-17 09:26 test/test_vagrant_package_upload.py
--rw-r--r--  2.0 unx     1008 b- defN 23-May-17 09:26 test/test_vagrant_package_upload_request.py
--rw-r--r--  2.0 unx     1487 b- defN 23-May-17 09:26 test/test_vulnerabilities_api.py
--rw-r--r--  2.0 unx      890 b- defN 23-May-17 09:26 test/test_vulnerability.py
--rw-r--r--  2.0 unx      924 b- defN 23-May-17 09:26 test/test_vulnerability_scan.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_vulnerability_scan_results.py
--rw-r--r--  2.0 unx     1016 b- defN 23-May-17 09:26 test/test_vulnerability_scan_results_list.py
--rw-r--r--  2.0 unx      982 b- defN 23-May-17 09:26 test/test_vulnerability_scan_version.py
--rw-r--r--  2.0 unx      908 b- defN 23-May-17 09:26 test/test_webhook_template.py
--rw-r--r--  2.0 unx     1557 b- defN 23-May-17 09:26 test/test_webhooks_api.py
--rw-r--r--  2.0 unx      457 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    39881 b- defN 23-May-17 09:27 cloudsmith_api-2.0.3.dist-info/RECORD
-411 files, 4309307 bytes uncompressed, 658862 bytes compressed:  84.7%
+Zip file size: 734212 bytes, number of entries: 415
+-rw-r--r--  2.0 unx    16073 b- defN 23-May-24 16:33 cloudsmith_api/__init__.py
+-rw-r--r--  2.0 unx    25067 b- defN 23-May-24 16:33 cloudsmith_api/api_client.py
+-rw-r--r--  2.0 unx     8390 b- defN 23-May-24 16:33 cloudsmith_api/configuration.py
+-rw-r--r--  2.0 unx    13166 b- defN 23-May-24 16:33 cloudsmith_api/rest.py
+-rw-r--r--  2.0 unx     1131 b- defN 23-May-24 16:33 cloudsmith_api/api/__init__.py
+-rw-r--r--  2.0 unx    11039 b- defN 23-May-24 16:33 cloudsmith_api/api/audit_log_api.py
+-rw-r--r--  2.0 unx    11425 b- defN 23-May-24 16:33 cloudsmith_api/api/badges_api.py
+-rw-r--r--  2.0 unx     7978 b- defN 23-May-24 16:33 cloudsmith_api/api/distros_api.py
+-rw-r--r--  2.0 unx    54786 b- defN 23-May-24 16:33 cloudsmith_api/api/entitlements_api.py
+-rw-r--r--  2.0 unx    26620 b- defN 23-May-24 16:33 cloudsmith_api/api/files_api.py
+-rw-r--r--  2.0 unx     7930 b- defN 23-May-24 16:33 cloudsmith_api/api/formats_api.py
+-rw-r--r--  2.0 unx    19214 b- defN 23-May-24 16:33 cloudsmith_api/api/metrics_api.py
+-rw-r--r--  2.0 unx     8514 b- defN 23-May-24 16:33 cloudsmith_api/api/namespaces_api.py
+-rw-r--r--  2.0 unx   195413 b- defN 23-May-24 16:33 cloudsmith_api/api/orgs_api.py
+-rw-r--r--  2.0 unx   294424 b- defN 23-May-24 16:33 cloudsmith_api/api/packages_api.py
+-rw-r--r--  2.0 unx    16386 b- defN 23-May-24 16:33 cloudsmith_api/api/quota_api.py
+-rw-r--r--  2.0 unx     4157 b- defN 23-May-24 16:33 cloudsmith_api/api/rates_api.py
+-rw-r--r--  2.0 unx    98642 b- defN 23-May-24 16:33 cloudsmith_api/api/repos_api.py
+-rw-r--r--  2.0 unx     4118 b- defN 23-May-24 16:33 cloudsmith_api/api/status_api.py
+-rw-r--r--  2.0 unx     8075 b- defN 23-May-24 16:33 cloudsmith_api/api/storage_regions_api.py
+-rw-r--r--  2.0 unx     7631 b- defN 23-May-24 16:33 cloudsmith_api/api/user_api.py
+-rw-r--r--  2.0 unx     4706 b- defN 23-May-24 16:33 cloudsmith_api/api/users_api.py
+-rw-r--r--  2.0 unx    22091 b- defN 23-May-24 16:33 cloudsmith_api/api/vulnerabilities_api.py
+-rw-r--r--  2.0 unx    26050 b- defN 23-May-24 16:33 cloudsmith_api/api/webhooks_api.py
+-rw-r--r--  2.0 unx    14876 b- defN 23-May-24 16:33 cloudsmith_api/models/__init__.py
+-rw-r--r--  2.0 unx     7305 b- defN 23-May-24 16:33 cloudsmith_api/models/allocated_limit.py
+-rw-r--r--  2.0 unx     5410 b- defN 23-May-24 16:33 cloudsmith_api/models/allocated_limit_raw.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-24 16:33 cloudsmith_api/models/alpine_package_upload.py
+-rw-r--r--  2.0 unx     7437 b- defN 23-May-24 16:33 cloudsmith_api/models/alpine_package_upload_request.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-May-24 16:33 cloudsmith_api/models/architecture.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-24 16:33 cloudsmith_api/models/cargo_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-24 16:33 cloudsmith_api/models/cargo_package_upload_request.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-24 16:33 cloudsmith_api/models/cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-24 16:33 cloudsmith_api/models/cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-24 16:33 cloudsmith_api/models/common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     5636 b- defN 23-May-24 16:33 cloudsmith_api/models/common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx     6052 b- defN 23-May-24 16:33 cloudsmith_api/models/common_downloads_metrics.py
+-rw-r--r--  2.0 unx     3526 b- defN 23-May-24 16:33 cloudsmith_api/models/common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx     6129 b- defN 23-May-24 16:33 cloudsmith_api/models/common_metrics.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-24 16:33 cloudsmith_api/models/composer_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-24 16:33 cloudsmith_api/models/composer_package_upload_request.py
+-rw-r--r--  2.0 unx    61539 b- defN 23-May-24 16:33 cloudsmith_api/models/conan_package_upload.py
+-rw-r--r--  2.0 unx    14491 b- defN 23-May-24 16:33 cloudsmith_api/models/conan_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-24 16:33 cloudsmith_api/models/conda_package_upload.py
+-rw-r--r--  2.0 unx     6177 b- defN 23-May-24 16:33 cloudsmith_api/models/conda_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-24 16:33 cloudsmith_api/models/cran_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-24 16:33 cloudsmith_api/models/cran_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-24 16:33 cloudsmith_api/models/dart_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-24 16:33 cloudsmith_api/models/dart_package_upload_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-24 16:33 cloudsmith_api/models/deb_package_upload.py
+-rw-r--r--  2.0 unx     9690 b- defN 23-May-24 16:33 cloudsmith_api/models/deb_package_upload_request.py
+-rw-r--r--  2.0 unx     6159 b- defN 23-May-24 16:33 cloudsmith_api/models/distribution.py
+-rw-r--r--  2.0 unx     8542 b- defN 23-May-24 16:33 cloudsmith_api/models/distribution_full.py
+-rw-r--r--  2.0 unx     4497 b- defN 23-May-24 16:33 cloudsmith_api/models/distribution_version.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-24 16:33 cloudsmith_api/models/docker_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-24 16:33 cloudsmith_api/models/docker_package_upload_request.py
+-rw-r--r--  2.0 unx     3541 b- defN 23-May-24 16:33 cloudsmith_api/models/entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     3729 b- defN 23-May-24 16:33 cloudsmith_api/models/error_detail.py
+-rw-r--r--  2.0 unx     5458 b- defN 23-May-24 16:33 cloudsmith_api/models/eula.py
+-rw-r--r--  2.0 unx    11287 b- defN 23-May-24 16:33 cloudsmith_api/models/format.py
+-rw-r--r--  2.0 unx     7319 b- defN 23-May-24 16:33 cloudsmith_api/models/format_support.py
+-rw-r--r--  2.0 unx     8615 b- defN 23-May-24 16:33 cloudsmith_api/models/geo_ip_location.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-24 16:33 cloudsmith_api/models/go_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-24 16:33 cloudsmith_api/models/go_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-24 16:33 cloudsmith_api/models/helm_package_upload.py
+-rw-r--r--  2.0 unx     7480 b- defN 23-May-24 16:33 cloudsmith_api/models/helm_package_upload_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-24 16:33 cloudsmith_api/models/hex_package_upload.py
+-rw-r--r--  2.0 unx     6143 b- defN 23-May-24 16:33 cloudsmith_api/models/hex_package_upload_request.py
+-rw-r--r--  2.0 unx     7028 b- defN 23-May-24 16:33 cloudsmith_api/models/history.py
+-rw-r--r--  2.0 unx     5168 b- defN 23-May-24 16:33 cloudsmith_api/models/history_fieldset.py
+-rw-r--r--  2.0 unx     5246 b- defN 23-May-24 16:33 cloudsmith_api/models/history_fieldset_raw.py
+-rw-r--r--  2.0 unx    59325 b- defN 23-May-24 16:33 cloudsmith_api/models/luarocks_package_upload.py
+-rw-r--r--  2.0 unx     6228 b- defN 23-May-24 16:33 cloudsmith_api/models/luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx    61667 b- defN 23-May-24 16:33 cloudsmith_api/models/maven_package_upload.py
+-rw-r--r--  2.0 unx    14513 b- defN 23-May-24 16:33 cloudsmith_api/models/maven_package_upload_request.py
+-rw-r--r--  2.0 unx     5806 b- defN 23-May-24 16:33 cloudsmith_api/models/namespace.py
+-rw-r--r--  2.0 unx    18223 b- defN 23-May-24 16:33 cloudsmith_api/models/namespace_audit_log.py
+-rw-r--r--  2.0 unx    11620 b- defN 23-May-24 16:33 cloudsmith_api/models/nested_license_policy.py
+-rw-r--r--  2.0 unx    12280 b- defN 23-May-24 16:33 cloudsmith_api/models/nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     9527 b- defN 23-May-24 16:33 cloudsmith_api/models/nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-24 16:33 cloudsmith_api/models/npm_package_upload.py
+-rw-r--r--  2.0 unx     7663 b- defN 23-May-24 16:33 cloudsmith_api/models/npm_package_upload_request.py
+-rw-r--r--  2.0 unx    58494 b- defN 23-May-24 16:33 cloudsmith_api/models/nuget_package_upload.py
+-rw-r--r--  2.0 unx     7272 b- defN 23-May-24 16:33 cloudsmith_api/models/nuget_package_upload_request.py
+-rw-r--r--  2.0 unx     7918 b- defN 23-May-24 16:33 cloudsmith_api/models/organization.py
+-rw-r--r--  2.0 unx     8391 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_group_sync.py
+-rw-r--r--  2.0 unx     8223 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_group_sync_request.py
+-rw-r--r--  2.0 unx    10169 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_invite.py
+-rw-r--r--  2.0 unx    10519 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_invite_extend.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_invite_request.py
+-rw-r--r--  2.0 unx     3821 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_invite_update.py
+-rw-r--r--  2.0 unx     3929 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx    12300 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_membership.py
+-rw-r--r--  2.0 unx    12219 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_license_policy.py
+-rw-r--r--  2.0 unx     9666 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     9539 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx    12855 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx    10230 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx    10245 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx     8110 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_team.py
+-rw-r--r--  2.0 unx     3669 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_team_members.py
+-rw-r--r--  2.0 unx     4783 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_team_membership.py
+-rw-r--r--  2.0 unx     7065 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_team_request.py
+-rw-r--r--  2.0 unx     7040 b- defN 23-May-24 16:33 cloudsmith_api/models/organization_team_request_patch.py
+-rw-r--r--  2.0 unx    57663 b- defN 23-May-24 16:33 cloudsmith_api/models/p2_package_upload.py
+-rw-r--r--  2.0 unx     6126 b- defN 23-May-24 16:33 cloudsmith_api/models/p2_package_upload_request.py
+-rw-r--r--  2.0 unx    55965 b- defN 23-May-24 16:33 cloudsmith_api/models/package.py
+-rw-r--r--  2.0 unx    57197 b- defN 23-May-24 16:33 cloudsmith_api/models/package_copy.py
+-rw-r--r--  2.0 unx     4776 b- defN 23-May-24 16:33 cloudsmith_api/models/package_copy_request.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-24 16:33 cloudsmith_api/models/package_dependencies.py
+-rw-r--r--  2.0 unx     7227 b- defN 23-May-24 16:33 cloudsmith_api/models/package_dependency.py
+-rw-r--r--  2.0 unx    12968 b- defN 23-May-24 16:33 cloudsmith_api/models/package_file.py
+-rw-r--r--  2.0 unx     6108 b- defN 23-May-24 16:33 cloudsmith_api/models/package_file_parts_upload.py
+-rw-r--r--  2.0 unx     7841 b- defN 23-May-24 16:33 cloudsmith_api/models/package_file_upload.py
+-rw-r--r--  2.0 unx     7815 b- defN 23-May-24 16:33 cloudsmith_api/models/package_file_upload_request.py
+-rw-r--r--  2.0 unx     6035 b- defN 23-May-24 16:33 cloudsmith_api/models/package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     5198 b- defN 23-May-24 16:33 cloudsmith_api/models/package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    57195 b- defN 23-May-24 16:33 cloudsmith_api/models/package_move.py
+-rw-r--r--  2.0 unx     3820 b- defN 23-May-24 16:33 cloudsmith_api/models/package_move_request.py
+-rw-r--r--  2.0 unx    58775 b- defN 23-May-24 16:33 cloudsmith_api/models/package_quarantine.py
+-rw-r--r--  2.0 unx     3527 b- defN 23-May-24 16:33 cloudsmith_api/models/package_quarantine_request.py
+-rw-r--r--  2.0 unx    57651 b- defN 23-May-24 16:33 cloudsmith_api/models/package_resync.py
+-rw-r--r--  2.0 unx    15877 b- defN 23-May-24 16:33 cloudsmith_api/models/package_status.py
+-rw-r--r--  2.0 unx    57199 b- defN 23-May-24 16:33 cloudsmith_api/models/package_tag.py
+-rw-r--r--  2.0 unx     5352 b- defN 23-May-24 16:33 cloudsmith_api/models/package_tag_request.py
+-rw-r--r--  2.0 unx     3547 b- defN 23-May-24 16:33 cloudsmith_api/models/package_usage_metrics.py
+-rw-r--r--  2.0 unx     2740 b- defN 23-May-24 16:33 cloudsmith_api/models/package_version_badge.py
+-rw-r--r--  2.0 unx     5707 b- defN 23-May-24 16:33 cloudsmith_api/models/package_vulnerability.py
+-rw-r--r--  2.0 unx     7491 b- defN 23-May-24 16:33 cloudsmith_api/models/package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     5318 b- defN 23-May-24 16:33 cloudsmith_api/models/package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    58771 b- defN 23-May-24 16:33 cloudsmith_api/models/python_package_upload.py
+-rw-r--r--  2.0 unx     6194 b- defN 23-May-24 16:33 cloudsmith_api/models/python_package_upload_request.py
+-rw-r--r--  2.0 unx     3358 b- defN 23-May-24 16:33 cloudsmith_api/models/quota.py
+-rw-r--r--  2.0 unx     3463 b- defN 23-May-24 16:33 cloudsmith_api/models/quota_history.py
+-rw-r--r--  2.0 unx     7675 b- defN 23-May-24 16:33 cloudsmith_api/models/rate_check.py
+-rw-r--r--  2.0 unx    58899 b- defN 23-May-24 16:33 cloudsmith_api/models/raw_package_upload.py
+-rw-r--r--  2.0 unx    11674 b- defN 23-May-24 16:33 cloudsmith_api/models/raw_package_upload_request.py
+-rw-r--r--  2.0 unx    66229 b- defN 23-May-24 16:33 cloudsmith_api/models/repository.py
+-rw-r--r--  2.0 unx    14861 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_audit_log.py
+-rw-r--r--  2.0 unx    67555 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_create.py
+-rw-r--r--  2.0 unx    52996 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_create_request.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     4488 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx     4424 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     4515 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     4312 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     3733 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     3906 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     7359 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx     8734 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_gpg_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_gpg_key_create.py
+-rw-r--r--  2.0 unx     7702 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_privilege_dict.py
+-rw-r--r--  2.0 unx     3818 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_privilege_input.py
+-rw-r--r--  2.0 unx     3881 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     3790 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx    51807 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_request_patch.py
+-rw-r--r--  2.0 unx     7753 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_rsa_key.py
+-rw-r--r--  2.0 unx     5133 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_rsa_key_create.py
+-rw-r--r--  2.0 unx    40544 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token.py
+-rw-r--r--  2.0 unx     2750 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_action.py
+-rw-r--r--  2.0 unx    41541 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_refresh.py
+-rw-r--r--  2.0 unx    21868 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_refresh_request.py
+-rw-r--r--  2.0 unx    22374 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_request.py
+-rw-r--r--  2.0 unx    22569 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_request_patch.py
+-rw-r--r--  2.0 unx     3505 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_sync.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_token_sync_request.py
+-rw-r--r--  2.0 unx    30728 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_webhook.py
+-rw-r--r--  2.0 unx    18912 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_webhook_request.py
+-rw-r--r--  2.0 unx    18774 b- defN 23-May-24 16:33 cloudsmith_api/models/repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx     3523 b- defN 23-May-24 16:33 cloudsmith_api/models/resources_rate_check.py
+-rw-r--r--  2.0 unx     2790 b- defN 23-May-24 16:33 cloudsmith_api/models/respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     2825 b- defN 23-May-24 16:33 cloudsmith_api/models/respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx    57940 b- defN 23-May-24 16:33 cloudsmith_api/models/rpm_package_upload.py
+-rw-r--r--  2.0 unx     7374 b- defN 23-May-24 16:33 cloudsmith_api/models/rpm_package_upload_request.py
+-rw-r--r--  2.0 unx    58217 b- defN 23-May-24 16:33 cloudsmith_api/models/ruby_package_upload.py
+-rw-r--r--  2.0 unx     6160 b- defN 23-May-24 16:33 cloudsmith_api/models/ruby_package_upload_request.py
+-rw-r--r--  2.0 unx     8234 b- defN 23-May-24 16:33 cloudsmith_api/models/service.py
+-rw-r--r--  2.0 unx     6726 b- defN 23-May-24 16:33 cloudsmith_api/models/service_request.py
+-rw-r--r--  2.0 unx     6701 b- defN 23-May-24 16:33 cloudsmith_api/models/service_request_patch.py
+-rw-r--r--  2.0 unx     4951 b- defN 23-May-24 16:33 cloudsmith_api/models/service_teams.py
+-rw-r--r--  2.0 unx     4584 b- defN 23-May-24 16:33 cloudsmith_api/models/status_basic.py
+-rw-r--r--  2.0 unx     8478 b- defN 23-May-24 16:33 cloudsmith_api/models/storage_allocated_limit.py
+-rw-r--r--  2.0 unx     6140 b- defN 23-May-24 16:33 cloudsmith_api/models/storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx     4670 b- defN 23-May-24 16:33 cloudsmith_api/models/storage_region.py
+-rw-r--r--  2.0 unx     6847 b- defN 23-May-24 16:33 cloudsmith_api/models/storage_usage.py
+-rw-r--r--  2.0 unx     5048 b- defN 23-May-24 16:33 cloudsmith_api/models/storage_usage_raw.py
+-rw-r--r--  2.0 unx    58865 b- defN 23-May-24 16:33 cloudsmith_api/models/swift_package_upload.py
+-rw-r--r--  2.0 unx     7279 b- defN 23-May-24 16:33 cloudsmith_api/models/swift_package_upload_request.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-May-24 16:33 cloudsmith_api/models/tags.py
+-rw-r--r--  2.0 unx    59602 b- defN 23-May-24 16:33 cloudsmith_api/models/terraform_package_upload.py
+-rw-r--r--  2.0 unx     6245 b- defN 23-May-24 16:33 cloudsmith_api/models/terraform_package_upload_request.py
+-rw-r--r--  2.0 unx     5738 b- defN 23-May-24 16:33 cloudsmith_api/models/usage.py
+-rw-r--r--  2.0 unx     4147 b- defN 23-May-24 16:33 cloudsmith_api/models/usage_fieldset.py
+-rw-r--r--  2.0 unx     4277 b- defN 23-May-24 16:33 cloudsmith_api/models/usage_limits.py
+-rw-r--r--  2.0 unx     4334 b- defN 23-May-24 16:33 cloudsmith_api/models/usage_limits_raw.py
+-rw-r--r--  2.0 unx     4382 b- defN 23-May-24 16:33 cloudsmith_api/models/usage_raw.py
+-rw-r--r--  2.0 unx     3590 b- defN 23-May-24 16:33 cloudsmith_api/models/user_auth_token.py
+-rw-r--r--  2.0 unx     4612 b- defN 23-May-24 16:33 cloudsmith_api/models/user_auth_token_request.py
+-rw-r--r--  2.0 unx     8019 b- defN 23-May-24 16:33 cloudsmith_api/models/user_brief.py
+-rw-r--r--  2.0 unx    11110 b- defN 23-May-24 16:33 cloudsmith_api/models/user_profile.py
+-rw-r--r--  2.0 unx    60899 b- defN 23-May-24 16:33 cloudsmith_api/models/vagrant_package_upload.py
+-rw-r--r--  2.0 unx     9492 b- defN 23-May-24 16:33 cloudsmith_api/models/vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx    13112 b- defN 23-May-24 16:33 cloudsmith_api/models/vulnerability.py
+-rw-r--r--  2.0 unx     5400 b- defN 23-May-24 16:33 cloudsmith_api/models/vulnerability_scan.py
+-rw-r--r--  2.0 unx    10348 b- defN 23-May-24 16:33 cloudsmith_api/models/vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     9725 b- defN 23-May-24 16:33 cloudsmith_api/models/vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx     8443 b- defN 23-May-24 16:33 cloudsmith_api/models/vulnerability_scan_version.py
+-rw-r--r--  2.0 unx     4751 b- defN 23-May-24 16:33 cloudsmith_api/models/webhook_template.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-24 16:33 test/__init__.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-24 16:33 test/test_allocated_limit.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_alpine_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-24 16:33 test/test_alpine_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-24 16:33 test/test_architecture.py
+-rw-r--r--  2.0 unx     1083 b- defN 23-May-24 16:33 test/test_audit_log_api.py
+-rw-r--r--  2.0 unx      883 b- defN 23-May-24 16:33 test/test_badges_api.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_cargo_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_cargo_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_cocoapods_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-24 16:33 test/test_cocoapods_package_upload_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_common_bandwidth_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-24 16:33 test/test_common_bandwidth_metrics_value.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_common_downloads_metrics.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-24 16:33 test/test_common_downloads_metrics_value.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_common_metrics.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-24 16:33 test/test_composer_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-24 16:33 test/test_composer_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_conan_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_conan_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_conda_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_conda_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_cran_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_cran_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_dart_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_dart_package_upload_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_deb_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-24 16:33 test/test_deb_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-24 16:33 test/test_distribution.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-24 16:33 test/test_distribution_full.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-24 16:33 test/test_distribution_version.py
+-rw-r--r--  2.0 unx     1019 b- defN 23-May-24 16:33 test/test_distros_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_docker_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-24 16:33 test/test_docker_package_upload_request.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-24 16:33 test/test_entitlement_usage_metrics.py
+-rw-r--r--  2.0 unx     2550 b- defN 23-May-24 16:33 test/test_entitlements_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_error_detail.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-24 16:33 test/test_eula.py
+-rw-r--r--  2.0 unx     1503 b- defN 23-May-24 16:33 test/test_files_api.py
+-rw-r--r--  2.0 unx      834 b- defN 23-May-24 16:33 test/test_format.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_format_support.py
+-rw-r--r--  2.0 unx     1022 b- defN 23-May-24 16:33 test/test_formats_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-24 16:33 test/test_geo_ip_location.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-24 16:33 test/test_go_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-24 16:33 test/test_go_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_helm_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_helm_package_upload_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_hex_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-24 16:33 test/test_hex_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-24 16:33 test/test_history.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-24 16:33 test/test_history_fieldset.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_history_fieldset_raw.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-24 16:33 test/test_luarocks_package_upload.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-24 16:33 test/test_luarocks_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_maven_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_maven_package_upload_request.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-24 16:33 test/test_metrics_api.py
+-rw-r--r--  2.0 unx      858 b- defN 23-May-24 16:33 test/test_namespace.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_namespace_audit_log.py
+-rw-r--r--  2.0 unx     1051 b- defN 23-May-24 16:33 test/test_namespaces_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_nested_license_policy.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-24 16:33 test/test_nested_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1032 b- defN 23-May-24 16:33 test/test_nested_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_npm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-24 16:33 test/test_npm_package_upload_request.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_nuget_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_nuget_package_upload_request.py
+-rw-r--r--  2.0 unx      882 b- defN 23-May-24 16:33 test/test_organization.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-24 16:33 test/test_organization_group_sync.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-24 16:33 test/test_organization_group_sync_request.py
+-rw-r--r--  2.0 unx      932 b- defN 23-May-24 16:33 test/test_organization_invite.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_organization_invite_extend.py
+-rw-r--r--  2.0 unx      990 b- defN 23-May-24 16:33 test/test_organization_invite_request.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_organization_invite_update.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-24 16:33 test/test_organization_invite_update_request_patch.py
+-rw-r--r--  2.0 unx      964 b- defN 23-May-24 16:33 test/test_organization_membership.py
+-rw-r--r--  2.0 unx     1048 b- defN 23-May-24 16:33 test/test_organization_package_license_policy.py
+-rw-r--r--  2.0 unx     1106 b- defN 23-May-24 16:33 test/test_organization_package_license_policy_request.py
+-rw-r--r--  2.0 unx     1148 b- defN 23-May-24 16:33 test/test_organization_package_license_policy_request_patch.py
+-rw-r--r--  2.0 unx     1096 b- defN 23-May-24 16:33 test/test_organization_package_vulnerability_policy.py
+-rw-r--r--  2.0 unx     1154 b- defN 23-May-24 16:33 test/test_organization_package_vulnerability_policy_request.py
+-rw-r--r--  2.0 unx     1196 b- defN 23-May-24 16:33 test/test_organization_package_vulnerability_policy_request_patch.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-24 16:33 test/test_organization_team.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-24 16:33 test/test_organization_team_members.py
+-rw-r--r--  2.0 unx      998 b- defN 23-May-24 16:33 test/test_organization_team_membership.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-24 16:33 test/test_organization_team_request.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-24 16:33 test/test_organization_team_request_patch.py
+-rw-r--r--  2.0 unx     8724 b- defN 23-May-24 16:33 test/test_orgs_api.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-24 16:33 test/test_p2_package_upload.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-24 16:33 test/test_p2_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-24 16:33 test/test_package.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_package_copy.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_package_copy_request.py
+-rw-r--r--  2.0 unx      940 b- defN 23-May-24 16:33 test/test_package_dependencies.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-24 16:33 test/test_package_dependency.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_package_file.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-24 16:33 test/test_package_file_parts_upload.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_package_file_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_package_file_upload_request.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-24 16:33 test/test_package_license_policy_violation_log.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-24 16:33 test/test_package_license_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_package_move.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_package_move_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-24 16:33 test/test_package_quarantine.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_package_quarantine_request.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_package_resync.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_package_status.py
+-rw-r--r--  2.0 unx      868 b- defN 23-May-24 16:33 test/test_package_tag.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_package_tag_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_package_usage_metrics.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_package_version_badge.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-24 16:33 test/test_package_vulnerability.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-24 16:33 test/test_package_vulnerability_policy_violation_log.py
+-rw-r--r--  2.0 unx     1182 b- defN 23-May-24 16:33 test/test_package_vulnerability_policy_violation_log_cursor_page.py
+-rw-r--r--  2.0 unx    11743 b- defN 23-May-24 16:33 test/test_packages_api.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_python_package_upload.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-24 16:33 test/test_python_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-24 16:33 test/test_quota.py
+-rw-r--r--  2.0 unx     1364 b- defN 23-May-24 16:33 test/test_quota_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-24 16:33 test/test_quota_history.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-24 16:33 test/test_rate_check.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-24 16:33 test/test_rates_api.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_raw_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-24 16:33 test/test_raw_package_upload_request.py
+-rw-r--r--  2.0 unx     4407 b- defN 23-May-24 16:33 test/test_repos_api.py
+-rw-r--r--  2.0 unx      866 b- defN 23-May-24 16:33 test/test_repository.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_repository_audit_log.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-24 16:33 test/test_repository_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-24 16:33 test/test_repository_create_request.py
+-rw-r--r--  2.0 unx      944 b- defN 23-May-24 16:33 test/test_repository_geo_ip_cidr.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-24 16:33 test/test_repository_geo_ip_country_code.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-24 16:33 test/test_repository_geo_ip_rules.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-24 16:33 test/test_repository_geo_ip_rules_request.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-May-24 16:33 test/test_repository_geo_ip_rules_request_patch.py
+-rw-r--r--  2.0 unx     1002 b- defN 23-May-24 16:33 test/test_repository_geo_ip_test_address.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-24 16:33 test/test_repository_geo_ip_test_address_response.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-May-24 16:33 test/test_repository_geo_ip_test_address_response_dict.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_repository_gpg_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-24 16:33 test/test_repository_gpg_key_create.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-24 16:33 test/test_repository_privilege_dict.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_repository_privilege_input.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-May-24 16:33 test/test_repository_privilege_input_request.py
+-rw-r--r--  2.0 unx     1082 b- defN 23-May-24 16:33 test/test_repository_privilege_input_request_patch.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_repository_request_patch.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_repository_rsa_key.py
+-rw-r--r--  2.0 unx      968 b- defN 23-May-24 16:33 test/test_repository_rsa_key_create.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-24 16:33 test/test_repository_token.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-24 16:33 test/test_repository_token_action.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_repository_token_refresh.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-24 16:33 test/test_repository_token_refresh_request.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_repository_token_request.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-24 16:33 test/test_repository_token_request_patch.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_repository_token_sync.py
+-rw-r--r--  2.0 unx     1000 b- defN 23-May-24 16:33 test/test_repository_token_sync_request.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-24 16:33 test/test_repository_webhook.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_repository_webhook_request.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-24 16:33 test/test_repository_webhook_request_patch.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_resources_rate_check.py
+-rw-r--r--  2.0 unx     1026 b- defN 23-May-24 16:33 test/test_respository_geo_ip_enable_disable.py
+-rw-r--r--  2.0 unx     1084 b- defN 23-May-24 16:33 test/test_respository_geo_ip_enable_disable_request.py
+-rw-r--r--  2.0 unx      918 b- defN 23-May-24 16:33 test/test_rpm_package_upload.py
+-rw-r--r--  2.0 unx      976 b- defN 23-May-24 16:33 test/test_rpm_package_upload_request.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-24 16:33 test/test_ruby_package_upload.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_ruby_package_upload_request.py
+-rw-r--r--  2.0 unx      842 b- defN 23-May-24 16:33 test/test_service.py
+-rw-r--r--  2.0 unx      900 b- defN 23-May-24 16:33 test/test_service_request.py
+-rw-r--r--  2.0 unx      942 b- defN 23-May-24 16:33 test/test_service_request_patch.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-24 16:33 test/test_service_teams.py
+-rw-r--r--  2.0 unx      864 b- defN 23-May-24 16:33 test/test_status_api.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_status_basic.py
+-rw-r--r--  2.0 unx      958 b- defN 23-May-24 16:33 test/test_storage_allocated_limit.py
+-rw-r--r--  2.0 unx      984 b- defN 23-May-24 16:33 test/test_storage_allocated_limit_raw.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_storage_region.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-24 16:33 test/test_storage_regions_api.py
+-rw-r--r--  2.0 unx      884 b- defN 23-May-24 16:33 test/test_storage_usage.py
+-rw-r--r--  2.0 unx      910 b- defN 23-May-24 16:33 test/test_storage_usage_raw.py
+-rw-r--r--  2.0 unx      934 b- defN 23-May-24 16:33 test/test_swift_package_upload.py
+-rw-r--r--  2.0 unx      992 b- defN 23-May-24 16:33 test/test_swift_package_upload_request.py
+-rw-r--r--  2.0 unx      818 b- defN 23-May-24 16:33 test/test_tags.py
+-rw-r--r--  2.0 unx      966 b- defN 23-May-24 16:33 test/test_terraform_package_upload.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-24 16:33 test/test_terraform_package_upload_request.py
+-rw-r--r--  2.0 unx      826 b- defN 23-May-24 16:33 test/test_usage.py
+-rw-r--r--  2.0 unx      892 b- defN 23-May-24 16:33 test/test_usage_fieldset.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_usage_limits.py
+-rw-r--r--  2.0 unx      902 b- defN 23-May-24 16:33 test/test_usage_limits_raw.py
+-rw-r--r--  2.0 unx      852 b- defN 23-May-24 16:33 test/test_usage_raw.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-24 16:33 test/test_user_api.py
+-rw-r--r--  2.0 unx      894 b- defN 23-May-24 16:33 test/test_user_auth_token.py
+-rw-r--r--  2.0 unx      952 b- defN 23-May-24 16:33 test/test_user_auth_token_request.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-24 16:33 test/test_user_brief.py
+-rw-r--r--  2.0 unx      876 b- defN 23-May-24 16:33 test/test_user_profile.py
+-rw-r--r--  2.0 unx      865 b- defN 23-May-24 16:33 test/test_users_api.py
+-rw-r--r--  2.0 unx      950 b- defN 23-May-24 16:33 test/test_vagrant_package_upload.py
+-rw-r--r--  2.0 unx     1008 b- defN 23-May-24 16:33 test/test_vagrant_package_upload_request.py
+-rw-r--r--  2.0 unx     1487 b- defN 23-May-24 16:33 test/test_vulnerabilities_api.py
+-rw-r--r--  2.0 unx      890 b- defN 23-May-24 16:33 test/test_vulnerability.py
+-rw-r--r--  2.0 unx      924 b- defN 23-May-24 16:33 test/test_vulnerability_scan.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_vulnerability_scan_results.py
+-rw-r--r--  2.0 unx     1016 b- defN 23-May-24 16:33 test/test_vulnerability_scan_results_list.py
+-rw-r--r--  2.0 unx      982 b- defN 23-May-24 16:33 test/test_vulnerability_scan_version.py
+-rw-r--r--  2.0 unx      908 b- defN 23-May-24 16:33 test/test_webhook_template.py
+-rw-r--r--  2.0 unx     1557 b- defN 23-May-24 16:33 test/test_webhooks_api.py
+-rw-r--r--  2.0 unx      457 b- defN 23-May-24 16:33 cloudsmith_api-2.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-24 16:33 cloudsmith_api-2.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-May-24 16:33 cloudsmith_api-2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    40280 b- defN 23-May-24 16:33 cloudsmith_api-2.0.4.dist-info/RECORD
+415 files, 4389226 bytes uncompressed, 669144 bytes compressed:  84.8%
```

## zipnote {}

```diff
@@ -552,14 +552,20 @@
 
 Filename: cloudsmith_api/models/storage_usage.py
 Comment: 
 
 Filename: cloudsmith_api/models/storage_usage_raw.py
 Comment: 
 
+Filename: cloudsmith_api/models/swift_package_upload.py
+Comment: 
+
+Filename: cloudsmith_api/models/swift_package_upload_request.py
+Comment: 
+
 Filename: cloudsmith_api/models/tags.py
 Comment: 
 
 Filename: cloudsmith_api/models/terraform_package_upload.py
 Comment: 
 
 Filename: cloudsmith_api/models/terraform_package_upload_request.py
@@ -1143,14 +1149,20 @@
 
 Filename: test/test_storage_usage.py
 Comment: 
 
 Filename: test/test_storage_usage_raw.py
 Comment: 
 
+Filename: test/test_swift_package_upload.py
+Comment: 
+
+Filename: test/test_swift_package_upload_request.py
+Comment: 
+
 Filename: test/test_tags.py
 Comment: 
 
 Filename: test/test_terraform_package_upload.py
 Comment: 
 
 Filename: test/test_terraform_package_upload_request.py
@@ -1215,20 +1227,20 @@
 
 Filename: test/test_webhook_template.py
 Comment: 
 
 Filename: test/test_webhooks_api.py
 Comment: 
 
-Filename: cloudsmith_api-2.0.3.dist-info/METADATA
+Filename: cloudsmith_api-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: cloudsmith_api-2.0.3.dist-info/WHEEL
+Filename: cloudsmith_api-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: cloudsmith_api-2.0.3.dist-info/top_level.txt
+Filename: cloudsmith_api-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudsmith_api-2.0.3.dist-info/RECORD
+Filename: cloudsmith_api-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudsmith_api/__init__.py

```diff
@@ -197,14 +197,16 @@
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
 from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
 from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
 from cloudsmith_api.models.storage_region import StorageRegion
 from cloudsmith_api.models.storage_usage import StorageUsage
 from cloudsmith_api.models.storage_usage_raw import StorageUsageRaw
+from cloudsmith_api.models.swift_package_upload import SwiftPackageUpload
+from cloudsmith_api.models.swift_package_upload_request import SwiftPackageUploadRequest
 from cloudsmith_api.models.tags import Tags
 from cloudsmith_api.models.terraform_package_upload import TerraformPackageUpload
 from cloudsmith_api.models.terraform_package_upload_request import TerraformPackageUploadRequest
 from cloudsmith_api.models.usage import Usage
 from cloudsmith_api.models.usage_fieldset import UsageFieldset
 from cloudsmith_api.models.usage_limits import UsageLimits
 from cloudsmith_api.models.usage_limits_raw import UsageLimitsRaw
```

## cloudsmith_api/api_client.py

```diff
@@ -70,15 +70,15 @@
         self._pool = None
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.0.3/python'
+        self.user_agent = 'Swagger-Codegen/2.0.4/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
```

## cloudsmith_api/configuration.py

```diff
@@ -254,9 +254,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 2.0.3".\
+               "SDK Package Version: 2.0.4".\
                format(env=sys.platform, pyversion=sys.version)
```

## cloudsmith_api/api/packages_api.py

```diff
@@ -3760,14 +3760,125 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def packages_upload_swift(self, owner, repo, **kwargs):  # noqa: E501
+        """Create a new Swift package  # noqa: E501
+
+        Create a new Swift package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_upload_swift(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param SwiftPackageUploadRequest data:
+        :return: SwiftPackageUpload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.packages_upload_swift_with_http_info(owner, repo, **kwargs)  # noqa: E501
+        else:
+            (data) = self.packages_upload_swift_with_http_info(owner, repo, **kwargs)  # noqa: E501
+            return data
+
+    def packages_upload_swift_with_http_info(self, owner, repo, **kwargs):  # noqa: E501
+        """Create a new Swift package  # noqa: E501
+
+        Create a new Swift package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_upload_swift_with_http_info(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param SwiftPackageUploadRequest data:
+        :return: SwiftPackageUpload
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'repo', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method packages_upload_swift" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `packages_upload_swift`")  # noqa: E501
+        # verify the required parameter 'repo' is set
+        if self.api_client.client_side_validation and ('repo' not in params or
+                                                       params['repo'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `repo` when calling `packages_upload_swift`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'repo' in params:
+            path_params['repo'] = params['repo']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/packages/{owner}/{repo}/upload/swift/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='SwiftPackageUpload',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def packages_upload_terraform(self, owner, repo, **kwargs):  # noqa: E501
         """Create a new Terraform package  # noqa: E501
 
         Create a new Terraform package  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.packages_upload_terraform(owner, repo, async_req=True)
@@ -6417,14 +6528,125 @@
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def packages_validate_upload_swift(self, owner, repo, **kwargs):  # noqa: E501
+        """Validate parameters for create Swift package  # noqa: E501
+
+        Validate parameters for create Swift package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_validate_upload_swift(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param SwiftPackageUploadRequest data:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.packages_validate_upload_swift_with_http_info(owner, repo, **kwargs)  # noqa: E501
+        else:
+            (data) = self.packages_validate_upload_swift_with_http_info(owner, repo, **kwargs)  # noqa: E501
+            return data
+
+    def packages_validate_upload_swift_with_http_info(self, owner, repo, **kwargs):  # noqa: E501
+        """Validate parameters for create Swift package  # noqa: E501
+
+        Validate parameters for create Swift package  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.packages_validate_upload_swift_with_http_info(owner, repo, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str owner: (required)
+        :param str repo: (required)
+        :param SwiftPackageUploadRequest data:
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['owner', 'repo', 'data']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method packages_validate_upload_swift" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'owner' is set
+        if self.api_client.client_side_validation and ('owner' not in params or
+                                                       params['owner'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `owner` when calling `packages_validate_upload_swift`")  # noqa: E501
+        # verify the required parameter 'repo' is set
+        if self.api_client.client_side_validation and ('repo' not in params or
+                                                       params['repo'] is None):  # noqa: E501
+            raise ValueError("Missing the required parameter `repo` when calling `packages_validate_upload_swift`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'owner' in params:
+            path_params['owner'] = params['owner']  # noqa: E501
+        if 'repo' in params:
+            path_params['repo'] = params['repo']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'data' in params:
+            body_params = params['data']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['apikey']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/packages/{owner}/{repo}/validate-upload/swift/', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

## cloudsmith_api/models/__init__.py

```diff
@@ -172,14 +172,16 @@
 from cloudsmith_api.models.service_teams import ServiceTeams
 from cloudsmith_api.models.status_basic import StatusBasic
 from cloudsmith_api.models.storage_allocated_limit import StorageAllocatedLimit
 from cloudsmith_api.models.storage_allocated_limit_raw import StorageAllocatedLimitRaw
 from cloudsmith_api.models.storage_region import StorageRegion
 from cloudsmith_api.models.storage_usage import StorageUsage
 from cloudsmith_api.models.storage_usage_raw import StorageUsageRaw
+from cloudsmith_api.models.swift_package_upload import SwiftPackageUpload
+from cloudsmith_api.models.swift_package_upload_request import SwiftPackageUploadRequest
 from cloudsmith_api.models.tags import Tags
 from cloudsmith_api.models.terraform_package_upload import TerraformPackageUpload
 from cloudsmith_api.models.terraform_package_upload_request import TerraformPackageUploadRequest
 from cloudsmith_api.models.usage import Usage
 from cloudsmith_api.models.usage_fieldset import UsageFieldset
 from cloudsmith_api.models.usage_limits import UsageLimits
 from cloudsmith_api.models.usage_limits_raw import UsageLimitsRaw
```

## cloudsmith_api/models/helm_package_upload_request.py

```diff
@@ -30,36 +30,41 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'package_file': 'str',
+        'provenance_file': 'str',
         'republish': 'bool',
         'tags': 'str'
     }
 
     attribute_map = {
         'package_file': 'package_file',
+        'provenance_file': 'provenance_file',
         'republish': 'republish',
         'tags': 'tags'
     }
 
-    def __init__(self, package_file=None, republish=None, tags=None, _configuration=None):  # noqa: E501
+    def __init__(self, package_file=None, provenance_file=None, republish=None, tags=None, _configuration=None):  # noqa: E501
         """HelmPackageUploadRequest - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._package_file = None
+        self._provenance_file = None
         self._republish = None
         self._tags = None
         self.discriminator = None
 
         self.package_file = package_file
+        if provenance_file is not None:
+            self.provenance_file = provenance_file
         if republish is not None:
             self.republish = republish
         if tags is not None:
             self.tags = tags
 
     @property
     def package_file(self):
@@ -86,14 +91,40 @@
         if (self._configuration.client_side_validation and
                 package_file is not None and len(package_file) < 1):
             raise ValueError("Invalid value for `package_file`, length must be greater than or equal to `1`")  # noqa: E501
 
         self._package_file = package_file
 
     @property
+    def provenance_file(self):
+        """Gets the provenance_file of this HelmPackageUploadRequest.
+
+        The provenance file containing the signature for the chart. If one is not provided, it will be generated automatically.
+
+        :return: The provenance_file of this HelmPackageUploadRequest.
+        :rtype: str
+        """
+        return self._provenance_file
+
+    @provenance_file.setter
+    def provenance_file(self, provenance_file):
+        """Sets the provenance_file of this HelmPackageUploadRequest.
+
+        The provenance file containing the signature for the chart. If one is not provided, it will be generated automatically.
+
+        :param provenance_file: The provenance_file of this HelmPackageUploadRequest.
+        :type: str
+        """
+        if (self._configuration.client_side_validation and
+                provenance_file is not None and len(provenance_file) < 1):
+            raise ValueError("Invalid value for `provenance_file`, length must be greater than or equal to `1`")  # noqa: E501
+
+        self._provenance_file = provenance_file
+
+    @property
     def republish(self):
         """Gets the republish of this HelmPackageUploadRequest.
 
         If true, the uploaded package will overwrite any others with the same attributes (e.g. same version); otherwise, it will be flagged as a duplicate.
 
         :return: The republish of this HelmPackageUploadRequest.
         :rtype: bool
```

## cloudsmith_api/models/status_basic.py

```diff
@@ -38,15 +38,15 @@
     }
 
     attribute_map = {
         'detail': 'detail',
         'version': 'version'
     }
 
-    def __init__(self, detail='Cloudsmith API is operational.', version='1.263.0', _configuration=None):  # noqa: E501
+    def __init__(self, detail='Cloudsmith API is operational.', version='1.273.0', _configuration=None):  # noqa: E501
         """StatusBasic - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
 
         self._detail = None
         self._version = None
```

## test/test_packages_api.py

```diff
@@ -256,14 +256,21 @@
     def test_packages_upload_ruby(self):
         """Test case for packages_upload_ruby
 
         Create a new Ruby package  # noqa: E501
         """
         pass
 
+    def test_packages_upload_swift(self):
+        """Test case for packages_upload_swift
+
+        Create a new Swift package  # noqa: E501
+        """
+        pass
+
     def test_packages_upload_terraform(self):
         """Test case for packages_upload_terraform
 
         Create a new Terraform package  # noqa: E501
         """
         pass
 
@@ -424,14 +431,21 @@
     def test_packages_validate_upload_ruby(self):
         """Test case for packages_validate_upload_ruby
 
         Validate parameters for create Ruby package  # noqa: E501
         """
         pass
 
+    def test_packages_validate_upload_swift(self):
+        """Test case for packages_validate_upload_swift
+
+        Validate parameters for create Swift package  # noqa: E501
+        """
+        pass
+
     def test_packages_validate_upload_terraform(self):
         """Test case for packages_validate_upload_terraform
 
         Validate parameters for create Terraform package  # noqa: E501
         """
         pass
```

## Comparing `cloudsmith_api-2.0.3.dist-info/RECORD` & `cloudsmith_api-2.0.4.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-cloudsmith_api/__init__.py,sha256=7OHUHU3rrnJgK02ZONaolRJvdd6QvNxqZF7MtpZm2Gw,15910
-cloudsmith_api/api_client.py,sha256=HASptj_Sexdb0XKrFAjSEWIqLXd7q9bv3vNsMDB0d3Q,25067
-cloudsmith_api/configuration.py,sha256=ZSn2tDaIx7vAhxU3JHaF_G8vs7JnQWQj3933WYcoNdc,8390
+cloudsmith_api/__init__.py,sha256=8dyH4Dd5vPZFMamSZyUgDyQ5Bv7umS4wPMFa0LToloc,16073
+cloudsmith_api/api_client.py,sha256=Q8eA3qjIXNsPTvCce_1oSKvldm2adp6vjUCvtvA9HOM,25067
+cloudsmith_api/configuration.py,sha256=VeGgrK_xYegB3KfgD24B4IbRfH--FPTUp7bDb-ssxwI,8390
 cloudsmith_api/rest.py,sha256=IVGz52ALLAOqfC3YGAkqFfFjiLz5mAB_R0mIs51372Y,13166
 cloudsmith_api/api/__init__.py,sha256=oHMaETBtdkm77g6ZMGgBaWJb1Q3a8jlD8Nh02VKZd2U,1131
 cloudsmith_api/api/audit_log_api.py,sha256=cDN0Rsgck9w4qB19hpWzsTETl41Zsm-pk8Wrr14EDGs,11039
 cloudsmith_api/api/badges_api.py,sha256=PF8u5FZiEm1BFP8e52ZEDjzMo9skZVM9Qc7arsPk4vc,11425
 cloudsmith_api/api/distros_api.py,sha256=44C2sU3C43GkhRNPLK-jxlB8KrS8-KFe7Bj7KxAc-cU,7978
 cloudsmith_api/api/entitlements_api.py,sha256=Ao8Zk99xiIDEf-5GTz9YbgyaVig05QDGN0Pc2TpZmmo,54786
 cloudsmith_api/api/files_api.py,sha256=lsuhZ5M3ugbdQoqeci23QCYe15g2zVmJ3nF_nRsljZM,26620
 cloudsmith_api/api/formats_api.py,sha256=7Bv_EKqHBEnSHJIbtQ_oh-5laVu5EmofmZwBJo9h4og,7930
 cloudsmith_api/api/metrics_api.py,sha256=cTqkKtutQn2u-zNS7FHVTkxX-LSc3xRpjgbLDIqsWWc,19214
 cloudsmith_api/api/namespaces_api.py,sha256=2qCN92-asz_tZyASYgXE7gpAPBfL6W13khfmuOYV8CA,8514
 cloudsmith_api/api/orgs_api.py,sha256=mPEe7pszQCmE63DPPsc6HUXj3Z_5Awgh8gPRqTacNKQ,195413
-cloudsmith_api/api/packages_api.py,sha256=YV6Bq61JHgMEavSzrD9k86JN7YSUVTqL6djPQqtmzHY,284986
+cloudsmith_api/api/packages_api.py,sha256=8RLm6j343dJzWSWNAEUHqmmg86nTY2-UBzRCXb7U1-c,294424
 cloudsmith_api/api/quota_api.py,sha256=cLljkIY1w8-urDPf5Zi31YdaoWsyVrzKKz1t3Qasm_w,16386
 cloudsmith_api/api/rates_api.py,sha256=iVavoIQtWfbFE6C_jPnTQP8uG8wk0YS-ejHztrajZdY,4157
 cloudsmith_api/api/repos_api.py,sha256=9IYStNbWWFqBnTEQfDnB14Dfp4-jrVfMG7Ea0FBnKUo,98642
 cloudsmith_api/api/status_api.py,sha256=Y7fJjz1UeBzgC2y7F8EcnBuJIFUh553zQDdk1oLGOIQ,4118
 cloudsmith_api/api/storage_regions_api.py,sha256=27lr9PVQ8G84depb-1M7z1dJ5srWscFsU776W7SRVpc,8075
 cloudsmith_api/api/user_api.py,sha256=B2_HoP2ZNBYI-2GfmmSEmucylTZV_VhU7GnnP4aYPpE,7631
 cloudsmith_api/api/users_api.py,sha256=fjOMJWnFJ8qx5i5WkiR4cdpsKR2RzdoUT_V0w-TIZVM,4706
 cloudsmith_api/api/vulnerabilities_api.py,sha256=gF5GPsUNONLhHE7bf_MIvqlyNU967AZVm0wHNWmYIoY,22091
 cloudsmith_api/api/webhooks_api.py,sha256=RsnHyob8BKBLbqKHq3U7TizhcFJF-VCkgzJllmTZliw,26050
-cloudsmith_api/models/__init__.py,sha256=BozmJco6SwxgXq7a9r1qzkdNYDPQqOijgygLONWx2kU,14713
+cloudsmith_api/models/__init__.py,sha256=Tt-KCq4X7QKa-F8k91JLlPVJ26mf8S9s7bxQq1WBje8,14876
 cloudsmith_api/models/allocated_limit.py,sha256=1SlEiDZ2Ozouu8Gg6CrYf47I7pJjyxUOCFtJd7Q0yzA,7305
 cloudsmith_api/models/allocated_limit_raw.py,sha256=p6vlL-y9gGwoER9aLnDeexcM0Ci6W5as9765n74SfRE,5410
 cloudsmith_api/models/alpine_package_upload.py,sha256=IUVVXR1YrQt0d52V93rFkdkHGg5YkymjC4pjUKpcxrQ,58771
 cloudsmith_api/models/alpine_package_upload_request.py,sha256=jrzolgP1mvgRKgLiDfWe6J2VS9hywOudnbpg-8zM3lk,7437
 cloudsmith_api/models/architecture.py,sha256=bzGmeP8O7tYFZfdkboF5_E34LlX-NyN2HU4W9T1Bkds,4748
 cloudsmith_api/models/cargo_package_upload.py,sha256=y6a8rNJxe9H4GWMv72MJkqnCPP-7L3YfGALtFbn8RvI,58494
 cloudsmith_api/models/cargo_package_upload_request.py,sha256=RmfIq722CsU9jPUpsofwJRXdTzjwZ0OG8js66XFUPpQ,6177
@@ -59,15 +59,15 @@
 cloudsmith_api/models/eula.py,sha256=_dafCxq6v5Cz8HxaCyjTr0T-ka9oMqsc36vy_QLuAwk,5458
 cloudsmith_api/models/format.py,sha256=w9JIldZS2mRBRKo-4tYyPP9ve-4wdF-xTf9gEBvJMuI,11287
 cloudsmith_api/models/format_support.py,sha256=-TbnGczxma_ziAuD4ss-jwdHSPhE6cAI_za52K_Gbpg,7319
 cloudsmith_api/models/geo_ip_location.py,sha256=w5oOjWMH_GcOQtcUwVo0gWk_dDkPVGwmHJ2IC0RxURY,8615
 cloudsmith_api/models/go_package_upload.py,sha256=Slt7_6-PvfajmCK0wHQOKjbdwBA9qs4EgZf__MtSvFE,57663
 cloudsmith_api/models/go_package_upload_request.py,sha256=UgLfJ7yrqfuch7bEjriI8c151CWwStC21nsgOl3Hw4g,6126
 cloudsmith_api/models/helm_package_upload.py,sha256=1AwH6eg9iLHxOf-VK1lzNuWqof7zGa3D1YXjhx7YnrA,58217
-cloudsmith_api/models/helm_package_upload_request.py,sha256=QNb20d7lYd1U1y7gJ_Q5Htm5NMphVtry4U12Mcmfbas,6160
+cloudsmith_api/models/helm_package_upload_request.py,sha256=X4b94ShCVDyD9nsReMyrgvzq6MX8W51xyuC9cqbgQQE,7480
 cloudsmith_api/models/hex_package_upload.py,sha256=cPGtS3VlNKXbKRbuwuDOvM8FTzNOebDym4xM6u9oQ7Y,57940
 cloudsmith_api/models/hex_package_upload_request.py,sha256=q-4Uh4f2OJmPY4CDL-P6YhlMGpOogbakNnMcYUPBNhs,6143
 cloudsmith_api/models/history.py,sha256=17AfMvcTcXVi0L8gkqSdytdMeVbNRrLVSToP9SnWsxE,7028
 cloudsmith_api/models/history_fieldset.py,sha256=Cng-daGoLVr2Hc2tlZ7_lktiEllkIGUcKjcTKG0pU-Q,5168
 cloudsmith_api/models/history_fieldset_raw.py,sha256=EV7mi9q3pTap9fsh1cVuSpTUrHrQxcmUreT-EFoUcq0,5246
 cloudsmith_api/models/luarocks_package_upload.py,sha256=D8VMxUWsIKi-evMg-AJW0r89t3hVfhrlSfa6jDNYMjM,59325
 cloudsmith_api/models/luarocks_package_upload_request.py,sha256=FQc8EpOCyRHBRBOmLC9xAl0TlZihGUnLhCE-hUlnIjk,6228
@@ -174,20 +174,22 @@
 cloudsmith_api/models/rpm_package_upload_request.py,sha256=dI7_B02n2f4DhzcTl_dClukOTFHbuL2ITWwnTEyZrOM,7374
 cloudsmith_api/models/ruby_package_upload.py,sha256=cLi1WS4JxzNIRkDjUAMtIM_Fx12s_-Th51ysO_t08Bk,58217
 cloudsmith_api/models/ruby_package_upload_request.py,sha256=pA2MIcN9TvnQBQdh-W3VsQRgkB2VkQg4lWuFalrmHmw,6160
 cloudsmith_api/models/service.py,sha256=lhEXDlJBEf2h_uhqlb0gLo9fPePbEi9Ayo4aC6Zyo6w,8234
 cloudsmith_api/models/service_request.py,sha256=JOv9I8cUiQqTFOBomiwC3KVnewi8x2Rc6NUpp4wg42g,6726
 cloudsmith_api/models/service_request_patch.py,sha256=G3Kyh4R5MA_qsdxaqygbWco5zFqdRmklQGaW0MfAKGQ,6701
 cloudsmith_api/models/service_teams.py,sha256=JVUDlli2nc2oVtCGZQo29lHNQRuRuEsGKei-ShRyYlA,4951
-cloudsmith_api/models/status_basic.py,sha256=uZwbfEza4MD1w7Jci-mvQ39HvpfGN95KogngviBJrXI,4584
+cloudsmith_api/models/status_basic.py,sha256=fNvdikEqdPfseNeeaRBB1ytafDe6lijfTWZtzNSt0gI,4584
 cloudsmith_api/models/storage_allocated_limit.py,sha256=NkE1HLffx1kwuA0GamS5COBvOE3I0CyNa44Ox2vkTcQ,8478
 cloudsmith_api/models/storage_allocated_limit_raw.py,sha256=EZ2PZeIOBGfue8u0HVjurLNClceuFc5wH2UKoBqdtyQ,6140
 cloudsmith_api/models/storage_region.py,sha256=dx_5FJDAJmHrcNI4cBWiZJ6Jr06fFCA5TWYxGob9BTc,4670
 cloudsmith_api/models/storage_usage.py,sha256=EfRE_skvZ85zdc57ZKXwpacL85QGDSrMiYKf2sBQxMQ,6847
 cloudsmith_api/models/storage_usage_raw.py,sha256=fFnveEKU771hbXtZXfCV262Tm3B3RNJH6-4JPC4QFqA,5048
+cloudsmith_api/models/swift_package_upload.py,sha256=p8cHVupHOLYXRqAbsedWsXBrmRMJQffcLFjajXKZpGA,58865
+cloudsmith_api/models/swift_package_upload_request.py,sha256=9lc6XNXvJylOK71lsz9DizrG_dubk8sLMYm2miTU6wU,7279
 cloudsmith_api/models/tags.py,sha256=p-1Zwln_mYSv2tQ3naimZtoRiFgntVOAOd9phO2zuDw,2665
 cloudsmith_api/models/terraform_package_upload.py,sha256=hXd--8XCuyh1gj9XMwmAytVoKt9zIE3qsKTYhG5H-Ws,59602
 cloudsmith_api/models/terraform_package_upload_request.py,sha256=BNrLwg_Oo0D8SE3y2I-R_ZNFyV82NtzTnQiFu0mtsyY,6245
 cloudsmith_api/models/usage.py,sha256=Ul0g37TGK2PyaL52ktLDl_nHRtrM4VQ4C9FUdW1Grt8,5738
 cloudsmith_api/models/usage_fieldset.py,sha256=FtRfgLJlKKco4fH0BMrrVTUNUqYX5J3cpVPcOOaH3fA,4147
 cloudsmith_api/models/usage_limits.py,sha256=5SkxEF-RFwCFMb02sVRNU6h0ulk_L5tTpEiNshh5gL0,4277
 cloudsmith_api/models/usage_limits_raw.py,sha256=xgqXqPYTufrxi7kSW505N0TWxA8gV1lNs3IfTp9FRzU,4334
@@ -315,15 +317,15 @@
 test/test_package_tag.py,sha256=BkcYyKWhYR0zx_a940tYo5Pm4bguJW6fnpnIboBQBi4,868
 test/test_package_tag_request.py,sha256=HXsOuuK6Tfv6fqZw8r5-PihQTJekhC5_L8kfmyh2F0w,926
 test/test_package_usage_metrics.py,sha256=SA2_RAqLdmvnXrhKq4rFEMb6jJ0uj1sIZO-WjwU9NrE,942
 test/test_package_version_badge.py,sha256=FceEfshIzpn-tZWImTMJWnhpiHObWejQv2syqoOFJ4s,942
 test/test_package_vulnerability.py,sha256=mTIkCXM1qjoanj2t0zdhGxV6TUzo9mhNmUqI1hzMlTs,948
 test/test_package_vulnerability_policy_violation_log.py,sha256=iIrZ6ABnEq_AmAr3jUd9vR_FQh66W1xB7ztdstyFMY4,1098
 test/test_package_vulnerability_policy_violation_log_cursor_page.py,sha256=W5uSYYF6ZzUruutsT4Jj78KOEnNqzN-HZaIzB2IEn2Y,1182
-test/test_packages_api.py,sha256=rFq5IloMIrPnB7yynnQgB5pIyXQGQDn7AZPDIiXY42k,11377
+test/test_packages_api.py,sha256=wPP9ZmJOcM6ABeA-8q4AzyvfMgdeugeF8PhF1rNkXa0,11743
 test/test_python_package_upload.py,sha256=9TqfbGmuNwLq5E3K2DW3jSTsj3NIUlgmQwPLQWcH3YY,942
 test/test_python_package_upload_request.py,sha256=I2Si5Gxo2QZcYiqnG9rJoKD3_uwa58Kj5XUDVS-IUpw,1000
 test/test_quota.py,sha256=MBDyrqP8f-c-sfrwseJSKhJr8n-CHk_RdVWKnzXQVeY,826
 test/test_quota_api.py,sha256=9s116ymseG0AEs5GjlYvA6sZQt3TA8314jiigYyHQ8I,1364
 test/test_quota_history.py,sha256=He4i2YAkLW9vikiNV6RkUOQvs5gUqjRUxgHihqriPAw,884
 test/test_rate_check.py,sha256=3chA15laHCwLu0QXKOyTCdiJKJbOzAQOeUTftcsaGCg,860
 test/test_rates_api.py,sha256=eEs-UjEVTAr5b40hueduthNROAGZfwy6pEx2VQaRaHM,862
@@ -377,14 +379,16 @@
 test/test_status_basic.py,sha256=PbQ_cv693ykgjTXcdivquHSHITNicdB8fhxIcsmNsM0,876
 test/test_storage_allocated_limit.py,sha256=bWe-Ylveo3nl-qyRFA8QI3Dy_eZviX22ZU0LrGKeQHQ,958
 test/test_storage_allocated_limit_raw.py,sha256=B-ee2fuKpZK5Qrhw1w0zxH0iYkg0VmBEn4wTmbp5QGc,984
 test/test_storage_region.py,sha256=BjZSa-EkFeefRy-ZR9RBS5nXBtzp8APmMTJd6XdNJOk,892
 test/test_storage_regions_api.py,sha256=I1kmxtq2MflgNeyAUr09oEQvqpbatAEECihtdJOB5_E,1088
 test/test_storage_usage.py,sha256=6Eum1n3K6FDcPHGnSqrdeyr7-A_41WsFQj9rnfzLo1c,884
 test/test_storage_usage_raw.py,sha256=2K1DanJXtZiDRZnntbL0-dkkX23jEcwa8GLe8uCa4e0,910
+test/test_swift_package_upload.py,sha256=Xhr3eGmkITrT0svGQoX4Hn7AwvsP0RfXYw_wRZBIJuI,934
+test/test_swift_package_upload_request.py,sha256=jT3z5aN8ks1s71_B37g4vAeNZ0Q35Rw252xcJXzbW_s,992
 test/test_tags.py,sha256=d-lPTWDjFN_G7ihzyC3EIr-EmIQdODPGQ72x-l-yOBI,818
 test/test_terraform_package_upload.py,sha256=ynJhz-h8TJ0H89EvJA1TRodUKg-QFjyVQZdCwjEcz_I,966
 test/test_terraform_package_upload_request.py,sha256=P26Jc367hdg2hhMxMhdQvJsTHkoRgeCbgiWn_cytolM,1024
 test/test_usage.py,sha256=ncymPsT2Ld4xusH3JLtDA_ZsS5-z99JiWqC5p_HIl5g,826
 test/test_usage_fieldset.py,sha256=I1IrPs87hGgH63yJVzUJd_ALI0nhrlcbUao5S_-uF2g,892
 test/test_usage_limits.py,sha256=FRrQS2vtHdBYdO2Kw3UJYyNtOHSfcyNWrfcHQiPDlIQ,876
 test/test_usage_limits_raw.py,sha256=St3yDuTIv_4qFY6gHTbsNKpSXoWJEvQVbc2d2Av_TJA,902
@@ -401,11 +405,11 @@
 test/test_vulnerability.py,sha256=4QDPIFWXKuHg_oy9PTRqFhO8yvsur5VyUFhDVkQ-Dnc,890
 test/test_vulnerability_scan.py,sha256=mGc0AETJ-UP30jb32rN5LvHeP8KFteXB8afWUED2mfI,924
 test/test_vulnerability_scan_results.py,sha256=8-nfCw6UiVWIOsTyge5XETxWxfCkB4hQf4km2lQ3pVI,982
 test/test_vulnerability_scan_results_list.py,sha256=dtcBvhUgGr6LluGnjA6x7dqQ7bkeSbCuPJpKSdHm1kQ,1016
 test/test_vulnerability_scan_version.py,sha256=hgxu72nwZ8rfEgverNQQ9_DF1A-cxa0kIBXPkEEknuk,982
 test/test_webhook_template.py,sha256=kCtiNGZ65WVUpB0an-VxzQ6-F1k-w7kTmHqdgQLSKDU,908
 test/test_webhooks_api.py,sha256=ujU1QfkYPe4MwlMR0M-p2rEfSVTzPO1Q3uB8VLiDbOg,1557
-cloudsmith_api-2.0.3.dist-info/METADATA,sha256=tl3RDn7PkU9J2DysX0BXwFSQ7RT5WOif9sfrjcqNb5o,457
-cloudsmith_api-2.0.3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-cloudsmith_api-2.0.3.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
-cloudsmith_api-2.0.3.dist-info/RECORD,,
+cloudsmith_api-2.0.4.dist-info/METADATA,sha256=RcwXRBCyMAPNoi3BVMcN_xvBQ3S-ejmkJj7kOQWDAY4,457
+cloudsmith_api-2.0.4.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+cloudsmith_api-2.0.4.dist-info/top_level.txt,sha256=1t-msgoxqMBhQpKKvO2wukE1NWKEk_yDQh9eXqeDNfk,20
+cloudsmith_api-2.0.4.dist-info/RECORD,,
```

